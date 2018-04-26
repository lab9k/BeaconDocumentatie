---
layout: post
title:  "Zones detecteren op verdieping -1"
date:   2018-04-10 16:27:27 +0200
categories: android
author: lotte_jespers
---

# Zones detecteren op verdieping -1

Dit is een testapplicatie om op een of andere manier toch localisatie te kunnen verwezenlijken op verdieping -1.
Aangezien triangulatie niet werkt doordat enkel cruciale beacons niet werken, deelde ik de ruimte op in 6 zones. Per zone ging ik na welke beacons het sterkst waren, deze beacons bepalen dus die zone.

Binnen de zones bepaalde ik welke beacons kunnen gebruikt worden om toch triangulatie te kunnen toepassen, rekening houdend met de niet werkende beacons. 

De applicatie kan binnen de 10 à 15 seconden detecteren in welke zone je staat, maar triangulatie werkt zoals verwacht niet nauwkeurig.

![BeaconsZoneScreenshot](https://i.imgur.com/AVEdrfO.png)