# CSS Variabler

## Oprettelse af variabler i CSS
```css
:root{
    --box-color: hsl(0,100%,50%)
}
```
--box-color er min variabel og har værdien: hsl(0,100%,50%)
___
## Brug af variabler i css
```css
.colorbox{
    background-color: var(--box-color);
}
```
Mit element med classen colorbox bruger værdien af variablen --box-color til baggrundsfarven af elementet
___
## Hentning af CSS variabler i javascript

```javascript
let rootElem = document.documentElement;
getComputedStyle(rootelem).getPropertyValue("--box-color")
```
Her tager jeg fat i mit root elementet html via 
```javascript
document.documentelement
```
Og læser variablen --box-color værdi
___
## Ændring af CSS variabler i javascript
```javascript
rootElem.style.setProperty("--box-color","red");
```
Her ændrer jeg mit rootelemets CSS variabel --box-color til at være rød via setProperty
___
