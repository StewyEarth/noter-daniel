# Fetch
Henter JSON fra api

## Kodesnippet

```javascript
	fetch("data/solsystem.json")
	.then( (response) => {
		return response.json();
	})
	.then((data) => {
	console.log(data)
	});
	console.log("Hej")
```
Det overstående kode, henter json fra en fil som hedder solsystem.json og til sidst udskriver det i konsollen

Fetch kører **Asynkron** fra resten af koden så den bliver sat i gang og så kører koden videre. Så derfor vil "hej" blive udskrevet først

```javascript
	.then( (response) => {
		return response.json();
	})
	.then((data) => {
	console.log(data)
	});
```
Man skal altid skrive det som skal gøres når når dataen er loaded i den sidste then.
Den første then er et mellemled før at dataen er lavet om til json

