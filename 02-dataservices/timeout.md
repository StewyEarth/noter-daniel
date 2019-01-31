# timeout

Timeouts kan bruges til at få noget til at vente med at køre. 

## Snippet
```javascript
	let timersDone = 0;
	setTimeout(()=>{
		console.log("#1");
		checktimer();
	},1500);

	setTimeout(()=>{
		console.log("#2");
		checktimer();
	},3000);

	setTimeout(()=>{
		console.log("#3");
		checktimer();
	},2000);

	function checktimer(){
	timersDone++
		if (timersDone == 3){
			console.log("Timers done")
		}
	}
```
### Timeouts 
Den første timer venter 1.5 sekunder (1500 milisekunder) på at console logger "#1" så kalder den funktionen "checktimer". 

### Funktionen
Checktimer tilføjer en til timersDone variablen og checker så om timersDone er 3. Så hvis alle 3 timere har kørt, og har tilføjet 1 til timersDone. Så er if statementet timersDone true, og så console logger den "Timers Done"

Det er en rigtig god måde at være sikre på at f.eks. alle fetches er done, ved at tilføje 1 til en variabel med et navn som: fetchesDone.