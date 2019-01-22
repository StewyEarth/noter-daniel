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

Definerer et **Array** ved hjælp af [ ] med navnet "people" som indeholder 4 **strings**: "Jesper", "Emil", "Oliver" og "Daniel". Elementer i et array er komma separeret.
```javascript
let people = ["Jesper","Emil","Oliver","Daniel"];
```
Sorterer arrayet alfabetisk ved hjælp af funktionen sort.
```javascript
people.sort();

//By default, the sort() function sorts values as strings.

//This works well for strings ("Apple" comes before "Banana").
```
Feverse funktionen kan brugres til at få arrayet til at være i omvendt rækkefølge.
```javascript
people.reverse();
``` 

Og så for hver person i people arrayet skriver jeg personen ud i konsollen.
```javascript
people.forEach(person => {
	console.log(person)
});
```
## Objecter
objekter bruger egenskaber f.eks.
fornavn: "Daniel" 


f.eks.
```javascript
document.innerhtml
```
ville på engelsk være lige som at sige documentet's innerhtml. document er et object. I dette tilfælde.

Man kan tilføje et egenskab ved at sige
```javascript
person.nyEgenskab = "bla bla bla";
```