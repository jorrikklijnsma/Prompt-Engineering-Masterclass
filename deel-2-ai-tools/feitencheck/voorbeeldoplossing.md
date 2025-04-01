# Voorbeeldoplossing: Feitencheck-helper Bouwen

## Effectieve prompt

```
Ik ben een onderzoeker bij het Vlaams Parlement en moet controleren of een samenvatting van het Klimaatactieplan Vlaanderen 2025-2030 feitelijk correct is. Help me systematisch te verifiëren of de beweringen in de tekst overeenkomen met het officiële referentiedocument.

Volg deze methodologie:

1. IDENTIFICATIE: Extraheer eerst alle feitelijke beweringen uit de te controleren tekst. Beschouw elke cijfermatige claim, datumvermelding of specifieke maatregel als een aparte bewering.

2. VERIFICATIE: Controleer elke bewering tegen het referentiedocument en categoriseer als:
   * ✓ CORRECT: De bewering komt volledig overeen met het referentiedocument
   * ⚠️ DEELS CORRECT: De bewering heeft gedeeltelijk gelijk maar bevat ook nuanceverschillen, afrondingen of kleine onnauwkeurigheden
   * ❌ INCORRECT: De bewering is duidelijk in tegenspraak met het referentiedocument
   * ❓ NIET VERIFIEERBAAR: De bewering kan niet geverifieerd worden op basis van het referentiedocument

3. ONDERBOUWING: Voor elke beoordeling, geef:
   * De exacte tekst uit het referentiedocument die je beoordeling ondersteunt
   * Een korte toelichting waarom de bewering correct of incorrect is
   * Bij deels correcte beweringen, specificeer precies wat klopt en wat niet klopt

4. OVERZICHTELIJKE PRESENTATIE: Presenteer je resultaten in een gestructureerde tabel met deze kolommen:
   * Bewering (uit de te controleren tekst)
   * Beoordeling (correct/deels correct/incorrect/niet verifieerbaar)
   * Referentie (exacte tekstdeel uit het referentiedocument)
   * Toelichting (uitleg van je beoordeling)

5. SAMENVATTING: Sluit af met een overzicht van hoeveel beweringen in elke categorie vallen en welke soorten fouten het meest voorkomen.

REFERENTIEDOCUMENT:
[Plak hier het referentiedocument]

TE CONTROLEREN TEKST:
[Plak hier de te controleren tekst]
```

## Resultaat: Feitelijke verificatierapport

### Verificatierapport Klimaatactieplan Vlaanderen 2025-2030

#### Gedetailleerde analyse van beweringen

| Bewering | Beoordeling | Referentie | Toelichting |
|----------|------------|------------|-------------|
| "Vlaanderen wil 60% minder broeikasgassen uitstoten tegen 2030 vergeleken met 1990." | ❌ INCORRECT | "55% reductie van broeikasgasemissies tegen 2030 (t.o.v. 1990)" | De doelstelling is 55% emissiereductie, niet 60%. |
| "Het plan voorziet in €5 miljard aan investeringen" | ❌ INCORRECT | "Totaalbudget: €4,3 miljard over 5 jaar (2025-2030)" | Het totaalbudget is €4,3 miljard, niet €5 miljard. |
| "waarvan het grootste deel uit het Klimaatfonds komt." | ❌ INCORRECT | "Klimaatfonds: €1,2 miljard<br>Europese cofinanciering: €1,5 miljard<br>Private investeringen: €1,6 miljard" | Het Klimaatfonds draagt €1,2 miljard bij, wat niet het grootste deel is. Zowel de Europese cofinanciering (€1,5 miljard) als private investeringen (€1,6 miljard) dragen meer bij. |
| "Vlaanderen jaarlijks 150.000 woningen renoveren" | ❌ INCORRECT | "100.000 woningrenovaties per jaar vanaf 2026" | Het plan voorziet in 100.000 woningrenovaties per jaar, niet 150.000. |
| "een verbod op nieuwe gasaansluitingen ingevoerd vanaf 2026" | ❌ INCORRECT | "Verbod op nieuwe aardgasaansluitingen vanaf 2027" | Het verbod op nieuwe aardgasaansluitingen gaat in vanaf 2027, niet 2026. |
| "een doelstelling van 75% elektrische auto's in de nieuwe verkoop tegen 2028" | ❌ INCORRECT | "50% van nieuw verkochte auto's elektrisch tegen 2028" | De doelstelling is 50% elektrische auto's in de nieuwe verkoop tegen 2028, niet 75%. |
| "Er komen 30.000 nieuwe laadpunten." | ⚠️ DEELS CORRECT | "Uitbreiding laadinfrastructuur: 35.000 publieke laadpunten tegen 2030" | De te controleren tekst noemt 30.000 nieuwe laadpunten, terwijl het referentiedocument specificeert dat er 35.000 publieke laadpunten komen tegen 2030. Het aantal is afgerond naar beneden en mist de tijdsaanduiding. |
| "verdrievoudigt Vlaanderen zijn zonne-energiecapaciteit van 5,2 GW naar 15 GW" | ❌ INCORRECT | "Capaciteit zonne-energie: van 5,2 GW (2023) naar 12 GW (2030)" | De zonne-energiecapaciteit zal toenemen van 5,2 GW naar 12 GW, niet naar 15 GW. |
| "wordt alle steenkoolgebruik in de industrie uitgefaseerd tegen 2028" | ✓ CORRECT | "Uitfasering steenkool in industrie tegen 2028" | Deze bewering komt volledig overeen met het referentiedocument. |
| "Het plan bevat ook een renovatieplicht bij verkoop voor woningen met een slecht energielabel (D, E of F)." | ❌ INCORRECT | "Renovatieplicht bij verkoop voor woningen met EPC-label E of F" | De renovatieplicht geldt alleen voor woningen met EPC-label E of F, niet voor woningen met label D. |

