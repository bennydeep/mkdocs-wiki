# Docker beugró feladatsor

Készíts részletes dokumentációt a kiadott parancsokról, indoklásokkal és válaszold meg a kérdéseket, járj utána, ha nem tiszta.

## 1.Hozz létre egy felhasználót a szerveren

A neve legyen: `demo`

## 2. Telepítsd fel a dockert a szerverre

## 3. Csináld meg, hogy a demo user tudja listázni a konténereket

## 4. Telepítsd fel a `docker-compose`-t is

## 5. Indítsd el a `hello-world` image-ből egy konténert

## 6. Az előzőhöz hasonlóan szintén indíts egy konténert, de most adj neki nevet

A neve legyen: `demo-hello`

## 7. Indítsd egy `nginx` konténert

Az nginx 80-as portját, a 81-es host portra vezesd ki

## 8. Indítsd egy `apache` konténert

Az apacje 80-as portját, a 82-es host portra vezesd ki

## 9. Hogyan tudnád csökkenteni a 6-7. feladat image méretét?

Ha tudod mutasd meg

## 10. Készíts egy `demo.html`-t

A tartalma tetszőleges, de látszódjon, hogy nem a gyári html-ről van szó

## 11. Indíts egy újabb konténert nginx vagy apache-ból (amelyik neked jobban tetszik)

A portot a 83-as portra nyisd ki

A `demo.html`-t kellene felcsatolni neki, hogy amikor megnyitom az oldalt és a `demo.html`-t akarom elérni, látszódjon a `demo.html` tartalma

## 12. Készíts egy `Dockerfile`-t

A kiindulási image szintén tetszőleges (nginx/apache)

Másold be a `demo.html`-t a default `index.html` helyére a `Dockerfile`-ban

Állítsd be, hogy amikor belépünk a konténerbe, akkor egyből a `demo.html` könyvtárába lépjünk be

## 13. Hogyan build-eled le az image-t?

A neve legyen {dockerhub_username}/demo:latest

## 14. Töltsd fel a dockerhub-ra

## Kutatómunka

### 15. Mi a különbség az `ADD` és a `COPY` parancsok között?

### 16. Mi a különbség a `CMD` és az `ENTRYPOINT` parancsok között?

### 17. Hogyan tudod felülírni őket, amikor a docker run parancsot alkalmazod?
