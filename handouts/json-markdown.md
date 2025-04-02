# JSON en Markdown voor Niet-Technici
## Handout voor Vlaams Parlement Masterclass

Dit document geeft een eenvoudige uitleg van Markdown en JSON, twee formats die vaak gebruikt worden bij het werken met AI. Deze handleiding is specifiek gemaakt voor medewerkers zonder technische achtergrond.

## Markdown: Eenvoudige Tekstopmaak

### Wat is Markdown?

Markdown is een eenvoudige manier om tekst op te maken zonder ingewikkelde menu's of knoppen. Het gebruikt gewone tekens om aan te geven hoe je tekst eruit moet zien. Het is ontworpen om zowel makkelijk te schrijven als te lezen, zelfs als het niet wordt omgezet naar opgemaakt formaat.

### Basis Markdown Elementen

#### 1. Koppen maken met hekjes (#)

```
# Hoofdtitel (niveau 1)
## Subtitel (niveau 2)
### Kleinere subtitel (niveau 3)
```

Hoe meer #-tekens, hoe kleiner de kop.

#### 2. Tekstopmaak

```
Normale tekst wordt gewoon getypt.

*Cursieve tekst* krijgt één sterretje aan elke kant.
_Dit is ook cursief_ met onderstreeptekens.

**Vette tekst** krijgt twee sterretjes aan elke kant.
__Dit is ook vet__ met onderstreeptekens.

***Vet en cursief*** met drie sterretjes.
```

#### 3. Lijsten maken

```
Ongenummerde lijst:
- Eerste punt
- Tweede punt
  - Subpunt (gebruik 2 spaties voor inspringen)
  - Nog een subpunt

Genummerde lijst:
1. Eerste stap
2. Tweede stap
   1. Substap (gebruik 3 spaties voor inspringen)
   2. Nog een substap
3. Derde stap
```

#### 4. Links en afbeeldingen

```
[Tekst van de link](https://www.voorbeeld.com)

![Alternatieve tekst voor een afbeelding](pad/naar/afbeelding.jpg)
```

#### 5. Citaten

```
> Dit is een citaat. Je gebruikt het > teken aan het begin van de regel.
> Je kunt meerdere regels gebruiken binnen één citaat.
```

#### 6. Horizontale lijn

```
---
```

Drie streepjes maken een horizontale scheidingslijn.

### Waarom Markdown gebruiken?

- **Eenvoudig**: Geen complexe opmaaktools nodig
- **Leesbaar**: Zelfs in platte tekst blijft het goed leesbaar
- **Universeel**: Wordt ondersteund door veel platforms en tools
- **Draagbaar**: Werkt op alle besturingssystemen
- **Toekomstbestendig**: Blijft werkt, zelfs als specifieke software verandert

### Markdown en AI

Markdown is ideaal om gestructureerde output te krijgen van AI-tools:

```
Schrijf een samenvatting in Markdown-formaat met:
# Een hoofdtitel
## Drie belangrijke punten als subtitels
Voor elk punt, maak een lijst van:
- Een korte uitleg
- Een praktisch voorbeeld
```

## JSON: Gestructureerde Data

### Wat is JSON?

JSON (JavaScript Object Notation) is een gestandaardiseerd formaat om gestructureerde informatie op te slaan en uit te wisselen. Het is ontworpen om zowel voor computers als mensen leesbaar te zijn. Denk aan JSON als een manier om informatie in een zeer georganiseerde vorm te presenteren, zoals een goed gestructureerd formulier.

### Basis JSON Elementen

#### 1. Objecten: { }

Een JSON-object wordt omsloten door accolades en bestaat uit naam/waarde-paren:

```json
{
  "naam": "Jan Janssens",
  "functie": "Beleidsadviseur",
  "afdeling": "Mobiliteit"
}
```

#### 2. Arrays (lijsten): [ ]

Een array is een geordende lijst van waarden, omsloten door vierkante haken:

```json
{
  "commissies": ["Mobiliteit", "Ruimtelijke Ordening", "Klimaat"]
}
```

#### 3. Datatypen in JSON

JSON ondersteunt verschillende soorten waarden:
- Tekst: altijd tussen dubbele aanhalingstekens `"tekst"`
- Getallen: zonder aanhalingstekens `42` of `3.14`
- Boolean: `true` of `false` (zonder aanhalingstekens)
- Null: `null` (zonder aanhalingstekens)
- Objecten: `{ ... }`
- Arrays: `[ ... ]`

#### 4. Geneste structuren

JSON kan complexe, geneste structuren bevatten:

```json
{
  "vergadering": {
    "titel": "Commissie Mobiliteit",
    "datum": "2025-04-14",
    "deelnemers": [
      {
        "naam": "Jan Janssens",
        "functie": "Voorzitter"
      },
      {
        "naam": "Petra Peeters",
        "functie": "Secretaris"
      }
    ]
  },
  "agendapunten": [
    {
      "titel": "Fietsmobiliteitsplan",
      "status": "Goedgekeurd",
      "actiepunten": [
        "Budget actualiseren",
        "Planning bijwerken"
      ]
    }
  ]
}
```

