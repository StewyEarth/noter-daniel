# npm

ctrl + æ, for at åbne terminalen by default.
___
## start på nyt projekt
Initialiser mappen med en package fil: package.json
```
npm init -y
```

package.json indeholder information om projektet, dependencies og licens.
___
## npm install
```
npm install *navn på package* --save
npm install --save *navn på package* 
```
Installerer et node modul. --save ændrer dependencies i package.json. Kan skrive på flere måder

```
npm install --save *navn på package* *navn på en anden package*
```
Der kan installeres flere moduler på en gang

```
npm install
```
Hvis man skriver npm install, så henter den de dependencies som er skrevet inde i package.json. Hvis der ikke står nogen dependencies så henter den ikke noget

npm install kan også forkortes til:

```
npm i
```
___
## Github og aflevering
Husk ".gitignore node" på github, eller pusher den alle de mange filer i node modules

Fjern node modules når den skal afleveres via zipping
___
## Scripts (npm run)
```
npm run *navn*
```
Kører et script som er defineret i package.json f.eks.
``` 
npm run test
``` 
kører en komando i package.json som hedder "test"