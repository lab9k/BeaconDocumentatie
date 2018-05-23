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


##### iOS

Naast ESP32’s kunnen ook Apple toestellen getraceerd worden in de bibliotheek. De gebruiker van het toestel heeft zelf de vrijheid om te kiezen hoelang hij gevolgd wil worden. De keuzes zijn ‘1uur’, ‘3uur’ en ‘zolang aanwezig’. De app stopt automatisch met het volgen van de locatie na één of drie uur. Wanneer ‘zolang aanwezig’ is geselecteerd en er wordt geen enkele beacon meer gedetecteerd dan kan ervan uit gegaan worden dat het toestel zich niet meer in de bibliotheek bevindt. Wordt er binnen de 30 seconden geen enkele beacon meer gevonden dan stopt de applicatie met de locatie te traceren. Als de applicatie is gestopt dan wordt het toestel automatisch verwijderd uit de lijst in de webapplicatie.  Op [Github](https://github.com/lab9k/Beacons/tree/master/Web/iOS) staat beschreven hoe het iOS project gebruikt kan worden met een firebase project. 


