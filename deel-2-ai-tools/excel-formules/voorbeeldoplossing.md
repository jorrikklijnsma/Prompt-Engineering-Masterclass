# Voorbeeldoplossing: Excel-formules Genereren

## Effectieve prompt

```
Je bent een Excel-expert met uitgebreide ervaring in data-analyse. Ik ben een beleidsmedewerker bij het Vlaams Parlement en werk met klimaatdata. Ik heb een beperkte Excel-kennis en zou graag je hulp krijgen bij het maken van een formule voor een belangrijk rapport over klimaatincidenten.

Ik wil een formule maken die:
1. De top 3 gemeenten toont met de hoogste totale kosten door wateroverlast
2. Alleen incidenten uit het eerste kwartaal van 2024 (januari t/m maart) meetelt
3. Per gemeente ook het aantal getroffenen toont
4. De gemeenten sorteert van hoogste naar laagste kosten

Mijn spreadsheet heeft de volgende kolommen:
- Kolom A (Datum): Datums in formaat DD/MM/YYYY
- Kolom B (Gemeente): Naam van de gemeente
- Kolom C (Type Incident): "Wateroverlast", "Stormschade" of "Hittestress"
- Kolom D (Omvang): Ernstgraad op schaal 1-5
- Kolom E (Kosten): Economische schade in euro
- Kolom F (Getroffenen): Aantal getroffen burgers

Geef me:
1. Een Excel-formule of -methode die ik hiervoor kan gebruiken
2. Een stap-voor-stap uitleg in eenvoudige taal (zonder vakjargon) hoe ik deze moet toepassen
3. Een voorbeeld van hoe het resultaat eruit kan zien
4. Eventuele alternatieve benaderingen die voor een beginner zoals ik misschien makkelijker te begrijpen zijn

Let op: ik heb geen ervaring met VBA of geavanceerde Excel-functies zoals LAMBDA.

Ik waardeer extra je hulp om me niet alleen de formule te geven maar ook te helpen begrijpen hoe deze werkt, zodat ik deze in de toekomst kan aanpassen voor vergelijkbare analyses.
```

## Resultaat: Excel-formule oplossing

### Oplossing: Top 3 gemeenten met hoogste kosten door wateroverlast in Q1 2024

#### Beste benadering: Draaitabel

Voor dit soort analyse is een draaitabel de meest gebruiksvriendelijke oplossing, vooral als je beperkte Excel-ervaring hebt.

**Stap-voor-stap handleiding:**

1. **Selecteer alle data** in je spreadsheet (inclusief de koprij)

2. **Maak een draaitabel:**
   - Klik op het tabblad "Invoegen" in de Excel-menubalk
   - Klik op "Draaitabel" (meestal links in het lint)
   - Controleer of het juiste gegevensbereik is geselecteerd
   - Kies "Nieuw werkblad" en klik op OK

3. **Stel de draaitabel in:**
   - Sleep "Gemeente" naar het vak "Rijen"
   - Sleep "Kosten" naar het vak "Waarden"
   - Sleep "Getroffenen" naar het vak "Waarden"

4. **Voeg filters toe:**
   - Sleep "Type Incident" naar het vak "Filters"
   - Sleep "Datum" naar het vak "Filters"

5. **Pas de filters aan:**
   - Klik op de filterpijl bij "Type Incident" en selecteer alleen "Wateroverlast"
   - Klik op de filterpijl bij "Datum" en:
     - Kies "Datumfilters" → "Tussen"
     - Vul bij "Begin" 01/01/2024 in
     - Vul bij "Einde" 31/03/2024 in
     - Klik op OK

6. **Sorteer de resultaten:**
   - Klik ergens in de kolom "Som van Kosten"
   - Klik op het tabblad "Gegevens" in de menubalk
   - Klik op "Aflopend sorteren" (Z→A pictogram)

7. **Beperk tot top 3:**
   - Je kunt nu eenvoudig de eerste drie rijen aflezen als je top 3

#### Voorbeeld van het resultaat:

| Gemeente    | Som van Kosten | Som van Getroffenen |
|-------------|----------------|---------------------|
| Gent        | 156.000        | 230                 |
| Antwerpen   | 98.500         | 185                 |
| Hasselt     | 87.300         | 140                 |

#### Alternatieve oplossing met formules:

