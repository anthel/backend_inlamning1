* Hur används HTTP-protokollet när du surfar in på en websida? Beskriv vilken metod, path, URI, response code och body som skickas in och svarar. Om du har svårt att bestämma dig för en url, ta ex. http://www.smp.se/kultur-noje/

När jag skriver in en URI i sökfältet skickas det en GET-request till den angivna adressen som i sin tur svarar med statuskod 200 (om allt gått bra) och skickar tillbaka det som finns på pathen som body, HTML och javascript, som sen visas i webbläsaren som en webbsida. 
Oftast finns det massa script och bilder som ligger på andra servrar än den man skrivit in, och requestsen blir då omdirigerade och pathsen kan se lite annorlunda ut.

* Beskriv HTTP-protokollets vanligaste metoder och vad de gör.

#### GET  
-Hämtar något på den angivna pathen
#### POST
-Skapar en resurs på angiven path
#### PUT
-Ersätter/byter ut hela innehållet på angiven resurs, eller skapar resurs om inget matchat
#### PATCH
-Ersätter DELAR av den angivna pathens resurs, eller skapar resurs om inget matchat
#### DELETE
-Tar bort resurser på den angivna pathen

* "http://localhost:3000/users?username=something" är en URI, beskriv vilka delar den består av och vad de kallas.

### http://
Detta är protokollet, eller schemat, som ska användas

### localhost:3000
Detta är domänen, följt av portnummer (deafult 80 för http, om inget annat angivits)

### users
Detta är pathen

### ?username=something
Detta är query parametrar

* På vilka tre sätt kan man skicka in parametrar i en HTTP-request? Ge exempel med curl.<br/>

#### `query parameter`
```sh
curl localhost:3000/users?name=ante
```
#### `path parameter`
```sh
curl localhost:3000/users/ante
```
#### `header parameter`
```sh
curl localhost:3000/users -H "name: ante"
```


## Feedback

Mycket nytt i denna kurs, men roligt. Tempot har varit lite ryckigt, ibland känns det som det är supermycket och ibland inte så mycket. Bra kurslitteratur.
