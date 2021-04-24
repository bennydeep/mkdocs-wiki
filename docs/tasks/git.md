# Git alapok

Ez a feladatsor a git használatáról fog szólni. 

## Git repository

Csinálj egy lokál repository-t. Adj hozzá egy `README.md` fájlt, és írd bele milyen paranccsal csináltad a repository-t.

Innentől minden kiadott parancsot írj bele ebbe a fáljba!

## Remote

Csinálj egy remote repository-t is ahová fel fogod tölteni a dolgokat. A repo legyen a céges gitlabon.

Itt igazából nem kell leírni semmit.

## Init

Töltsd fel az eddig létrehozott fájlokat gitlabra. A commit üzenet legyen 'Init'

## Branch

Csinálj egy külön branch-et, 'commands' névvel. Innentől ezen a branch-en dolgozz!

## Merge request

A README.md fájlnak most tartalmaznia kell a parancsot amivel létre hoztad a branch-et. Ezt töltsd fel a gitlabra.

Csinálj egy `Work In Progress` merge requestet. A neve legyen 'Commands', és a `commands` branchet merge-eld a `master`-be.

Adj hozzá reviewer-ként a kéréshez! A review most kivételesen itt fog történni, nem Jira-n. A Jira kártyát ettől függetlenül ugyan úgy használd mint eddig!

Arra is ügyelj, hogy a merge request-ből egyértelmű legyen ki felelős az azt tartalmazó módosításokért!

## Checkout

Commit-olj minden módosítást, és válts át a master branch-re.

csinálj egy új fájlt `feature.js` néven, és írd bele a következőt:
```javascript
console.log('Hello, I\'m a new feature')
```

Ez is legyen commit-olva és feltöltve a remote-ra

## WIP
Jelezd a merge requesten, hogy kész a munkád. Ugyan ezt tedd meg Jira-n is a megfelelő módon

## Final
Bizonyosodj meg róla hogy mindent feltöltöttél gitlabra
