---
title: Breville Dual Boiler 00–12: de tweecijferige codes
description: De Breville Dual Boiler BES920 meldt codes 00 t/m 12 in een verborgen zelftestmenu: wat elk blok betekent, stoom- versus zetkant en de oplossingen.
---

De meeste espressomachines van Breville kondigen hun fouten aan op het gewone display: de Barista Touch met ER-codes, de Oracle met 'Error'-codes, de Oracle Jet met E-nummers. De **Dual Boiler BES920** doet dat anders. Zijn fouttabel bestaat uit kale tweecijferige codes, **00 tot en met 12**, en die staan niet op het alledaagse scherm maar in een verborgen zelftestmenu. Door alleen naar het voorpaneel te kijken op een normale dag ziet u ze niet — u moet de knoppencombinatie kennen.

De nummering is het begrijpen waard, want het is een opgeruimde tabel: het blok waarin een code valt, vertelt wat voor soort storing het is, en binnen elk blok noemt de code het onderdeel dat over de klacht gaat.

## Het foutenlog lezen

U bereikt het logboek via het zelftestmenu:

1. Schakel de machine volledig uit (wandschakelaar of stekker).
2. Houd **EXIT** en **MANUAL** ingedrukt terwijl u de stroom terugzet; het zelftestmenu verschijnt.
3. Druk op **MENU** tot u bij item 3 bent, het foutenlog. Item 4 toont de vulstand van de boiler, weergegeven als LLL (laag) of HHH (hoog).
4. Blader in het foutenlog met **MENU** door de codes 00 tot en met 12; bij elke code hoort een opgeslagen tellerstand.
5. Bij 'ErSt' houdt u **MANUAL** ingedrukt tot de machine piept om de opgeslagen codes te wissen; de kopjesteller wordt niet gereset.

De tellers zijn minstens zo belangrijk als de codes zelf. Een storing met een tellerstand van één van een jaar geleden is geschiedenis; een storing waarvan de teller elke week oploopt, is een levend probleem dat zich opbouwt.

## Wat de 00-familie dekt

De codes **00 tot en met 05** vormen het temperatuursensorblok, gerangschikt als drie paren. Binnen elk paar betekent het lagere nummer dat de sensor **niet wordt gedetecteerd** — de print leest een open circuit — en het hogere nummer dat de sensor als **kortsluiting** wordt uitgelezen:

- **00 en 01** — temperatuursensor van de stoomboiler, eerst niet gedetecteerd, dan kort.
- **02 en 03** — temperatuursensor van de koffieboiler, eerst niet gedetecteerd, dan kort.
- **04 en 05** — temperatuursensor van de verwarmde zetgroep, eerst niet gedetecteerd, dan kort.

De BES920 heeft twee roestvrijstalen boilers plus een verwarmde zetgroep, en deze drie sensoren bewaken precies die drie verwarmde zones. De [code 00-pagina](https://nl.codefixcoffee.com/breville/dual-boiler-bes920/00/) behandelt de sensor van de stoomboiler, maar het praktische advies geldt voor alle zes: controleer en hersteek de sensorplug voordat u onderdelen bestelt, en zoek naar vocht — water over een connector wordt gelezen als open circuit of als kortsluiting, afhankelijk van hoe het precies zit. Originele NTC-sensorsets lopen uiteen van ongeveer €25 tot €90 afhankelijk van welke van de drie het betreft; o-ringsets kosten €10 tot €20 en zijn vaak al de echte boosdoener.

## Stoomkant versus zetkant

De rest van de tabel volgt dezelfde scheidslijn als de sensorparen:

- **Stoomboiler:** 06 (pompprobleem tijdens het opstarten), 07 (waterstand of pompstoring) en 11 (oververhitting gedetecteerd).
- **Koffieboiler, de zetkant:** 08 (pomp- of doorstroomprobleem), 09 (waterstandstoring) en 10 (oververhitting gedetecteerd).
- **Zetgroep:** 12 (oververhitting gedetecteerd).

### Codes die samengaan

Deze storingen grijpen in elkaar, en daarom zegt het hele log meer dan één code op zich. Code 08 betekent dat de pomp draaide terwijl de doorstroommeter niets zag — meestal kalk op het schoepenrad van de flowmeter, of een kleine pomp die zoemt zonder water te verplaatsen; in beide gevallen is ontkalken de eerste zet. Code 11, overtemperatuur van de stoomboiler, volgt vrijwel altijd op een boiler die niet wordt bijgevuld — kijk of 07 of 08 ook een tellerstand heeft — want het verwarmingselement blijft een lege boiler verwarmen; een lekkende afdichting rond de peiler is de andere oorzaak. Bestel dus niets voordat u item 4 in het zelftestmenu hebt gelezen: een vulstand die niet past bij wat u hoort tijdens het vullen, vertelt aan welke kant de storing werkelijk zit.

Code 12, oververhitting van de zetgroep, is het zeldzame uiteinde van de tabel — en de code waarbij herhaling het zwaarst weegt: een oververhitting die steeds terugkomt, wijst op een print die het verwarmingselement vast 'aan' zet in plaats van op een sensor die afglijdt. De [code 12-pagina](https://nl.codefixcoffee.com/breville/dual-boiler-bes920/12/) werkt dat verder uit.

### Praktisch voor Nederland

In Nederland en de rest van Europa wordt dit merk verkocht als Sage; de BES920 heet hier de Sage Dual Boiler en is technisch hetzelfde toestel, dus de codes en het zelftestmenu werken identiek. Handleidingen en ondersteuning staan op [de supportsite van Sage Appliances](https://www.sageappliances.co.uk). Koopt u een tweedehands exemplaar dat uit het Verenigd Koninkrijk komt, let dan op de Britse type G-stekker: die hoort niet rechtstreeks in een Nederlands stopcontact — gebruik een geaarde adapter of laat de stekker vervangen.

## Wat de onderdelen kosten

- Ontkalker voor de doorstroom- en waterstandscodes: ongeveer €10, en het lost een aanzienlijk deel ervan echt op.
- Vulpomp: €30 tot €60.
- Peiler van de stoomboiler met o-ringset: ongeveer €85; losse o-ringsets €10 tot €20.
- Thermische zekering: €10 tot €20 — maar zoek eerst uit waarom hij is doorgeblazen.
- Triac of voedingsprint: €80 tot €150.

Een reparatie bij Breville zelf buiten garantie kost voor interne storingen doorgaans €300 tot €500 en meer, dus een pomp of sensor is het waard om zelf te doen; bij een print op een ouder apparaat vraagt u eerst een offerte. Water en netspanning delen de bovenkant van de boiler, dus trek altijd de stekker voordat u aan peilers zit.

Voor de formulering van de codes bij de andere machines uit het gamma, zie de [Breville-sectie](https://nl.codefixcoffee.com/breville/) — de ER-machines delen diagnostische ideeën, maar niet de nummering. In het Verenigd Koninkrijk loopt het merk onder de naam Sage; Engelstalige lezers kunnen terecht op de [UK-editie](https://nl.codefixcoffee.com/uk/) van deze site.