Als je toch liever met formules werkt, kun je deze aanpak gebruiken:

**Stap 1: Maak een hulptabel voor de berekeningen**
In een nieuw gebied van je spreadsheet, bijvoorbeeld vanaf cel H1:

1. Maak een tabel met deze koppen:
   ```
   H1: Gemeente
   I1: Totale Kosten Wateroverlast Q1
   J1: Totaal Getroffenen Wateroverlast Q1
   ```

2. In cel H2, maak een lijst van unieke gemeenten:
   ```
   =UNIQUE(B2:B1000)
   ```
   (Pas het bereik aan op basis van je gegevens)

**Stap 2: Bereken de totale kosten per gemeente**
In cel I2 (naast de eerste gemeente) gebruik je deze formule:
```
=SUMIFS(E2:E1000, B2:B1000, H2, C2:C1000, "Wateroverlast", A2:A1000, ">=01/01/2024", A2:A1000, "<=31/03/2024")
```

**Stap 3: Bereken het totale aantal getroffenen per gemeente**
In cel J2 gebruik je een vergelijkbare formule:
```
=SUMIFS(F2:F1000, B2:B1000, H2, C2:C1000, "Wateroverlast", A2:A1000, ">=01/01/2024", A2:A1000, "<=31/03/2024")
```

**Stap 4: Kopieer de formules naar beneden** voor alle gemeenten in kolom H

**Stap 5: Sorteer de resultaten**
1. Selecteer het gehele gebied (H1:J en alle rijen met data)
2. Klik op Gegevens → Sorteren
3. Sorteer op "Totale Kosten Wateroverlast Q1" van groot naar klein

**Stap 6: Je top 3 zijn nu** de eerste drie rijen in je gesorteerde tabel.

#### Uitleg van de SUMIFS formule

De `SUMIFS` formule werkt als volgt:
- Eerste argument `E2:E1000`: Dit zijn de cellen waarvan we de waarden willen optellen (de kosten)
- De volgende argumenten komen in paren (bereik, criteria):
  - `B2:B1000, H2`: Tel alleen als de gemeente overeenkomt met de gemeente in cel H2
  - `C2:C1000, "Wateroverlast"`: Tel alleen als het type incident "Wateroverlast" is
  - `A2:A1000, ">=01/01/2024"`: Tel alleen als de datum op of na 1 januari 2024 is
  - `A2:A1000, "<=31/03/2024"`: Tel alleen als de datum op of voor 31 maart 2024 is

#### Waarom de draaitabel-methode beter is voor beginners

1. **Geen complexe formules nodig**: Je hoeft geen formules te schrijven of te begrijpen
2. **Visuele interface**: Je kunt velden slepen en neerzetten in plaats van formules te typen
3. **Eenvoudig aan te passen**: Filters en sorteringen kun je met een paar klikken wijzigen
4. **Minder foutgevoelig**: Minder kans op typfouten of formulefouten
5. **Direct resultaat**: Je ziet onmiddellijk het resultaat van je aanpassingen

## Waarom deze aanpak effectief is

1. **Begrijpt de gebruiker**:
   - De prompt erkent het vaardigheidsniveau (beperkte Excel-kennis)
   - Vraagt expliciet om eenvoudige uitleg zonder vakjargon
   - Vermijdt geavanceerde functies die de gebruiker niet kent

2. **Context is specifiek**:
   - Vermeldt de rol van de gebruiker (beleidsmedewerker)
   - Beschrijft het concrete doel (rapport over klimaatincidenten)
   - Geeft alle relevante details over de data

3. **Duidelijke verwachtingen**:
   - Precies gespecificeerd wat de formule moet doen (4 punten)
   - Vraagt om meerdere soorten output (formule, uitleg, voorbeeld, alternatieven)

4. **Leermoment ingebouwd**:
   - Vraagt niet alleen om de oplossing maar ook om begrip
   - Vermeldt het doel om in de toekomst zelf aanpassingen te kunnen maken

5. **Resultaat is praktisch bruikbaar**:
   - Biedt meerdere oplossingsmethoden aan
   - Geeft stap-voor-stap instructies
   - Legt uit waarom één methode beter is dan de andere

Deze aanpak zorgt ervoor dat je niet alleen een oplossing krijgt voor je huidige probleem, maar ook beter wordt in het gebruiken van Excel voor toekomstige taken.