---
layout: post
title:  "Applicatie: Op ontdekking in de kinderbibliotheek"
date:   2018-04-19 15:57:00 +0200
categories: android
author: lotte_jespers
---

# Applicatie: Op ontdekking in de kinderbibliotheek

<iframe width="560" height="315" src="https://www.youtube.com/embed/OTEOj9tQghM" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

Deze applicatie werd ontwikkeld voor de kinderafdeling in de bibliotheek, De Krook. De kinderbibliotheek werd opgedeeld in 6 zones, deze zones moeten door de kinderen ontdekt worden. De applicatie detecteert door gebruik te maken van de beacons in welke zone het kind zich bevind. 

Je wordt welkom geheten en nadien heeft de applicatie jouw naam nodig, jouw score wordt bijgehouden in het scorebord. Dit scorebord wordt bijgehouden in firebase, op deze manier heeft iedereen telkens het juiste realtime scorebord. 
<img  width="200" height="150" src="https://github.com/lab9k/BeaconDocumentatie/blob/gh-pages/images/bibontdekking/hallo.png">
<img width="200" height="150" src="https://github.com/lab9k/BeaconDocumentatie/blob/gh-pages/images/bibontdekking/naam.png">

Als je het spel start krijg je eerst een rondleiding, er wordt duidelijk gemaakt welke onderdelen er zijn en waarvoor deze dienen. En dan kan het spel echt beginnen. 

<img width="200" height="150" src="https://github.com/lab9k/BeaconDocumentatie/blob/gh-pages/images/bibontdekking/snelheidwiel.png">
<img width="200" height="150" src="https://github.com/lab9k/BeaconDocumentatie/blob/gh-pages/images/bibontdekking/plattegrond.png">
<img width="200" height="150" src="https://github.com/lab9k/BeaconDocumentatie/blob/gh-pages/images/bibontdekking/vooruitgang.png">

De applicatie detecteert zo goed mogelijk zelf waar je je bevindt in de kinderbibliotheek. Eens er een zone gedetecteerd wordt, krijgt deze een zwarte rand rond zich op de plattegrond en wordt de kleur van het vooruitgangswiel aangepast door de kleur van de zone. Aan het vooruitgangswiel is ook te zien hoeveel procent van de zone al ontdekt werd. Als een zone volledig ontdekt is, krijg je een melding en wordt er een vink op deze zone geplaast. Dit wordt nog uitgebreid door vragen te stellen die over de ontdekte zone gaan, op deze manier kunnen ze nog extra punten scoren

<img width="200" height="150" src="https://github.com/lab9k/BeaconDocumentatie/blob/gh-pages/images/bibontdekking/speelscherm.png">
<img width="200" height="150" src="https://github.com/lab9k/BeaconDocumentatie/blob/gh-pages/images/bibontdekking/voltooid.png">
<img width="200" height="150" src="https://github.com/lab9k/BeaconDocumentatie/blob/gh-pages/images/bibontdekking/melding.png">

Wanneer kinderen te snel bewegen met de tablet wordt er een melding gegeven en schud het hele scherm door elkaar. Ze krijgen hiervoor ook minpunten in de percenten die ze al behaald hebben onderweg. 

<img width="200" height="150" src="https://github.com/lab9k/BeaconDocumentatie/blob/gh-pages/images/bibontdekking/snelheid.png">

Wanneer alle zones ontdekt werden, krijg je de tijd die je nodig had te zien. Ook confetti en een passend muziekje hoort erbij.

<img width="200" height="150" src="https://github.com/lab9k/BeaconDocumentatie/blob/gh-pages/images/bibontdekking/score.png">

Je kan dan ook nog kijken op welke plaats je staat binnen het scorebord. Als er ondertussen spelers bijkomen (op andere tablets) zie je die ook meteen verschijnen. 

<a target="_blank" href="https://github.com/lab9k/BibZoneOntdekken">GitHub</a><br>