#### Samenvatting van de verificatie

- **Correcte beweringen**: 1 (10%)
- **Deels correcte beweringen**: 1 (10%)
- **Incorrecte beweringen**: 8 (80%)
- **Niet verifieerbare beweringen**: 0 (0%)

#### Meest voorkomende fouten:
1. **Overdrijving van cijfers**: Emissiereductie (60% i.p.v. 55%), woningrenovaties (150.000 i.p.v. 100.000), elektrische auto's (75% i.p.v. 50%), zonne-energie (15 GW i.p.v. 12 GW)
2. **Foutieve jaartallen**: Verbod op gasaansluitingen (2026 i.p.v. 2027)
3. **Verkeerde financiële gegevens**: Totaalbudget (€5 miljard i.p.v. €4,3 miljard) en verdeling (Klimaatfonds als grootste deel)
4. **Onterechte uitbreiding van doelgroepen**: Renovatieplicht inclusief woningen met label D

## Waarom deze aanpak effectief is

1. **Systematische methode**:
   - Duidelijke stapsgewijze aanpak (identificatie → verificatie → onderbouwing → presentatie → samenvatting)
   - Behandelt elke bewering als een aparte claim die moet worden geverifieerd
   - Zorgt ervoor dat niets wordt gemist

2. **Duidelijke categorisering**:
   - Vier categorieën (correct, deels correct, incorrect, niet verifieerbaar) bieden nuance
   - Visuele markeringen (✓, ⚠️, ❌, ❓) maken de beoordeling direct herkenbaar
   - Focus op nauwkeurigheid door onderscheid te maken tussen volledig fout en deels correct

3. **Grondige onderbouwing**:
   - Elke beoordeling wordt ondersteund door specifieke tekstdelen uit het referentiedocument
   - Toelichting verduidelijkt wat precies correct of incorrect is
   - Bij gedeeltelijk correcte beweringen wordt gespecificeerd wat klopt en wat niet

4. **Overzichtelijke presentatie**:
   - Tabelformaat maakt de informatie gemakkelijk scanbaar
   - Consistente structuur voor alle beweringen
   - Samenvatting geeft een duidelijk overzicht van de algemene betrouwbaarheid

5. **Praktische toepasbaarheid**:
   - De methode is toepasbaar op verschillende soorten documenten
   - De samenvatting helpt patronen te identificeren in fouten
   - Het format is direct bruikbaar voor rapportage of besluitvorming

Deze aanpak is bijzonder nuttig voor:
- Het controleren van beleidsdocumenten voor publicatie
- Het verifiëren van persberichten en communicatiemateriaal
- Het analyseren van samenvattingen van complexe rapporten
- Training van medewerkers in accuraat communiceren over beleid
- Het identificeren van systematische fouten in informatiestromen