---
layout: post
title:  "Webapplicatie: Bibliocation"
date:   2018-05-17 12:35:27 +0200
categories: web
author: jeremie_van_de_walle
---

# Bibliocation

Een veelvoorkomend probleem in bibliotheek de Krook is dat men vaak naar een laptop moet zoeken wanneer er van shift gewisseld wordt. Als oplossing voor dit probleem werd een webapplicatie ontwikkeld om mobiele toestellen te lokaliseren binnenin de bibliotheek. Men kan zowel laptops a.d.h.v. ESP32’s, Android toestellen en Apple toestellen terugvinden. Als backend voor dit project is Firebase gebruikt. 

##### ESP32

Aangezien de laptops in de bibliotheek nog steeds op Windows 8.1 draaien, kan er niet gebruikgemaakt worden van de “Universal Windows Platform”.  Hierdoor is het niet mogelijk om op een correcte manier de signalen van beacons te lezen. Als alternatief kan er een ESP32 aan de laptop bevestigd worden met een USB-kabel. Dit maakt het mogelijk om de signalen op een juiste manier op te vangen. 

Standaard is de programmaopslag van de ESP32 voor deze applicatie te klein. Daarom moet de partities van de ESP32 herverdeeld worden. Hoe dit kan doorgevoerd worden staat volledig omschreven op [Github](https://github.com/lab9k/Beacons/tree/master/Web/ESP32). 