### Belangrijke regels voor JSON

1. Alle eigenschapsnamen (links van de dubbele punt) **moeten** tussen dubbele aanhalingstekens staan
2. De laatste waarde in een object of array krijgt **geen** komma
3. Tekstwaarden moeten tussen dubbele aanhalingstekens staan
4. JSON is hoofdlettergevoelig (`"Naam"` en `"naam"` zijn verschillende eigenschappen)

### Waarom JSON gebruiken?

- **Structuur**: Dwingt een consistente organisatie van informatie af
- **Validatie**: Maakt het mogelijk om te controleren of alle vereiste velden aanwezig zijn
- **Nauwkeurigheid**: Voorkomt verwarring over welke waarde bij welk veld hoort
- **Verwerkbaarheid**: Kan gemakkelijk worden verwerkt door computersystemen
- **Standaardisatie**: Universeel formaat dat door vrijwel alle systemen wordt ondersteund

### JSON en AI

JSON is uitstekend voor het structureren van AI-output:

```
Analyseer dit document en geef de resultaten in JSON-formaat:
{
  "hoofdonderwerp": "het centrale thema van het document",
  "kernpunten": ["een array van maximaal 5 belangrijke punten"],
  "betrokken_partijen": ["een array van genoemde organisaties of personen"],
  "aanbevelingen": [
    {
      "beschrijving": "beschrijving van de aanbeveling",
      "prioriteit": "hoog, middel of laag",
      "implementatie_tijd": "korte, middellange of lange termijn"
    }
  ]
}
```

Door JSON te specificeren, krijg je altijd precies de velden die je nodig hebt, in de structuur die je verwacht.

## Praktische toepassingen in het Vlaams Parlement

### Voor communicatieprofessionals

**Markdown** is ideaal voor:
- Persberichten structureren
- Nieuwsbrieven opmaken
- Social media content voorbereiden

**JSON** is handig voor:
- Communicatieplannen structureren
- Contentkalenders organiseren
- Stakeholder-informatie ordenen

### Voor juridische specialisten

**Markdown** is nuttig voor:
- Juridische notities structureren
- Samenvattingen van wetgeving
- Amendementen documenteren

**JSON** is waardevol voor:
- Gestructureerde extractie van wetteksten
- Metagegevens van juridische documenten bijhouden
- Vergelijking van wetsversies

### Voor administratieve ondersteuning

**Markdown** helpt bij:
- Vergadernotities opmaken
- To-do lijsten beheren
- Instructiedocumenten maken

**JSON** ondersteunt:
- Gestructureerde documentatie van processen
- Metagegevens van archieven
- Consistente vastlegging van beslissingen

## Voorbeelden voor AI-gebruik

### Voorbeeld 1: Vergadernotities structureren met Markdown

**Prompt aan AI:**
```
Converteer deze ruwe vergadernotities naar een goed gestructureerd Markdown-document met:
# Titel van de vergadering
## Datum, tijd en aanwezigen
## Voor elk agendapunt:
### Naam van het agendapunt
- Besproken punten
- Genomen beslissingen
- Actiepunten met verantwoordelijken

Ruwe notities:
[plak hier je ongestructureerde notities]
```

### Voorbeeld 2: Beleidsinformatie structureren met JSON

**Prompt aan AI:**
```
Analyseer dit beleidsdocument en extraheer de kerngegevens in dit JSON-formaat:
{
  "titel": "titel van het beleid",
  "ingangsdatum": "datum van ingang",
  "doelgroepen": ["lijst van beïnvloede groepen"],
  "kernmaatregelen": [
    {
      "beschrijving": "beschrijving van de maatregel",
      "budget": "gealloceerd budget indien genoemd",
      "tijdlijn": "implementatietijdlijn"
    }
  ],
  "verantwoordelijke_instanties": ["betrokken instanties"]
}

Beleidsdocument:
[plak hier je beleidsdocument]
```

## Tips voor beginners

### Voor Markdown
1. Begin eenvoudig met alleen koppen en lijsten
2. Gebruik een Markdown-preview tool zoals [StackEdit](https://stackedit.io/app#) of [Dillinger](https://dillinger.io/)
3. Maak een "spiekbriefje" met de meest gebruikte opmaak
4. Oefen door bestaande documenten om te zetten

### Voor JSON
1. Start met eenvoudige structuren en bouw van daaruit op
2. Gebruik een JSON-validator zoals [JSONLint](https://jsonlint.com/) om fouten te vinden
3. Let goed op komma's en aanhalingstekens
4. Kopieer en pas bestaande voorbeelden aan voor je eigen doeleinden

## Conclusie

Zowel Markdown als JSON zijn krachtige tools die je helpen effectiever met AI te werken. Ze vereisen geen programmeerkennis, alleen begrip van enkele eenvoudige regels en structuren. Door deze formats te gebruiken, krijg je consistentere en bruikbaardere resultaten uit je AI-interacties.