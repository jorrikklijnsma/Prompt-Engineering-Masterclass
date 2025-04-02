# Overzicht Prompt Engineering Technieken
## Masterclass Vlaams Parlement

Dit document biedt een overzicht van de belangrijkste prompt engineering technieken die in de masterclass zijn behandeld, inclusief wanneer en hoe je ze het beste kunt toepassen.

## 1. Basisprincipes voor effectieve prompts

### Duidelijkheid
- **Wat**: Expliciete, ondubbelzinnige instructies
- **Voorbeeld**: "Vat dit samen in precies 100 woorden" (niet: "Maak dit korter")
- **Wanneer**: Altijd, maar vooral bij complexe opdrachten

### Specificiteit
- **Wat**: Concrete parameters en verwachtingen
- **Voorbeeld**: "Gebruik formele taal geschikt voor een parlementair document, zonder jargon"
- **Wanneer**: Als je een specifiek resultaat nodig hebt

### Structuur
- **Wat**: Duidelijke opbouw en opdeling van de prompt
- **Voorbeeld**: Gebruik kopjes, nummering en witregels voor verschillende instructies
- **Wanneer**: Bij complexe prompts met meerdere componenten

### Context
- **Wat**: Relevante achtergrondinformatie
- **Voorbeeld**: "Je schrijft voor een publiek dat bekend is met de basisprincipes maar niet met recente ontwikkelingen"
- **Wanneer**: Als de AI specifieke kennis nodig heeft over doelgroep, doel of context

### Parameters
- **Wat**: Meetbare criteria en beperkingen
- **Voorbeeld**: "Maximaal 500 woorden", "Focus op deze 3 aspecten", "Gebruik ten minste 2 voorbeelden"
- **Wanneer**: Als je controle wilt over de lengte, focus of diepgang

## 2. Rolspecifieke technieken

### Few-shot learning (leren door voorbeelden)
- **Wat**: Voorbeelden geven van wat je wilt
- **Voorbeeld**: "Herschrijf zoals dit voorbeeld: [voorbeeld]"
- **Wanneer**: Voor communicatieprofessionals die teksten voor verschillende doelgroepen moeten schrijven
- **Voordeel**: Zeer effectief in het sturen van stijl, toon en format

### Referentiegerichte prompting
- **Wat**: Vragen om alleen informatie uit een specifieke bron te gebruiken
- **Voorbeeld**: "Gebruik alleen informatie uit de wettekst, met exacte citaten en artikelnummers"
- **Wanneer**: Voor juridische analyses waarbij nauwkeurigheid cruciaal is
- **Voordeel**: Voorkomt "hallucinaties" en zorgt voor verifieerbare output

### Template-based prompting
- **Wat**: Een specifiek format of sjabloon voorschrijven
- **Voorbeeld**: "Gebruik dit format: [gedetailleerd sjabloon]"
- **Wanneer**: Voor administratieve taken zoals het structureren van notities
- **Voordeel**: Zorgt voor consistente en direct bruikbare output

## 3. Geavanceerde workflow-strategieën

### Context-opbouw methode
- **Wat**: Eerst expertise delen en corrigeren, dan pas creëren
- **Stappen**: 1) Laat AI uitleggen 2) Corrigeer 3) Gebruik voor nieuwe creatie
- **Wanneer**: Voor specialistische onderwerpen waar nauwkeurigheid belangrijk is
- **Voordeel**: Zorgt dat AI jouw expertise gebruikt voor betere resultaten

### Monoloog vs. dialoog
- **Monoloog**: Één lange, gedetailleerde prompt
  - **Wanneer**: Voor gestandaardiseerde, herhaalde taken
  - **Voordeel**: Gemakkelijk te kopiëren en hergebruiken
- **Dialoog**: Stapsgewijze interactie
  - **Wanneer**: Voor complexe of creatieve taken die tussentijdse feedback nodig hebben
  - **Voordeel**: Mogelijkheid om bij te sturen tijdens het proces

### Multi-chat pijplijnen
- **Wat**: Verschillende chats voor verschillende fasen van een taak
- **Stappen**: 1) Onderzoeker 2) Structureerder 3) Schrijver 4) Editor
- **Wanneer**: Voor complexe documenten die meerdere expertises vereisen
- **Voordeel**: Specialisatie per fase leidt tot betere resultaten

## 4. Praktische implementatie-technieken

### Progressieve samenvattingsmethode
- **Wat**: Grote documenten in delen analyseren met kennisoverdracht
- **Stappen**: 1) Segmentatie 2) Analyse per segment 3) Cumulatieve kennis opbouwen
- **Wanneer**: Bij langere documenten zonder upload-mogelijkheid
- **Voordeel**: Omzeilt token-limieten terwijl verbanden behouden blijven

### Abstractiemethode voor gevoelige informatie
- **Wat**: Werken met structuren en templates zonder inhoud te delen
- **Voorbeeld**: "Coach me door het proces zonder dat ik de inhoud deel"
- **Wanneer**: Bij vertrouwelijke informatie die niet gedeeld kan worden
- **Voordeel**: Behoudt privacy terwijl je toch AI-assistentie krijgt

### Single-chat workflow simulatie
- **Wat**: Meerdere fasen simuleren binnen één chat
- **Voorbeeld**: "Dit is FASE 2. Hier is een samenvatting van FASE 1: [...]"
- **Wanneer**: Als je beperkt bent tot één enkele chat-sessie
- **Voordeel**: Biedt structuur binnen de beperkingen van één chat

## Keuzehulp: Welke techniek wanneer?

| Als je wilt... | Gebruik deze techniek |
|----------------|----------------------|
| Tekst aanpassen voor verschillende doelgroepen | Few-shot learning |
| Juridische teksten nauwkeurig analyseren | Referentiegerichte prompting |
| Ongestructureerde informatie organiseren | Template-based prompting |
| Complexe berekeningen maken zonder expertise | Formula generation |
| De juistheid van informatie controleren | Fact checking prompts |
| Specialistische documenten maken | Context-opbouw methode |
| Een complexe taak stap voor stap aanpakken | Dialoogaanpak |
| Een complex document maken met verschillende aspecten | Multi-chat pijplijn |
| Lange documenten analyseren | Progressieve samenvattingsmethode |
| Met vertrouwelijke informatie werken | Abstractiemethode |

## Praktijktips voor het Vlaams Parlement

1. **Begin eenvoudig**: Start met basisprincipes en bouw van daaruit op naar complexere technieken
2. **Documenteer succesvolle prompts**: Bewaar prompts die goed werken voor hergebruik
3. **Iteratief werken**: Verfijn je prompts op basis van de resultaten
4. **Denk aan de balans**: Weeg tijdsinvestering in complexe technieken af tegen de meerwaarde
5. **Deel kennis**: Laat collega's meekijken en van elkaar leren

## Verdiepingsmateriaal

Voor verdere verdieping in deze technieken, bekijk de uitgewerkte voorbeelden in de bijbehorende uitdagingen van de masterclass: