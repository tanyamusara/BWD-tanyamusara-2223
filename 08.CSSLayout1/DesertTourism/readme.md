# DesertTourism

Tip: druk **Ctrl+Shift+V** in VS Code om deze tekst opgemaakt weer te geven.

Deze oefening gaat over CSS layout, zie [CSS Course > 03 CSS LAYOUT](https://rogiervdl.github.io/CSS-course/03_layout.html#/). In deze oefening gebruiken we enkel **Flexbox** en **Floating**

**Flexbox** wordt gebruikt om elementen te stapelen, bv. naast elkaar of in rijen. Je hebt in 99% van de gevallen genoeg aan deze vijf properties:
* `display: flex`: duid aan dat je de inhoud van deze parent wil layouten 
* `flex-wrap: wrap|nowrap`: moeten de children op één lijn blijven of niet (standaardwaarde: `wrap`)
* `flex-direction: row|column `: in welke richting wil je de children stapelen (standaardwaarde: `row`) 
* `justify-content: flex-start|justify-content|center|flex-end...`: uitlijning in de richting van de stapeling (standaardwaarde: `flex-start`) 
* `align-items: flex-start|center|flex-end...`: uitlijning dwars op de stapeling (standaardwaarde: `flex-start`) 

Een veel uitgebreider overzicht vind je op [https://css-tricks.com/snippets/css/a-guide-to-flexbox/](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

**Floating** wordt gebruikt om inhoud rond een blok te laten vloeien, b.v. tekst rond een afbeelding. In de meeste gevallen heb je genoeg aan één property: 
* `float: left|right` 

Laat ons deze technieken nu stap voor stap toepassen.

## A. Content maximum breedte geven en centreren 

Veel designs zijn beperkt in breedte en gecentreerd. 

1. beperk de breedte van de body op 960px met de `max-width` property 
2. centreer de body nu met `margin-left: auto` en `margin-right: auto`; daardoor zullen marges links en rechts gelijk blijven, en is de body magisch gecentreerd

## B. Afbeeldingen in breedte beperken 

Je ziet dat de afbeeldingen nu rechts hier en daar uit de body lopen, omdat ze te breed zijn. Afbeeldingen moeten altijd binnen hun parent blijven: 

3. beperk met `max-width: 100%` de breedte van afbeeldingen 

## C. Header layouten 

In de header zitten twee elementen: het logo en het menu. Die moeten naast elkaar komen, zover mogelijk uit elkaar, en verticaal in het midden gecentreerd.

4. zet logo en menu naast elkaar door in de header `display:flex` in te stellen
5. zet ze zo ver mogelijk uit elkaar met `justify-content: space-between`
6. centreer ze nu verticaal met `align-items: center`

## D. Menu layouten 

7. zet nu de menu items naast elkaar met flexbox
8. voeg wat marge toe aan de LI's om ze een beetje uit elkaar te zetten.

## E. Fotogallerij layouten 

De fotogallerij bestaat uit 8 LI's. Die moeten naast elkaar komen op twee regels. 

9. stel de breedte van de fotogallerij LI's in op iets minder dan een kwart, bv. 23%
10. zet ze nu naast elkaar zoals je met het logo en het menu in de header gedaan hebt
11. ze staan nu alle 8 op één rij; maak meerdere rijen mogelijk met `flex-wrap: wrap`

## F. Content layouten 

De content bestaat uit twee kolommen: de linkerkolom is 65% breed, de rechterkolom 30%. 

12. stel de breedtes in van de twee kolommen
13. zet ze naast elkaar, zover mogelijk uit elkaar

## G. Tekst rond afbeelding laten vloeien

In de linkerkolom staat de tekst nu onder de afbeelding. Pas dat aan:

14. gebruik `float: left` op de afbeelding om de tekst er rechts rond te laten vloeien

## H. Afwerking van de rest

Je hebt nu zowat alle basistechnieken gezien om te kunnen layouten. Werk nu de rest van de pagina af!





