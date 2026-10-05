---
title: Breville/Sage Oracle stoom en ER-codes: wat u eerst controleert
description: Stoomstoringen op de Oracle: wat de stoomzijde-codes betekenen, welke purge u eerst draait en wanneer kalk de echte oorzaak is.
---

De stoomzijde van een Breville Oracle is het drukste plekje van de machine: een roestvrijstalen stoomboiler, een stoompijp die melk automatisch textuurt, niveauprobes en een vulpomp, alles dagelijks op temperatuur. Logisch dat daar ook een flink deel van de foutcodes vandaan komt. De Oracle-familie hanteert een servicetabel van 32 entries die Breville niet publiceert, en in Europa — Nederland incluis — draagt hetzelfde toestel het **Sage**-logo met identieke codes. Voordat u op een kapot onderdeel gokt: neem eerst de goedkope controles door, want de meeste stoomstilstanden worden veroorzaakt door een verstopte stoomtip, een nagelaten purge of kalk op een probe. Het dagelijkse onderhoud van de stoompijp beschrijft de fabrikant zelf in [de supportsectie van Sage Appliances](https://www.sageappliances.co.uk).

## Waar de stoomcodes in de Oracletabel zitten

De Oracle (BES980) en de Oracle Touch (BES990) delen één tabel; de BES980 toont de entries als "Error 1" tot "Error 32", de BES990 geeft ze een ER-voorvoegsel. De stoomgerelateerde entries clusteren op vijf plekken:

- **Error 1 tot 4** — de temperatuursensor van de stoomboiler, in de cyclus open circuit bij opstarten, signaal weg tijdens bedrijf, en kortsluiting in beide situaties. Eén sensor, vier manieren van melden.
- **Error 13 tot 16** — hetzelfde kwartet voor de temperatuursensor van de stoompijp zelf: de probe die het automatisch textureren stopt zodra de melk de juiste temperatuur bereikt. Die zit op de natste plek van de machine.
- **Error 18** — de stoomboiler komt niet normaal op temperatuur.
- **Error 20 en 21** — waterniveau- of vulpompproblemen van de stoomboiler, en een niveauprobe die iets anders rapporteert dan het bord verwacht.
- **Error 26** — de stoomboiler liep boven de doeltemperatuur door; **Error 32** is een stoomboilerlek of een mislukte navulling.

Niet alles vlak bij de stoompijp is stoomzijde: codes 5 tot 8 horen bij de sensor van de koffieboiler, met [Error 8](https://nl.codefixcoffee.com/breville/oracle-bes980/error-8/) als de kortsluiting-tijdens-bedrijf-entry. Het opgeslagen logboek helpt de families uit elkaar te halen — op de BES980 opent u Error Storage door met de machine uit 1 CUP, 2 CUP en POWER samen in te drukken, waarna u door alle 32 codes met hun tellingen bladert.

## Wat u eerst doet: de purge-routine

Zwakke of spetterende stoom, of een code vlak na een melkdrank, wijst eerder naar de stoomtip dan naar de boiler:

1. Trek de stekker eruit en laat de stoompijp afkoelen.
2. Schroef de tip los en laat hem weken in heet water met een scheut ontkalker; prik elk gaatje vrij met de pin op het reinigingsgereedschap.
3. Draai de purge: zo'n tien seconden stoom in de drupbak met de tip eraf, daarna nogmaals met de tip erop.
4. Purge de pijp vanaf nu na elke melksessie; opgedroogde melk in de tip is de aanstichter van de meeste van deze stilstanden.

Meet de machine de stoomdruk, zoals de Oracle Jet met zijn E16-code, dan kan een dichtgeslibde tip een code laten aanslaan nog voordat u merkt dat de stoomkracht afneemt.

### Waterhardheid meenemen

De hardheid van Nederlands leidingwater verschilt flink per regio: vrij zacht in de duingebieden, aanzienlijk harder in Zuid-Limburg en delen van Brabant. Stel de waterhardheidsinstelling van uw Oracle in op de lokale waarde — uw waterbedrijf publiceert die per woongebied — zodat de ontkalkherinnering realistisch blijft. In een hardwatergebied met zelden een ontkalkbeurt legt u zelf de basis voor Error 20, 21 of 32.

## Hardheid, kalk en de niveauprobes

Waar het water hard is, schrijft kalk zijn eigen foutcodes. De niveauprobes van de stoomboiler staan permanent in heet water, en een kalklaag isoleert ze, zodat het bord "geen water" concludeert terwijl de boiler vol zit — de klassieke route naar Error 20 of 21 en naar de navulfout van Error 32. Kalk hoopt ook op in het stoompad en op de inlaat van de vulpomp. Een volledige ontkalking, inclusief de stoomboilercyclus, is de goedkoopste diagnostiek die u kunt draaien en ruimt opvallend veel van deze codes in één keer op.

Het naaste familielid maakt hetzelfde punt: de Dual Boiler verbergt zijn codes 00 tot 12 in een zelftestmenu, en [code 00](https://nl.codefixcoffee.com/breville/dual-boiler-bes920/00/) — stoomboilersensor niet gedetecteerd — staat bovenaan een tabel waarvan de niveau- en vul-entries onder hard water precies hetzelfde gedrag vertonen.

## Wanneer ontkalken volstaat en wanneer niet

Eerst ontkalken, dan pas demonteren — maar ken de grens:

- **Ontkalk eerst** bij vul-, niveau- en navulcodes (20, 21, 32), bij zwakke stoom zonder code en bij elke machine waarvan de laatste beurt meer dan drie maanden geleden was. Kosten: één fles ontkalker.
- **Ontkalken lost het niet op** wanneer een sensorcode op een vers ontkalkte, warme machine direct terugkeert — of het nu een stoomboiler-entry uit 1 tot 4 betreft of [Error 8](https://nl.codefixcoffee.com/breville/oracle-bes980/error-8/) aan de koffiezijde. Een code die een ontkalking overleeft, wijst naar de sensor, de kabel of een connector.
- **Stop en controleer de afdichtingen** als Error 26 terugkeert: een lekkende o-ring rond de stoomprobe laat stoom de sensorkabel opwarmen en bootst een ontsporende boiler na. Nieuwe probe-o-rings zijn spotgoedkoop; een triac-bord dat de verwarming niet meer kan uitschakelen is dat niet.
- **Error 18** op een machine die helemaal geen stoom meer maakt is doorgaans verwarmingszijde — thermische zekering, element of bord — en geen kalk, dus behandel hem als reparatie in plaats van schoonmaakklus.

## Wat de onderdelen kosten

Originele temperatuursensorassemblages lopen van circa €25 tot €95 afhankelijk van de sensor; complete stoompijpassemblages, sensor inbegrepen, kosten rond €60 tot €95; een probe- met o-ringset zo'n €85 en een vulpomp €30 tot €60. Fabrieksquotes buiten de garantie zitten doorgaans tussen €300 en €500 voor interne storingen, waardoor de volgorde "eerst een fles ontkalker, daarna eventueel een sensorreparatie" vrijwel altijd de betere rekenkunst is. De Sage-variant van deze tabellen vindt u op de [UK-editie van de site](https://nl.codefixcoffee.com/uk/).
