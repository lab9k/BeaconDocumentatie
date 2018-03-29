---
layout: post
title:  "Informatie over de beacons algemeen"
date:   2018-02-28 12:07:27 +0200
categories: beacons
author: lotte_jespers
---
# Informatie over de beacons algemeen

Een beacon is een draadloos apparaat op batterijen dat signalen uitzend via bluetooth. Smartphones kunnen deze signalen ontvangen tot op een afstand van 70 meter.

Beacons worden vooral gebruikt bij winkels om klanten te adverteren als ze binnen de range van de beacon komen. Natuurlijk moeten klanten dan wel hun applicatie gedownload hebben en steeds hun bluetooth aan hebben staan.
De beacon wordt vooral gebruikt in de retail maar er zijn zeker ook andere toepassingen. Zo kan een beacon specifieke informatie geven bij elk kunstwerk in een museum. De beacon kan ook dienen als hotelsleutel, zo wordt de deur ontgrendeld eens je in de buurt komt. Ze worden ook gebruikt voor indoorlocalisatie en mensen te begeleiden naar de juiste weg.

Bluetooth beacons gebruiken Bluetooth low energy proximity sensing om een universeel unieke identifier (UUID) te verzenden, deze kunnen dan opgepikt worden door een compatibele applicatie of besturingssysteem. 
Het UUID, major en minor dat de beacon verstuurd kunnen gebruikt worden om de fysieke locatie van een apparaat te bepalen, mensen te volgen of locatiegebaseerde acties op een apparaat te laten uitvoeren (zoals pushmeldingen sturen)

Er zijn verschillende Beacon Protocols:
* iBeacon
* AltBeacon
* URIBeacon
* Eddystone

Apple introduceerde in 2013 de iBeacon technologie. AltBeacon is een open source alternatief voor iBeacon gecreeerd door Radius Networks.
De URIBeacon is helemaal anders dan de 2 vorige beacons. I.p.v. zijn UUID uit te zenden, zend hij een URL.
Eddystone is een Google standaard voor Bluetooth beacons. het ondersteund 3 types : Eddystone-UUID, Eddystone-URL en Eddystone-TLM.

Enkele van de waarden die men kan lezen uit het bluetooth signaal zijn: 
* UUID
* major 
* minor

Het UUID is hetzelfde voor alle beacons binnen dezelfde context. De major en minor hebben een verschillende waarde per beacon.
Het UUID bestaat uit 32 hexadecimale tekens, opgedeeld in 5 groepen. 
Major en minor hebben een waarde tussen 0 en 65535. Major waarden worden gebruikt om een groep te identificeren. vb: alle beacons op eenzelfde verdieping hebben dezelfde major.
Minor waarden worden gebruikt om het individu binnen die groep te identificeren. vb: beacons op verdiep 2 hebben allemaal een major van 2 en een unieke minor om zich te onderscheiden op het verdiep.

