# Kodtest

Uppgiften består i att skapa en webapp som visar en text hämtad från ett API.
Webappen ska visa en knapp som man klickar på för att generera en text.
Följande komponenter ska finnas i appen:

 - JS klient
 - Server API
 - Externt API

Externt API är valfritt - det står dig fritt att välja vilken typ av app du vill bygga.
Exempel på API kan vara:

 - [complimentr][1]
 - [evilinsult][2]
 - [zenquotes][3]


Diagram över hur appen ska fungera:

```
+-------+                +---------+             +---------+                      +-----+
| User  |                | Browser |             | Server  |                      | API |
+-------+                +---------+             +---------+                      +-----+
    |                         |                       |                              |
    | Clicks button           |                       |                              |
    |------------------------>|                       |                              |
    |                         |                       |                              |
    |                         | Makes JS request      |                              |
    |                         |---------------------->|                              |
    |                         |                       |                              |
    |                         |                       | Makes server side request    |
    |                         |                       |----------------------------->|
    |                         |                       |                              |
    |                         |                       |             Returns response |
    |                         |                       |<-----------------------------|
    |                         |                       |                              |
    |                         |      Returns response |                              |
    |                         |<----------------------|                              |
    |                         |                       |                              |
    |      Displays some text |                       |                              |
    |<------------------------|                       |                              |
    |                         |                       |                              |
```

Exempel på implementation - **Pep talk** - som hämtar data från [complimentr][1]:

![Pep talk](https://peptalk.herokuapp.com/peptalk.gif)

Lägg upp din app i repo på Github och skicka länken till apps@rebla.se

Lycka till! 🙌

Rebla teamet

[1]:https://complimentr.com/
[2]:https://evilinsult.com/api/
[3]:https://zenquotes.io/api/random
