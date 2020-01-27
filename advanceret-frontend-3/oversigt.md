[Date time modul](https://github.com/rts-cmk/the-awesome-newspage/blob/master/date-and-time.md)


___



# Notes


NodeJS + ExpressJS (Server)

Routes: 

* interface til server, handlinger vi kan få serveren til at udføre. Samt sende 

* res.send() giver et svar tilbage til browser/Client.

* req
    * params (Url parameter)
    * eksempel 
        * Hvad man skriver efter params er bestemt af vores route. F.eks
        * app.get("/articles/:articleid")
        * så ville vi skrive req.params.articleid for at få fat i værdien af articleid


View Engines (Ejs)

* Render: res.render("home") Viser en ejs fil som hedder home. Kan også bruges til at sende data med. f.eks.
     res.render("home",{
         title: "Hjem"
     })
     
    * Partials (f.eks Nav) Undgår gentagende kode.

    req.params

    * Server tags 
        * <% %> bruges til at lave javascript
        * <%= %> bruges til at udskrive værdien af en variabel
        * <%- %> Tager den den får at face value. altså den kan se html som at være html og derved sætte det ind på siden som html.
        * God vane: Check om variablen eksisterer f.eks
        <% if(typeof articles != "undefined"){ %>

MySQL (DB)
* SQL (Sproget)
    * Exempel: "SELECT * FROM articles"

BodyParser (Modul)
* req.body.(name attribute værdien)
    * f.eks req.body.email 


Når vi er i gang med at udskrive f.eks artikler fra vores database så er det kolonnernes navn som bestemmer hvad vi kan skrive efter punktummet. f.eks

articles.forEach(article =>{

<%= article.(kolonne navn)%>

})