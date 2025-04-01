# Uitdaging 3: Vergadernotities Structureren
## Deel 1: Rolspecifieke Prompt Engineering

## 🎯 Doel van deze uitdaging

Leer hoe je ongestructureerde vergadernotities kunt omzetten naar een overzichtelijk, bruikbaar format met behulp van template-based prompting.

## 📋 Wat is template-based prompting?

Template-based prompting is een techniek waarbij je de AI vraagt om informatie in een specifiek format te structureren, zoals een formulier of een tabel, zodat de output direct bruikbaar is.

### Waarom is dit nuttig voor administratieve ondersteuning?

Als administratief medewerker bij het Vlaams Parlement:
- Verwerk je vaak handgeschreven of chaotische vergadernotities
- Moet je actiepunten en beslissingen duidelijk kunnen identificeren
- Moet je informatie gestructureerd delen met verschillende betrokkenen
- Besteed je veel tijd aan het herformatteren van notities

Deze techniek helpt je om snel ongestructureerde notities om te zetten naar een professioneel, gestandaardiseerd format dat direct bruikbaar is voor alle betrokkenen.

## 📚 Hoe werkt het?

**Zonder template:** "Maak deze notities overzichtelijker"  
*Resultaat:* Een verbeterde maar mogelijk inconsistente opmaak

**Met template:** "Gebruik dit specifieke format: [template met koppen, subkoppen, etc.]"  
*Resultaat:* Een consistent, gestandaardiseerd document dat direct bruikbaar is

## 🏋️ De Uitdaging

1. Gebruik de [ongestructureerde vergadernotities](./voorbeelddata.md) van de Commissie Mobiliteit
2. Identificeer welke elementen je wilt extraheren (agendapunten, besluiten, actiepunten, etc.)
3. Ontwerp een prompt die een consistent format produceert voor deze notities
4. Test met de voorbeeldnotities en beoordeel de bruikbaarheid

## 🛠️ Stap-voor-stap aanpak

1. **Analyseer de notities**: Welke informatie moet behouden blijven?
2. **Definieer je format**: Welke structuur is het nuttigst voor jouw doel?
3. **Ontwerp je prompt**: Geef duidelijke instructies over het gewenste format
4. **Voeg specificaties toe**: Wat moet er gebeuren met ontbrekende informatie?
5. **Test en verfijn**: Controleer of het resultaat aan je verwachtingen voldoet

## 📝 Template om mee te beginnen

```
Je bent een administratief medewerker van het Vlaams Parlement.
Converteer deze ongestructureerde vergadernotities naar een gestructureerd format.

Gebruik dit overzichtelijke format:

VERGADERING: [titel]
DATUM: [datum]
DEELNEMERS: [lijst van namen]

AGENDAPUNTEN:

1. ONDERWERP: [eerste agendapunt]
   - Besproken punten:
     * [punt 1]
     * [punt 2]
   - Beslissingen:
     * [beslissing 1]
     * [beslissing 2]
   - Actiepunten:
     * [persoon 1] zal [actie] doen voor [deadline]
     * [persoon 2] zal [actie] doen voor [deadline]

2. ONDERWERP: [tweede agendapunt]
   [...]

VOLGENDE VERGADERING:
DATUM: [datum]
LOCATIE: [locatie]
VOORLOPIGE AGENDA:
- [agendapunt 1]
- [agendapunt 2]

BELANGRIJK: Zorg ervoor dat alle actiepunten een verantwoordelijke en deadline hebben.
Als deze informatie ontbreekt in de notities, schrijf dan "Verantwoordelijke: Niet gespecificeerd" of "Deadline: Niet gespecificeerd".

VERGADERNOTITIES:
[Plak hier de ongestructureerde notities]
```

## ✨ Tips voor succes

- Wees specifiek over de structuur die je wilt (koppen, subkoppen, etc.)
- Geef duidelijke instructies over hoe om te gaan met ontbrekende informatie
- Vraag om actiepunten duidelijk te markeren met verantwoordelijke personen
- Overweeg of je bepaalde onderdelen wilt benadrukken of prioriteren
- Denk aan de eindgebruiker: wat maakt het document bruikbaar voor hen?

## 📊 Evaluatie

Beoordeel je resultaten op:
- Compleetheid: Is alle belangrijke informatie behouden?
- Structuur: Is het format consistent en overzichtelijk?
- Bruikbaarheid: Zijn actiepunten en beslissingen makkelijk te identificeren?
- Professionaliteit: Is het resultaat direct deelbaar met betrokkenen?
- Tijdsbesparing: Hoeveel tijd bespaar je met deze aanpak?

## 🎓 Wat je hebt geleerd

Na het voltooien van deze uitdaging heb je geleerd:
- Hoe je template-based prompting gebruikt voor administratieve taken
- Hoe je notities consistent en professioneel kunt structureren
- Hoe je essentiële informatie uit ongestructureerde tekst kunt extraheren
- Hoe je tijd kunt besparen bij het verwerken van vergadernotities

## 🔍 Voorbeeld oplossing

Bekijk een [voorbeeldoplossing](./voorbeeldoplossing.md) om te zien hoe een effectieve aanpak eruit kan zien.