# Uitdaging 8: Multi-Chat Pijplijnen
## Deel 3: Geavanceerde Workflow-strategieën

## 🎯 Doel van deze uitdaging

Leer hoe je verschillende AI-chats kunt gebruiken voor verschillende stappen in een workflow, om complexere taken op te delen en betere resultaten te krijgen.

## 📋 Wat zijn Multi-Chat Pijplijnen?

Een multi-chat pijplijn is een aanpak waarbij je meerdere, afzonderlijke chats gebruikt voor verschillende fasen van een taak. Elke chat is gespecialiseerd in een specifiek aspect, en de output van één chat wordt (mogelijk na menselijke bewerking) de input voor de volgende chat.

### Waarom is dit nuttig?

Als medewerker bij het Vlaams Parlement:
- Werk je aan complexe documenten die meerdere bewerkingsstappen vereisen
- Kun je taken beter opdelen in fasen (onderzoek, schrijven, redigeren)
- Wil je verschillende prompting-strategieën gebruiken voor verschillende aspecten
- Heb je mogelijk verschillende specialisten nodig voor verschillende onderdelen

Deze techniek helpt je om grotere, complexere taken efficiënt aan te pakken door deze op te delen in behapbare stukken.

## 📚 Hoe het werkt: De Estafetteloop van AI-chats

Stel je een multi-chat pijplijn voor als een estafetteloop waarbij elke loper (chat) goed is in een specifiek onderdeel van de race:

1. **Chat 1 - De Onderzoeker**: Verzamelt informatie, feiten en achtergrond
2. **Chat 2 - De Schrijver**: Neemt deze informatie en maakt er een coherente tekst van
3. **Chat 3 - De Editor**: Controleert, verbetert en verfijnt het document

Bij elke overgang kun je het werk beoordelen, aanpassen en bijsturen voordat je het doorgeeft aan de volgende chat.

## 🏋️ De Uitdaging

1. Gebruik het [voorbeeldscenario](./voorbeelddata.md) over een beleidsnota voor multimodale vervoersknooppunten
2. Ontwerp een workflow met minimaal drie verschillende chats/stappen
3. Specificeer voor elke chat:
   - De specifieke taak
   - Het promptsjabloon
   - Het gewenste outputformaat
   - Hoe je context doorgeeft naar de volgende stap
4. Test de workflow met het voorbeeldscenario
5. Evalueer of deze aanpak betere resultaten oplevert dan één enkele chat

## 🛠️ Stap-voor-stap aanpak

1. **Definieer je eindproduct**: Wat wil je precies bereiken?
2. **Identificeer de fasen**: Welke stappen zijn nodig om daar te komen?
3. **Ontwerp gespecialiseerde prompts**: Optimaliseer elke prompt voor zijn specifieke taak
4. **Plan de overdracht**: Hoe geef je informatie door tussen de chats?
5. **Test en verfijn**: Pas elke stap aan om het beste eindresultaat te krijgen

## 📝 Template voor een 3-stappen workflow

### Chat 1: De Onderzoeker/Informatieverzamelaar
```
Je bent een onderzoeksspecialist met expertise in [onderwerp]. Ik verzamel informatie voor [eindproduct].

Ik heb specifiek het volgende nodig:
1. [Informatiesoort 1]
2. [Informatiesoort 2]
3. [Informatiesoort 3]

Presenteer de informatie in een gestructureerd formaat dat ik gemakkelijk kan gebruiken voor de volgende fase. Waar mogelijk, voeg bronverwijzingen of contextuele details toe.

Mijn onderwerp is: [specifiek onderwerp]
```

### Chat 2: De Inhoudsproducent/Schrijver
```
Je bent een schrijfspecialist met ervaring in het opstellen van [documenttype]. 

Ik heb informatie verzameld die je moet verwerken tot [eindproduct]. Hier is de verzamelde informatie:

[Plak output van Chat 1]

Schrijf op basis van deze informatie een [documenttype] met de volgende kenmerken:
- [Toon/stijl]
- [Structuur]
- [Lengte]
- [Andere vereisten]

Focus in het bijzonder op [specifieke aandachtspunten].
```

### Chat 3: De Editor/Verfijner
```
Je bent een redactie-expert gespecialiseerd in het verbeteren van [documenttype] voor [doelgroep].

Hier is een concept dat ik wil verbeteren:

[Plak output van Chat 2]

Verbeter dit document op de volgende punten:
1. [Verbeterpunt 1, bijv. taalgebruik]
2. [Verbeterpunt 2, bijv. structuur]
3. [Verbeterpunt 3, bijv. overtuigingskracht]

Behoud de originele informatie en bedoeling, maar maak het document overtuigender, duidelijker en effectiever voor de doelgroep.

Voeg waar nodig koppen, tussenkopjes of andere structuurelementen toe om de leesbaarheid te verbeteren.
```

## ✨ Tips voor succes

- Ontwerp elke chat voor een specifieke taak of expertise
- Geef duidelijke instructies over het gewenste format bij elke stap
- Neem de tijd om de output van elke chat te evalueren en aan te passen voordat je doorgaat
- Voeg context toe over wat in eerdere stappen is gebeurd
- Zorg dat de laatste chat een consistentiecheck doet op het hele document
- Experimenteer met andere rollen/specialisaties afhankelijk van je specifieke behoeften

## 📊 Evaluatie

Beoordeel je resultaten op:
- Kwaliteit: Is het eindresultaat beter dan met één chat?
- Controle: Heb je meer controle over het proces?
- Efficiëntie: Is deze aanpak tijdbesparend of juist tijdrovend?
- Toepasbaarheid: Past deze aanpak bij jouw werkprocessen?
- Verbeteringen: Welke specifieke aspecten zijn verbeterd door de multi-chat aanpak?

## 🎓 Wat je hebt geleerd

Na het voltooien van deze uitdaging heb je geleerd:
- Hoe je complexe taken kunt opdelen in gespecialiseerde stappen
- Hoe je verschillende prompting-strategieën kunt toepassen voor verschillende fasen
- Hoe je effectief context kunt doorgeven tussen chats
- Wanneer een multi-chat workflow meerwaarde biedt ten opzichte van één enkele chat
- Hoe je complexere documenten kunt creëren die meerdere expertisegebieden vereisen

## 🔍 Voorbeeld oplossing

Bekijk een [voorbeeldoplossing](./voorbeeldoplossing.md) om te zien hoe een effectieve aanpak eruit kan zien.