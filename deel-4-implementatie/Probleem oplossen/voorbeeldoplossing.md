# Voorbeeldoplossing: Probleemoplossing op de Werkplek

Deze voorbeeldoplossing demonstreert een creatieve promptstrategie voor Scenario 2: Geen document-uploads.

## Probleemstelling

**Beperking**: Je gebruikt een versie van een AI-tool die geen documentuploads ondersteunt. Je kunt alleen tekst kopiëren en plakken.

**Uitdaging**: Je moet een lang wetsvoorstel (30+ pagina's) analyseren, maar dit is te groot om in één keer te kopiëren en te plakken vanwege token-limieten.

**Context**: Als beleidsmedewerker bij het Vlaams Parlement moet je regelmatig lange beleidsdocumenten en wetsvoorstellen analyseren. De beveiligingsbeleid staat geen documentuploads toe in de beschikbare AI-tools, waardoor je beperkt bent tot kopiëren en plakken. Bovendien heeft het AI-systeem een token-limiet die het onmogelijk maakt om het hele document in één keer te verwerken.

## Doel

Een betrouwbare en grondige analyse maken van een lang wetsvoorstel zonder de mogelijkheid om het document te uploaden en ondanks de token-limiet.

## Creatieve prompt-strategie: De progressieve samenvattingsmethode

De oplossing is een methode in vier stappen:

1. **Segmentatie**: Verdeel het document in logische, behapbare secties (bijvoorbeeld per hoofdstuk of artikel)
2. **Progressieve samenvatting**: Vat elke sectie systematisch samen en bouw een cumulatieve kennis op
3. **Metagegevensoverdracht**: Gebruik een speciale structuur om kennis van eerdere secties door te geven aan latere analyses
4. **Holistische analyse**: Combineer alle samenvattingen voor een eindanalyse van het gehele document

Deze aanpak werkt als een soort "estafette" waarbij elke sessie met de AI een deel van het document analyseert en de belangrijkste punten doorgeeft aan de volgende ronde. Zo kan het model kennis opbouwen over het volledige document zonder dat je het hele document in één keer hoeft in te voeren.

## Promptsjablonen

### Stap 1: Initialisatie en structuurbepaling

```
Je bent een deskundige juridische analist die mij helpt bij het analyseren van een lang wetsvoorstel. 
Vanwege beperkingen kan ik het document alleen in delen aan je voorleggen.

Ik zal eerst de inhoudsopgave/structuur delen, zodat we een duidelijk beeld hebben van het volledige document.

INHOUDSOPGAVE/STRUCTUUR:
[Plak hier de inhoudsopgave of beschrijf de structuur van het wetsvoorstel]

Geef me op basis van deze structuur advies over:
1. Hoe we het document het beste kunnen opdelen in logische secties voor analyse (4-5 secties)
2. Wat voor soort informatie we per sectie moeten extraheren
3. Hoe we de analyse kunnen structureren voor een coherent eindresultaat
```

### Stap 2: Analyse van individuele secties

```
We zijn bezig met de analyse van het wetsvoorstel [TITEL]. 
Dit is SECTIE [X/Y]: [NAAM VAN DE SECTIE].

CONTEXT VAN VORIGE SECTIES (indien van toepassing):
[Korte samenvatting van de belangrijkste bevindingen uit vorige secties]

HUIDIGE SECTIE:
[Plak hier de tekst van de huidige sectie]

Analyseer deze sectie op de volgende aspecten:
1. Hoofddoel en kernbepalingen van deze sectie
2. Verplichtingen die worden opgelegd en aan wie
3. Deadlines of tijdlijnen die worden genoemd
4. Uitzonderingen of bijzondere bepalingen
5. Relatie tot eerdere secties (indien van toepassing)

Geef je analyse in een gestructureerd format dat gemakkelijk kan worden geïntegreerd met analyses van andere secties.
```

### Stap 3: Cumulatieve kennisoverdracht

```
We hebben nu [X] secties van het wetsvoorstel geanalyseerd. Hier is een beknopte samenvatting van wat we tot nu toe hebben:

SECTIE 1: [zeer beknopte samenvatting]
SECTIE 2: [zeer beknopte samenvatting]
...

We gaan nu verder met SECTIE [X+1]:
[Plak hier de tekst van de volgende sectie]

Analyseer deze nieuwe sectie met inachtneming van de voorafgaande informatie. Let specifiek op:
1. Hoe deze sectie voortbouwt op of verwijst naar eerder geanalyseerde delen
2. Nieuwe elementen die worden geïntroduceerd
3. Mogelijke tegenstrijdigheden met eerdere secties
```

### Stap 4: Holistische eindanalyse

```
We hebben nu alle secties van het wetsvoorstel [TITEL] geanalyseerd. Hier zijn de samenvattingen per sectie:

SECTIE 1: [samenvatting]
SECTIE 2: [samenvatting]
SECTIE 3: [samenvatting]
...

Op basis van deze gecombineerde informatie, geef een holistische analyse van het volledige wetsvoorstel:

1. Hoofddoel en reikwijdte
2. Belangrijkste verplichtingen en betrokkenen
3. Implementatietraject en tijdlijnen
4. Potentiële uitdagingen of onduidelijkheden
5. Samenhang en consistentie tussen de verschillende delen
6. Algemene implicaties en aandachtspunten

Structureer je analyse in een format dat direct bruikbaar is voor beleidsadvisering.
```

## Implementatiestappen

1. **Voorbereidingsfase**:
   - Print het wetsvoorstel uit of open het in een document viewer
   - Identificeer de inhoudsopgave of globale structuur
   - Maak een plan voor logische secties op basis van hoofdstukken, artikelen of thema's

2. **Segmentatie en initiële analyse**:
   - Gebruik de eerste prompt om een strategisch segmentatieplan te krijgen
   - Volg het advies van de AI om het document op te delen in logische secties
   - Maak een document waar je de analyses per sectie kunt bijhouden

3. **Progressieve analyse-ronde**:
   - Begin met de eerste sectie en gebruik de tweede prompt
   - Kopieer en bewaar de analyse van deze sectie
   - Ga door naar de volgende sectie met de derde prompt, waarbij je een zeer beknopte samenvatting van de vorige sectie(s) meegeeft
   - Herhaal dit proces voor alle secties

4. **Holistische eindanalyse**:
   - Gebruik de vierde prompt en voeg beknopte samenvattingen van alle secties toe
   - Vraag om een geïntegreerde analyse van het gehele document
   - Sla het eindresultaat op voor gebruik in je beleidsadvies

5. **Verificatie en aanvulling**:
   - Controleer de eindanalyse op consistentie met het originele document
   - Stel gerichte vervolgvragen over specifieke onderdelen indien nodig

## Evaluatie

### Effectiviteit
- **Hoog**: Deze methode stelt je in staat om een 30+ pagina's document te analyseren binnen de beperkingen van token-limieten en zonder upload-mogelijkheden
- **Betrouwbaar**: Door het systematisch opbouwen van kennis over het document, worden belangrijke verbanden en afhankelijkheden niet gemist
- **Flexibel**: De methode is aanpasbaar aan verschillende typen documenten en specifieke analysebehoeften

### Beperkingen
- **Tijdsinvestering**: Vereist meer tijd dan een enkele analyse van het volledige document
- **Handmatig proces**: Het opdelen en kopiëren van secties is een handmatig proces
- **Risico op inconsistenties**: Er is een risico dat de cumulatieve kennis niet perfect wordt overgedragen tussen de verschillende analyse-rondes
- **Beknoptheid vereist**: Bij zeer lange documenten moeten de samenvattingen van eerdere secties mogelijk te beknopt zijn

### Alternatieven overwogen

1. **Losse fragmentanalyse**: Elke sectie volledig onafhankelijk analyseren zonder context van voorgaande secties
   - **Nadeel**: Mist verbanden en samenhang tussen de verschillende delen

2. **Extremere samenvatting**: Eerst het hele document laten samenvatten in zeer beknopte vorm, en dan dieper ingaan op specifieke secties
   - **Nadeel**: Risico op het missen van belangrijke details in de eerste samenvattingsfase

3. **Gerichte vraag-antwoordronde**: In plaats van systematische analyse, gerichte vragen stellen over specifieke aspecten van het document
   - **Nadeel**: Vereist dat je al weet waar je naar zoekt en kan belangrijke aspecten missen

## Toepassingsgebieden

Deze strategie is niet alleen nuttig voor wetsvoorstellen, maar kan worden toegepast op verschillende soorten lange documenten:

1. **Strategische beleidsplannen**
2. **Jaarverslagen en begrotingsdocumenten**
3. **Uitgebreide onderzoeksrapporten**
4. **Internationale verdragen of overeenkomsten**
5. **Complexe subsidiereglementen**

Door deze methode aan te passen aan je specifieke behoeften, kun je effectief werken met AI-tools ondanks beperkingen in upload-mogelijkheden en token-limieten.