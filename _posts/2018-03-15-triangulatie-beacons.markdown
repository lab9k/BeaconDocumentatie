---
layout: post
title:  "Positiebepaling: triangulation in de Krook"
date:   2018-03-15 12:07:27 +0200
categories: beacons android
author: lotte_jespers
---
# Positiebepaling: triangulatie in de Krook

<p>Door triangulatie kunnen we met behulp van de beacons iets of iemand localiseren op een verdieping. </p>

<p>Eens we de afstand weten tot 3 beacons, kan triangulatie gebruikt worden om de x- en y-coördinaten te berekenen van dat object. Drie cirkels, met als straal de afstand tot die beacon, worden getrokken rond het midden van elke beacon. De triangulatie locatie is het zwaartepunt van de driehoek ABC, die bestaat uit de kruispunten van de drie cirkels. Dit zijn dan de x- en y-coördinaten van het object. </p>
![Triangulation](https://i.imgur.com/bekuGpUm.png )

<P>Aangezien we de plattegronden van de bibliotheek hebben, bepaalden we van elke beacon zijn positie (x- en y-coördinaat). Met behulp van <a href="https://github.com/lemmingapex/Trilateration">deze android library </a>  kunnen we dan met de coördinaten van de gedetecteerde beacons en de afstand tot die beacons, het punt bepalen waar men op dat ogenblik staat.</p>

<b>Testapplicatie: verdieping -2</b>
<p>Er werd een test applicatie geschreven voor verdieping -2 (de kleinste verdieping).
Op deze verdieping werken 13 van de 17 beacons. 
Er werd rekening gehouden met de beacons die niet werken, maar dat zijn niet zo'n cruciale beacons. Op basis van deze kennis en de kennis van de coördinaten van de beacons werden eerst enkele test berekeningen uitgevoerd. De juiste coördinaten van het rode punt werden gevonden.
</p>
![Werkende beacons -2](https://i.imgur.com/oMtTCNFm.png) ![TestBerekening](https://i.imgur.com/aVHFqbUm.png)
<p>De test met de applicatie zelf verliep ook redelijk goed. Er kan tot op 1 meter nauwkeurig bepaald worden waar je staat op verdieping -2, na een tijd van 10 tot 15 seconden. Deze test verliep goed omdat zo goed als alle nodige beacons werken. </p>

<b>Testapplicatie: verdieping -1</b>
<p>Deze test werd nu ook uitgevoerd op verdieping -1. Voor deze verdieping trachten we een app te ontwikkelen om een boek te kunnen vinden door warm-koud aanduiding, dus juiste plaatsbepaling is wel noodzakelijk.<br>
Op deze verdieping werken 30 van de 40 beacons. Er zijn wel enkele cruciale beacons die niet werken in de regio waar we deze locatiebepaling nodig hebben.<br>
De testapplicatie voor verdieping -2 werd omgevormd om te gebruiken op verdieping -1. <br>
De test verliep niet zo vlot als op de andere verdieping. De signalen van de beacons zijn niet juist genoeg op vlak van afstand tot het toestel, hierdoor zijn de waarden niet correct en kan er dus ook geen correcte coördinaat berekend worden. De berekende coördinaat kwam bijna nooit overeen met het punt waar het toestel zich bevond.
</p>
![TestBerekening](https://i.imgur.com/71IpjqFl.png)
