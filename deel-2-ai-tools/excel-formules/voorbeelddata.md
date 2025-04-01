# Voorbeelddata: Excel-formules Genereren

## Dataset Beschrijving: Klimaatincidenten in Vlaanderen

Voor deze uitdaging werken we met een fictieve dataset van klimaatgerelateerde incidenten in verschillende Vlaamse gemeenten. Hiermee kun je oefenen met het genereren van diverse Excel-formules.

### Structuur van de spreadsheet

De dataset bevat de volgende kolommen:

- **Kolom A (Datum)**: De datum waarop het incident plaatsvond in formaat DD/MM/YYYY
- **Kolom B (Gemeente)**: Naam van de Vlaamse gemeente
- **Kolom C (Type Incident)**: Categorieën: "Wateroverlast", "Stormschade" of "Hittestress"
- **Kolom D (Omvang)**: Ernstgraad op een schaal van 1-5 (1=beperkt, 5=zeer ernstig)
- **Kolom E (Kosten)**: Geschatte economische schade in euro
- **Kolom F (Getroffenen)**: Aantal getroffene burgers

### Voorbeeld van de data (eerste rijen)

| Datum       | Gemeente    | Type Incident | Omvang | Kosten    | Getroffenen |
|------------|-------------|--------------|--------|-----------|-------------|
| 15/01/2024 | Gent        | Wateroverlast | 4      | 156.000   | 230         |
| 15/01/2024 | Antwerpen   | Wateroverlast | 3      | 98.500    | 185         |
| 17/01/2024 | Leuven      | Wateroverlast | 2      | 45.000    | 62          |
| 24/02/2024 | Brugge      | Stormschade   | 5      | 287.500   | 345         |
| 24/02/2024 | Oostende    | Stormschade   | 5      | 312.600   | 420         |
| 25/02/2024 | Gent        | Stormschade   | 4      | 178.900   | 250         |
| 12/03/2024 | Hasselt     | Wateroverlast | 3      | 87.300    | 140         |
| 14/04/2024 | Mechelen    | Wateroverlast | 2      | 42.500    | 75          |
| 03/06/2024 | Leuven      | Hittestress   | 3      | 58.200    | 182         |
| 15/06/2024 | Antwerpen   | Hittestress   | 4      | 125.000   | 430         |
| 16/06/2024 | Gent        | Hittestress   | 3      | 94.500    | 320         |
| 18/06/2024 | Hasselt     | Hittestress   | 4      | 112.400   | 285         |
| ...        | ...         | ...          | ...    | ...       | ...         |

### Voorbeelden van analyses die je zou kunnen maken

1. **Totale kosten per type incident**
   - Je zou de totale economische schade per type incident kunnen berekenen

2. **Gemeenten met de meeste getroffenen**
   - Je zou kunnen analyseren welke gemeenten het zwaarst getroffen zijn

3. **Seizoensgebonden patronen**
   - Je zou kunnen nagaan of bepaalde incidenttypen vaker voorkomen in bepaalde maanden

4. **Correlatie tussen omvang en kosten**
   - Je zou kunnen onderzoeken of er een duidelijk verband is tussen de ernstgraad en de economische schade

5. **Vergelijking kwartalen**
   - Je zou de impact van klimaatincidenten kunnen vergelijken tussen verschillende kwartalen

### Mogelijke uitdagingen voor formules

- Een formule die het gemiddelde aantal getroffenen berekent per omvangscategorie
- Een formule die de top 3 gemeenten vindt met de hoogste kosten voor wateroverlast
- Een formule die berekent hoeveel procent van de totale kosten wordt veroorzaakt door stormschade
- Een formule die incidenten telt die zowel grote omvang (4-5) als hoge aantallen getroffenen (>200) hebben
- Een formule die een dashboard-samenvatting maakt van totale getroffenen en kosten per kwartaal

Kies een van deze analyses of bedenk je eigen vraag waar je een Excel-formule voor nodig hebt.