# Server i guess

• Skriv hvad *res.render()* metoden gør.
Den inlæser filen som man siger den skal?
• Skriv hvad metoden kræver som *parameter/argument*.
En string som er navnet på filen man vil inlæse

```
<%- include("partials/styles.ejs") %>
```
bruges til at hente noget partial

hvis den siger cannot get så kan det nok ikke finde den route man snakker om

henter en variabel og chekcer om den er undefined
```
<%= typeof product.picture != "undefined" ? product.picture : "/img/products/placeholder.jpg" %>
```


