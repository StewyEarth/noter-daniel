
## funktion med parameter
```javascript
	let velkmostbesked =  velkomstMedNavn("Ady");

	console.log(velkmostbesked);

	function velkomstMedNavn(navn){
		return "Velkommen til siden " + navn;
	}
```
**definerer** en **funktion** med navnet "velkomstMedNavn" som medtager et **parameter** som hedder navn. "navn" er en scopet variabel som kun kan bruges inde i funktionen. Funktionen **retunerer** så "Velkommen til siden (navn)".
```javascript
	function velkomstMedNavn(navn){
		return "Velkommen til siden " + navn;
	}
```
Laver en variabel som gemmer det som **funktionen** "velkomstMedNavn" **retunerer** når **agumentet** "ady" bliver sendt med

```javascript
	let velkmostbesked =  velkomstMedNavn("Ady");
```
Logger "velkomstbesked" variablen til konsollen 
```javascript
	console.log(velkmostbesked);
```