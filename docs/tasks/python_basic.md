# Python alapok

A feladtokhoz  3.6 vagy újabb python-t használj!

## 1. Köszönő program

Csinálj egy programot ami megkérdezi a a felhasználó nevét és köszönti `Hello Név!` formátumban, ahol a `Név` a felhasználó által megadott név.

## 2. Faktoriális

Csinálj egy olyan programot ami parancssori argumentumként kap egy számot és kiírja a terminába a kapott szám faktoriálisát

**Példa**
```sh
user: ~$ python fakt.py 4
24
user: ~$
```

## 3. .env

Adott a következő `.env` file ami egy nodeJs alkalmazás futtatásához szükséges környezeti változókat tartalmazza.

```
DB_HOST=localhost
DB_USER=
DB_PASSWORD = pw24
DB_PORT=3036
DB_NAME=db_name

# port to listen on
PORT=80
```

Írj egy programot ami parancssori argumentumként kap egy mysql url-t és kitölti a hiányzó változókat, illetve frissíti a régi értéket a kapott url szerint.


**Példa bemenet**
```
"mysql://username:password@host:3096/db_name"
```

**Példa kimenet**
```
DB_HOST=host
DB_USER=username
DB_PASSWORD=password
DB_PORT=3096
DB_NAME=db_name

# port to listen on
PORT=80
```

**Folder structure**
```
.
├── .env
└── url_parser.py
```


## 4. Hibakezelés

Egészítsd ki az előző feladat kódját, úgy hogy gond nélkül tudjon működni ha nem, vagy nem megfelelő bemenetet kap, esetleg nem létezik a `.env` file ott ahol futtatva van a program.


## 5. Cleanup script

Írj egy programot, ami terminálból kap egy JSON file-t és az abban meghatározott mappában és az összes almappájában törli a `node_modules` mappát és összes tartalmát.

A program valahányszor talál egy `node_modules` mappát, írja ki a terminálba, hogy hol találta azt (teljes elérési út). Plussz pont ha szines a log.

**Config file**
```json
{
    "entrypoint": "/home/user/workspace/"
}
```

**Folder structure**
```
.
├── workspace
│       ├── project1
│       │      ├── node_modules
│       │      └── server.js
│       ├── project2
│       │      ├── node_modules
│       │      └── app.js
│       ├── project3
│       └── cleanup.py
└── config.json
```

**Példa futtatás**
```bash
$ python cleanup.py ../config.json
```

## 6. PIP

* Csinálj egy virtuális környezetet. Tipp: python venv
* Telepíts egy python package-t a virtuális környezetbe. Például numpy.
* Irasd ki egy `requirements.txt` nevű fájlba hogy milyen package-ek vannak telepítve a virtuális környezetben
* Deaktiváld a virtuális környezetet.

## 7. Adatszerkezetek

Írd le miket tudsz a következő adatszerkezetekről python-ban:

* list
* tuple
* array
* str
* range
* dict
* set
* bool
