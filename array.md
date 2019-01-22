# Arrays
Serie af data.

Gøre noget for hver element.

Usikker på mængde men hvis der skal gøres noget for alt.

Tomt array
```javascript
var arraynavn = [];
```
Starter i 0 istedet for 1.


## Eksempel
```javascript
let people = ["Jesper","Emil","Oliver","Daniel"];

people.sort();

people.forEach(person => {
	console.log(person)
});
```

Definerer et **Array** med navnet "people" som indeholder 4 **strings**: "Jesper", "Emil", "Oliver", "Daniel"
```javascript
let people = ["Jesper","Emil","Oliver","Daniel"];
```
Sorterer arrayet alfabetisk ved hjælp af 
```javascript
people.sort();
```

Og så for hver person i people arrayet skriver jeg personen ud i konsollen.
```javascript
people.forEach(person => {
	console.log(person)
});
```