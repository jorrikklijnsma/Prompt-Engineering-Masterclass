# Voorbeelddata: Feitencheck-helper Bouwen

Voor deze uitdaging ga je een AI-tool bouwen die controleert of informatie in een tekst overeenkomt met de feiten in een referentiedocument. Je krijgt twee teksten: een referentiedocument (de "grondwaarheid") en een te controleren tekst die enkele feitelijke onjuistheden bevat.

## Referentiedocument (Feitelijke informatie)

```
KLIMAATACTIEPLAN VLAANDEREN 2025-2030

Emissiereductiedoelstellingen:
- 55% reductie van broeikasgasemissies tegen 2030 (t.o.v. 1990)
- 42% van energie uit hernieuwbare bronnen tegen 2030
- 20% reductie in energieverbruik gebouwen tegen 2030 (t.o.v. 2020)

Budget en financiering:
- Totaalbudget: €4,3 miljard over 5 jaar (2025-2030)
- Klimaatfonds: €1,2 miljard
- Europese cofinanciering: €1,5 miljard
- Private investeringen: €1,6 miljard

Sectorale maatregelen:
1. Gebouwen
   - 100.000 woningrenovaties per jaar vanaf 2026
   - Verbod op nieuwe aardgasaansluitingen vanaf 2027
   - Renovatieplicht bij verkoop voor woningen met EPC-label E of F

2. Mobiliteit
   - 50% van nieuw verkochte auto's elektrisch tegen 2028
   - Uitbreiding laadinfrastructuur: 35.000 publieke laadpunten tegen 2030
   - Verdubbeling fietsgebruik voor woon-werkverkeer tegen 2030

3. Energie
   - Capaciteit zonne-energie: van 5,2 GW (2023) naar 12 GW (2030)
   - Capaciteit windenergie: van 1,5 GW (2023) naar 4,5 GW (2030)
   - Uitfasering steenkool in industrie tegen 2028
```

## Te controleren tekst (met enkele fouten)

```
Het nieuwe Klimaatactieplan Vlaanderen 2025-2030 stelt ambitieuze doelen. Vlaanderen wil 60% minder broeikasgassen uitstoten tegen 2030 vergeleken met 1990. Het plan voorziet in €5 miljard aan investeringen, waarvan het grootste deel uit het Klimaatfonds komt.

Om deze doelen te bereiken moet Vlaanderen jaarlijks 150.000 woningen renoveren en wordt een verbod op nieuwe gasaansluitingen ingevoerd vanaf 2026. Voor mobiliteit zet het plan in op elektrificatie met een doelstelling van 75% elektrische auto's in de nieuwe verkoop tegen 2028. Er komen 30.000 nieuwe laadpunten.

Op energiegebied verdrievoudigt Vlaanderen zijn zonne-energiecapaciteit van 5,2 GW naar 15 GW en wordt alle steenkoolgebruik in de industrie uitgefaseerd tegen 2028. Het plan bevat ook een renovatieplicht bij verkoop voor woningen met een slecht energielabel (D, E of F).
```

## Opzet van de uitdaging

Je opdracht is om een prompt te ontwerpen die systematisch controleert welke beweringen in de te controleren tekst wel of niet overeenkomen met het referentiedocument.

Enkele richtlijnen:
1. Je prompt moet vragen om elke feitelijke bewering in de tekst te identificeren
2. Voor elke bewering moet worden gecontroleerd of deze overeenkomt met het referentiedocument
3. Er moet een duidelijke markering komen (bijvoorbeeld correct/deels correct/incorrect)
4. Er moet toelichting zijn waarom iets correct of incorrect is
5. Waar mogelijk moeten er specifieke referenties naar het brondocument zijn

## Aandachtspunten

Let op deze specifieke fouten in de te controleren tekst:
- Emissiereductie is verkeerd (60% versus 55% in referentiedocument)
- Budget is onjuist (€5 miljard versus €4,3 miljard)
- Verdeling financiering is verkeerd voorgesteld
- Aantal te renoveren woningen is onjuist
- Jaartal voor gasverbod is verkeerd
- Percentage elektrische auto's is verkeerd
- Aantal laadpunten is afgerond/verkeerd
- Capaciteit zonne-energie doel is overschat
- Energielabel D is ten onrechte opgenomen bij renovatieplicht

De uitdaging is om een prompt te ontwerpen die deze fouten systematisch identificeert, maar ook correct aangeeft welke delen wel kloppen.