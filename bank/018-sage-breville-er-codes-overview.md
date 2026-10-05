---
title: Sage/Breville ER-codes: de verborgen servicetabel lezen
description: Sage/Breville-machines tonen ER-codes uit een nooit gepubliceerde servicetabel. Zo zijn ER01-ER18 opgebouwd en waarom de Oracle anders nummert.
---

Stopt een Breville-espressomachine en verschijnt ER05 op het paneel, dan vindt u in de handleiding geen betekenis terug. Dat is geen omissie: de foutcodes komen uit interne servicetabellen die het bedrijf voor reparaties hanteert en voor eigenaren achterhoudt. In Europa — dus ook in Nederland — loopt dezelfde hardware onder de naam **Sage** over de toonbank: identieke machines, alleen het logo op de badge verschilt, en een ER-code op een Sage Barista Touch betekent exact wat hij op een Breville betekent. Ons [Breville/Sage-overzicht](https://nl.codefixcoffee.com/breville/) volgt het huidige gamma; dit bericht verklaart hoe de nummering is georganiseerd, zodat ook een code die u nog nooit zag iets zinnigs vertelt.

## Waarom Breville de codes niet publiceert

De gebruikershandleiding behandelt reinigen en ontkalken, geen diagnostiek. De volledige codetabellen schuilen in de servicemodus van elke machine: met een wachtwoord afgeschermde schermen voor technici, met opgeslagen fouttellers en live sensoruitlezingen. Juist omdat de codes reparatie-instrumentarium zijn en geen consumentenfunctie, bestaat er geen openbaar document — de meeste eigenaren zien dan ook alleen de ene code die een stilligging veroorzaakte. Het contrast met Miele is schril: daar staan de F-codebetekenissen gewoon in de gebruiksaanwijzing, en daarom kunnen de [Miele-codepagina's](https://nl.codefixcoffee.com/miele/) de handleiding letterlijk citeren.

## De Barista Touch-tabel: ER01 tot en met ER18

De Barista Touch (BES880) en de Barista Touch Impress (BES881) delen een besturingsplaatfamilie én codetabel, met achttien entries. Eenmaal doorzien leest de tabel zich vanzelf: de sensorcodes komen in **groepen van vier**, per sensor één groep, doorlopend open circuit bij het opstarten, open circuit tijdens bedrijf, kortsluiting bij het opstarten en kortsluiting tijdens bedrijf.

- **ER01 tot ER04** — de temperatuursensor van het ThermoJet-thermoblok in zijn vier open- en kortvarianten. [ER01](https://nl.codefixcoffee.com/breville/barista-touch-bes880/er01/) is de entry voor open circuit bij het opstarten.
- **ER05 tot ER08** — de temperatuursensor van de melkkan, de kleine probe in het gebied van de drupbak die de kan uitleest terwijl de stoompijp de melk textuurt. ER05, open circuit bij opstarten, is de vaakst gemelde Barista Touch-code, en alle vier de entries delen één oplossing.
- **ER09 tot ER12** — de temperatuursensor in de zetwaterlijn (inline), volgens hetzelfde viervoudige patroon.
- **ER13 en ER14** — telproblemen van de flowmeter, bij het opstarten en tijdens bedrijf: de pomp draaide, maar de machine kon het passerende water niet tellen.
- **ER15** — een communicatiestoring tussen interne elektronische modules; regelmatig een losgeschoten flatcable of vochtige connector in plaats van een dood bord.
- **ER16 en ER17** — de maalmolen: eerst oververhitte de motor en schakelde zichzelf beveiligend uit, daarna tijdde de motor uit zonder de klus af te maken.
- **ER18** — de E-fast-beveiliging, een elektrische of veiligheidsstoring zoals lekstroom; dit is tevens de code die de aardlekschakelaar in uw meterkast kan laten uitslaan.

## De Oracle-familie hanteert een langere tabel

Kiest u een Oracle, dan krijgt hetzelfde idee meer entries mee. De Oracle (BES980) en de Oracle Touch (BES990) delen een lijst van 32, waarbij de BES980 ze als "Error 1" tot "Error 32" toont en de BES990 het voorvoegsel ER gebruikt. De eerste zestien volgen het kwartetprincipe over vier sensors: stoomboilercodes 1 tot 4, koffieboilercodes 5 tot 8 — met [Error 8](https://nl.codefixcoffee.com/breville/oracle-bes980/error-8/) als de kortsluiting van de koffieboilersensor tijdens bedrijf — de verwarmde zetgroep op 9 tot 12, en de stoompijp op 13 tot 16. De rest betreft boilers die niet op temperatuur komen (17 tot 19), niveau- en vulstoringen van de stoomboiler (20 en 21), flowmeterproblemen (22 en 23), niveauprobes en oververhitting (24 tot 27), een communicatiestoring op het bord bij 28, de maalmolen bij 29 en 30, de tampermotor bij 31 en een lekkende dan wel niet bijvullende stoomboiler bij 32.

Twee kleinere tabellen ronden de familie af. De Oracle Jet (BES985) gebruikt een eigen, kortere tabel van E1 tot E19, en de Dual Boiler (BES920) houdt tweecijferige codes 00 tot 12 verborgen in een zelftestmenu in plaats van op het gewone display — een Dual Boiler kan dus op een storing staan die u op het scherm nooit zag.

## Het verborgen foutenlogboek zelf uitlezen

Omdat het servicedata is, leest u de geschiedenis van uw machine via dezelfde serviceschermen. De routes zijn technisch gekleurd maar goed gedocumenteerd onder reparateurs:

- **Barista Touch en Oracle Touch** — schakel aan de muur uit, houd de Power-knop vooraan ingedrukt terwijl u de muurschakelaar terugzet, laat los bij het logo, toets het servicewachtwoord 00000 en open vervolgens Error Counter voor opgeslagen fouten of Live Debug voor actuele temperaturen en waterniveaus.
- **Barista Touch Impress** — zelfde knoppenserie, maar het wachtwoord luidt 02015.
- **Oracle BES980** — houd met de machine ingestoken maar uitgeschakeld 1 CUP, 2 CUP en POWER minstens een seconde tegelijk in; na de lange piep opent de SELECT-dial Error Storage, waarmee u door errors 1 tot 32 met hun opgeslagen aantallen bladert.

Beschouw deze schermen als alleen-lezen: noteer wat er staat, laat instellingen onaangeroerd en wis het logboek pas ná een reparatie, zodat een terugkeerende code zichtbaar blijft.

### Sage in Nederland: aankoop, garantie en support

In Nederland wordt dit merk officieel als Sage verkocht, met eigen handleidingen en support via [de officiële site van Sage Appliances](https://www.sageappliances.co.uk). Wie binnen Europa koopt, heeft daarnaast twee jaar wettelijke garantie op gebreken die er bij aflevering al waren — bewaar de aankoopbon dus zorgvuldig. Bij een ER-code binnen die termijn zijn de verkoper en de Sage-support uw eerste aanspreekpunt, niet uw eigen schroevendraaier.

## Wat de reparaties doorgaans kosten

Zelfs tegenover een ongepubliceerde tabel blijft de rekenkunde voorspelbaar. Temperatuursensorassemblages lopen van circa €25 tot €95, afhankelijk van de sensor in kwestie (stoompijp- en melksensoren zijn de prijzige), o-ringsets kosten €10 tot €20 en een reparatiekit voor de melksensor zo'n €30 tot €50 tegenover €80 tot €95 voor de originele assemblage. Fabrieksquotes buiten de garantie voor interne storingen liggen vaak tussen €300 en €500, dus een sensorreparatie via een onafhankelijke reparateur is doorgaans de betere route. De Britse Sage-dekking van dezelfde tabellen staat op de [UK-editie van de site](https://nl.codefixcoffee.com/uk/).
