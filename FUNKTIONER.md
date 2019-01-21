
## funktion med parameter
### Kodesnippet
```javascript
var velkomstbesked = "";

velkmostbesked =  velkomstMedNavn("Ady");
console.log(velkmostbesked);

velkmostbesked =  velkomstMedNavn("Daniel");
console.log(velkmostbesked);

function velkomstMedNavn(navn){
	return "Velkommen til siden " + navn;
}
```

### Gennemgang
**Definerer** en **funktion** med navnet "velkomstMedNavn" som medtager et **parameter** som hedder navn. "navn" er en scopet variabel som kun kan bruges inde i funktionen. Funktionen **retunerer** så "Velkommen til siden (navn)".
```javascript
function velkomstMedNavn(navn){
	return "Velkommen til siden " + navn;
}
```

Laver en **variabel** "velkomstbesked" som er en tom **string**. For at gøre den klar til at blive overskrevet. så overskriver jeg "velkomstbesked" med det som **funktionen** "velkomstMedNavn" **retunerer** når **agumentet** "Ady" eller "Daniel" bliver sendt med.
```javascript
var velkomstbesked = "";
velkmostbesked =  velkomstMedNavn("Ady");
velkmostbesked =  velkomstMedNavn("Daniel");
```

Logger "velkomstbesked" variablen til konsollen 
```javascript
console.log(velkmostbesked);
```