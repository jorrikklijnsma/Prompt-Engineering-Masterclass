# Uitdaging 2: Juridische Extractie en Verificatie
## Deel 1: Rolspecifieke Prompt Engineering

## 🎯 Doel van deze uitdaging

Leer hoe je nauwkeurig en betrouwbaar specifieke informatie uit juridische teksten kunt extraheren met behulp van "referentiegerichte prompting".

## 📋 Wat is referentiegerichte prompting?

Referentiegerichte prompting is een techniek waarbij je de AI vraagt om alleen informatie te geven die rechtstreeks uit een brondocument komt, met exacte verwijzingen naar de bron.

### Waarom is dit nuttig voor juridische specialisten?

Als juridisch specialist bij het Vlaams Parlement:
- Moet je vaak grote hoeveelheden wetteksten doorwerken
- Is absolute precisie vereist - interpretaties kunnen grote gevolgen hebben
- Moet je snel specifieke informatie kunnen vinden zonder iets te missen
- Moeten beweringen altijd verifieerbaar zijn met bronverwijzingen

Deze techniek helpt je om betrouwbare, feitelijke extracties te maken uit juridische documenten zonder risico op "hallucinaties" of verkeerde interpretaties.

## 📚 Hoe werkt het?

**Zonder referentieprompt:** "Vat samen wat dit decreet zegt over privacy"  
*Resultaat:* Mogelijk een mix van feitelijke inhoud en interpretatie zonder duidelijke bronnen

**Met referentieprompt:** "Identificeer alle artikelen die privacy behandelen en citeer de exacte tekst"  
*Resultaat:* Precieze citaten met artikelnummers, zonder toevoegingen

## 🏋️ De Uitdaging

1. Gebruik het [voorbeelddecreet](./voorbeelddata.md) over klimaatadaptatiemaatregelen
2. Identificeer welke informatie je uit de wettekst wilt halen (termen, actoren, verplichtingen, deadlines, etc.)
3. Ontwerp een prompt die deze info extraheert en alleen feitelijke informatie uit de brontekst gebruikt
4. Bouw een verificatiestap in die controleert of alle informatie direct uit de brontekst komt
5. Test met de voorbeeldtekst en beoordeel de nauwkeurigheid

## 🛠️ Stap-voor-stap aanpak

1. **Identificeer informatiebehoeften**: Bepaal welke specifieke informatie je nodig hebt (bv. subsidiepercentages, deadlines, voorwaarden)
2. **Maak gerichte vragen**: Formuleer vragen die met specifieke tekstdelen beantwoord kunnen worden
3. **Vraag om citaten**: Vereis dat antwoorden citaten uit de brontekst bevatten
4. **Voeg verificatie toe**: Vraag de AI om te controleren of alle informatie direct uit de tekst komt
5. **Test en valideer**: Controleer of de antwoorden correct zijn door ze te vergelijken met de brontekst

## 📝 Template om mee te beginnen

```
Je bent een juridisch analist voor het Vlaams Parlement. Extraheer de volgende informatie uit de wettekst:

1. Wat is het maximale subsidiepercentage voor standaard projecten?
2. Wat is het maximumbedrag dat een lokaal bestuur kan ontvangen?
3. Welke deadline geldt voor het indienen van subsidieaanvragen?
4. Aan welke doelstellingen moeten klimaatadaptatiemaatregelen bijdragen?
5. Welke beoordelingscriteria worden gehanteerd?

Antwoord ALLEEN met informatie die letterlijk in de tekst staat.
Citeer voor elke extractie het relevante artikelnummer en paragraaf.
Als bepaalde informatie niet in de tekst staat, schrijf dan "Niet gespecificeerd".

VERIFICATIE:
Na extractie, controleer of alle informatie direct uit de brontekst komt.
Als er interpretatie is gebruikt, markeer dit duidelijk.

WETTEKST:
[Plak hier de voorbeelddecreet-tekst]
```

## ✨ Tips voor succes

- Formuleer je vragen zo specifiek mogelijk
- Vraag expliciet om bronverwijzingen (artikelnummers)
- Geef duidelijke instructies over wat te doen als informatie ontbreekt
- Gebruik de verificatiestap om het resultaat te controleren
- Beperk je vragen tot wat daadwerkelijk in de tekst te vinden is

## 📊 Evaluatie

Beoordeel je resultaten op:
- Nauwkeurigheid van de extracties
- Volledigheid van de bronverwijzingen
- Consistentie met de originele tekst
- Afwezigheid van interpretatie of toevoegingen
- Praktische bruikbaarheid voor je werk

## 🎓 Wat je hebt geleerd

Na het voltooien van deze uitdaging heb je geleerd:
- Hoe je gerichte informatie uit juridische teksten extraheert zonder interpretatie
- Hoe je AI kunt gebruiken om nauwkeurige en betrouwbare juridische analyses te maken
- Hoe je verificatiestappen kunt inbouwen om betrouwbaarheid te waarborgen
- Hoe je tijd kunt besparen bij het analyseren van lange wetteksten

## 🔍 Voorbeeld oplossing

Bekijk een [voorbeeldoplossing](./voorbeeldoplossing.md) om te zien hoe een effectieve aanpak eruit kan zien.