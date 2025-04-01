# Uitdaging 5: Feitencheck-helper Bouwen
## Deel 2: Je Eigen AI-Tools Bouwen

## 🎯 Doel van deze uitdaging

Leer hoe je een AI-tool kunt maken die controleert of informatie feitelijk correct is en overeenkomt met een betrouwbare bron.

## 📋 Wat is een feitencheck-helper?

Een feitencheck-helper is een prompt-gebaseerde tool die systematisch controleert of beweringen in een tekst overeenkomen met de informatie in een referentiedocument.

### Wat zijn hallucinaties in AI?

"Hallucinaties" zijn wanneer AI-systemen informatie geven die niet waar is of niet in de bronnen staat. Dit kan gebeuren omdat:
- De AI probeert behulpzaam te zijn, zelfs als het niet alle informatie heeft
- De AI verbanden legt die niet echt bestaan
- De AI details invult die ontbreken

### Waarom is dit nuttig?

Als medewerker bij het Vlaams Parlement:
- Moet je werken met feitelijk correcte informatie
- Kan verkeerde informatie grote gevolgen hebben
- Moet je bronnen kunnen verifiëren
- Wil je niet onbedoeld onjuiste informatie verspreiden

Deze techniek helpt je om te controleren of informatie betrouwbaar is en waar mogelijk fouten zitten.

## 📚 Hoe werkt het?

**Zonder deze techniek:** Je krijgt een mooie samenvatting, maar weet niet of alles klopt

**Met deze techniek:** De AI controleert systematisch elke bewering tegen de brongegevens en markeert wat wel en niet onderbouwd is

## 🏋️ De Uitdaging

1. Gebruik het [referentiedocument en de te controleren tekst](./voorbeelddata.md) over het Klimaatactieplan Vlaanderen
2. Ontwerp een prompt die de AI laat controleren of de beweringen in de tekst overeenkomen met het referentiedocument
3. Laat de AI duidelijk markeren welke beweringen correct, deels correct of incorrect zijn
4. Test je prompt en beoordeel de nauwkeurigheid van de feitencheck

## 🛠️ Stap-voor-stap aanpak

1. **Definieer de verificatiecriteria**: Wat maakt een bewering correct, deels correct of incorrect?
2. **Structureer je prompt**: Vraag om een methodische aanpak voor het controleren van feiten
3. **Vraag om bronverwijzingen**: Elke beoordeling moet gebaseerd zijn op specifieke informatie uit het referentiedocument
4. **Creëer een duidelijk rapportageformaat**: Maak gebruik van tabellen of lijsten voor overzichtelijke resultaten
5. **Test je feitencheck-helper**: Voer een controle uit op tekst met bekende fouten

## 📝 Template om mee te beginnen

```
Ik heb een referentiedocument en een tekst die beweert informatie te geven gebaseerd op dit document.
Controleer systematisch of de beweringen in de tekst worden ondersteund door het referentiedocument.

Volg deze stappen:
1. Identificeer elke feitelijke bewering in de tekst
2. Controleer of deze bewering direct ondersteund wordt door het referentiedocument
3. Markeer elke bewering als:
   - ✓ CORRECT: volledig ondersteund door het document
   - ⚠️ DEELS CORRECT: gedeeltelijk ondersteund, maar met nuanceverschillen
   - ❌ INCORRECT: in tegenspraak met het document

Geef je analyse in een overzichtelijke tabel met kolommen:
- Bewering
- Beoordeling
- Toelichting
- Referentie in het document

REFERENTIEDOCUMENT:
[Plak hier het referentiedocument]

TE CONTROLEREN TEKST:
[Plak hier de te controleren tekst]
```

## ✨ Tips voor succes

- Wees duidelijk over de verificatiecriteria (wat maakt iets correct of incorrect?)
- Vraag om specifieke referenties naar het brondocument
- Gebruik een tabel- of lijstformaat voor duidelijke resultaten
- Overweeg meerdere categorieën (correct, deels correct, incorrect, niet verifieerbaar)
- Vraag om toelichting bij elke beoordeling

## 📊 Evaluatie

Beoordeel je resultaten op:
- Volledigheid: Zijn alle beweringen gecontroleerd?
- Nauwkeurigheid: Zijn de beoordelingen correct?
- Duidelijkheid: Is het resultaat gemakkelijk te begrijpen?
- Onderbouwing: Zijn de beoordelingen goed onderbouwd met verwijzingen?
- Bruikbaarheid: Is deze aanpak praktisch voor je dagelijkse werk?

## 🎓 Wat je hebt geleerd

Na het voltooien van deze uitdaging heb je geleerd:
- Hoe je AI kunt gebruiken om feitelijke accuraatheid te controleren
- Hoe je systematisch informatie kunt verifiëren tegen een referentiedocument
- Hoe je hallucinaties en onjuistheden kunt identificeren in AI-gegenereerde of menselijke tekst
- Hoe je dit kunt toepassen in je eigen werkprocessen

## 🔍 Voorbeeld oplossing

Bekijk een [voorbeeldoplossing](./voorbeeldoplossing.md) om te zien hoe een effectieve aanpak eruit kan zien.