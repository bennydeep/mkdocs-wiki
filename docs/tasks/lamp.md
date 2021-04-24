# Lamp stack feladatsor

A feladat célja a jelentkezők rendszergazdai és PHP képességeinek felmérése. A jelentkező a feladatok elkészítése során bármilyen weboldat használhat.

## Telepíts fel (lehetőleg) egy Ubuntu 18.04 LTS-re egy alábbi architektúrát:

* Apache 2.4 webszervert, 80-as portra
* MySQL 5.5 adatbázist
* PHP 5.5-t
* PhpMyadmin

## Majd telepíts fel egy legújabb Wordpresst rá, és állítsd be a saját AWS Public domainedre.

## Shell scripting

Hozz létre Wordpressed admin felületén 2-3 cikket, generálj egy kis forgalmat a wordpressen, majd elemezd ki a logokat.

### Milyen parancssal keresnéd ki az Apache access logból a nem 200 HTTP kódú requesteket?

### Milyen paranccsal szednéd ki az aznap legtöbbet nézett URL-jei közül az első 5-öt az Apache logból?

### Milyen paranccsal határoznád meg a Wordpress főkönyvtárában, hogy mennyi az alkönyvtáraknak a mérete?


## Backup

Írj egy napi adatbázis backupokat készítő shell scriptet, ami a következőeket csinálja

* létrehoz egy könyvtárat az aktuális dátummal egy backup főkönyvtár alatt
* lekéri az adatbázisok neveit
* végigiterál az adatbázisokon, és csinál belük egy-egy adatbázis dumpot gzipbe

Írd ide a shell scripted elérhetőségét!

## PHP

* Írj ki a láblécbe (`footer.php`) a `</body>` elé PHP-val az aktuális dátumot és időt.

* Írj egy Wordpresstől különálló PHP scriptet a Wordpress gyökérkönyvtárába, ami csupán ennyit csináljon:
  - lekér adatbázisból véletlenszerűen egy publikus cikket
  - frissíti a cikk legutóbbi módosítási dátumát az aktuális dátumra
  - felvesz egy új commentet a cikkhez „Nagyon jó cikk” tárggyal.

Írd ide a PHP scripted elérhetőségét!

> Plusz pontot ér, ha a scriptet és a plugint is feltöltöd a github repositorydba.

