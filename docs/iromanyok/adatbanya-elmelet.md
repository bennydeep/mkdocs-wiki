# Adatbányászat

 ^^Test^^

## 1. Az adatbányászat definíciói, alapfogalmai, példák. Az adatbányászat eredete. Alapfeladatok: felügyelt és nem-felügyelt adatbányászat. Alkalmazási területek. Kihívások. Adatfeltárás: leíró statisztikák és vizualizáció.

**Adatbányászat** alatt hatékony módszerek használatát értjük adatok
nagyon nagy összességének az elemzésére és hasznos, lehetőleg nem várt
mintázatok kinyerésére.

\-**Implicit** (rejtett), korábban nem ismert és potenciálisan hasznos
információ nem-triviális eszközökkel való feltárása.

**-**Nagy tömegű adatokfeltárása és elemzése **félig automatikus** módon
azért, hogy értelmes mintázatokat fedezzünk fel.

**-**A **KDD-folyamat** része: **K**nowledge **D**iscovery from
**D**atabases

> Adatrögzítés, adattisztítás, adatintegráció, adatszelekció,
> adattranszformáció, adatbányászat, kiértékelés, tudásreprezentáció
> (2.-5.: **adaattárház** kialakítása)

**Miért bányászunk?**

-Rengeteg az adat, nagy sebességgel gyűlnek

-Egyre olcsóbb számítógépek, nagyobb teljesítményűek

-Erősödő verseny

-Hagyományos módszerek haszontalanok (pl. tudományban)

-adatok szegmentálása, osztályozása

-hipotézisek megfogalmazása

Nagy számú **nyers adat,** melyekből elemzéssel tudunk **tudást**
kinyerni.

**Adatok**

Többféle **típus**: táblázatok, idősorok, képek, grafikonok, stb.

**Tér** és **időbeli** szempontok.

**Összekapcsolt** adatok különféle fajtái: A mobiltelefonból
összegyűjthetjük a felhasználók helyét, baráti körét, megérkezését adott
helyekre, twitteren közölt véleményét, kamera képeket, kereső
szoftverekben elindított lekérdezéseket.

**Példák**

**Tranzakciós adatok**: Valódi ügyfelek ; **Dokumentum adatok:** web
(1335 milliárd weblap), Wikipedia (5.5 millió cikkely); **Hálózati
adatok:** Web, Facebook, Twitter; **Genom-szekvenciák:** gén
kifejeződési adatok; **Magatartási adatok:** A mobilok- GPS, Facebook,
Képek)

**Mi nem adatbányászat?** Telefonszám kikeresése a telefonkönyvből,
„Amazon" szóval kapcsolatos infók lekérdezése Googleval.

**Mi adatbányászat?** Bizonyos nevek elterjedtebbek egyes területeken az
USA-ban, Csoportosítsuk a tartalmuk alapján azokat a dokumentumokat,
amelyeket egy keresővel kaptunk (pl. Amazonas esőerdő, Amazon kiadó)

**Mi az adatbányászat?**

**Üzleti** szempont: adat = versenyelőny

**Tudományos** szempont: rengeteg adatfel kell őket dolgozni

**Skála** (adat méret és jellemző dimenzió): sok adat, dimenzióprobléma

**Adatbányászati modellek**

\-**magyarázzák** az adatokat (pl. egy egyszerű függvénykapcsolat)

\-**előrejelzik** a jövőbeli adat eseteket

\-**összegzik** az adatokat

-kinyerik a kiemelkedő **jellemzőit** az adatoknak

**Adatbányászat eredete**

Ötleteket, módszereket merít a **gépitanulás/MI**, az
**alakfelismerés**, a **statisztika** és az **adatbázisrendszerek**
területéről.

A hagyományos módszerek alkalmatlanok lehetnek köszönhetően az
adattömegnek, a nagy dimenziónak, az adatok heterogén és elosztott
természetének.

**Adatbányászati feladatok**

**Előrejelzés** -- predikció (**Felügyelt adatbányászat**)

\-**Egyes változók** segítségével becsüljük meg, **jelezzük előre** más
változók **ismeretlen** vagy **jövőbeli értékét.**

**Leírás** -- jellemzés (**Nem-felügyelt adatbányászat**)

-Találjunk olyan, az emberek számára interpretálható **mintázatot**,
amely **jellemzi az adatot**.

**Adatbányászati alapfeladatok**

-Osztályozás (Felügyelt)

-Csoportosítás (Nem-felügyelt)

-Társítási (Asszociációs) szabályok keresése (Nem-felügyelt)

-Szekvenciális mintázatok keresése (Nem-felügyelt)

-Regresszió (felügyelt)

-Eltérés/Rendellenesség keresés (Felügyelt)

**Osztályozás**

Adott **rekordok egy halmaza (tanító állomány**), melyben minden rekord
**attribútumok értékeinek egy halmazából** áll, az attribútumok egyike
(vagy némelyike) az ún. **osztályozó változó**.

Találjunk olyan **modellt** az osztályozó attribútumra, amely **más
attribútumok függvényeként állítja elő**.

Cél: **korábban nem ismert rekordokat** kell olyan **pontosan
osztályozni** ahogyan csak lehetséges.

A **tesztállomány** a modell **pontosság**ának meghatározására szolgál.
Az adatállományt két részre osztjuk, a tanítón illesztjük a modellt, a
tesztelőn pedig megállapítjuk a hibáját.

**Osztályozás alkalmazása**

**Direkt marketing**: levelezés ktg.-jének csökkentése, azon ügyfelek
megcélzásával akik valószínű vásárolni is fognak

**Csalás keresés**: pl. hitelkártya tranzakcióknál.

**Ügyfél lemorzsolódás:** ügyfél elvesztésének előrejelzése

**Égboltfelmérés katalogizálása**: égi objektumok osztályainak (csillag
vagy galaxis) előrejelzése,

**Csoportosítás**

**Adott rekordok** (pontok) egy halmaza, melyeket **attribútumok egy
halmazával** írunk le, továbbá adott közöttük egy **hasonlósági
mérték**. Találjunk olyan **csoportokat(klasztereket)**, amelyekre az
azonos csoportban lévő rekordok minél **hasonlóbbak**, a különböző
csoportokban lévők pedig minél **kevésbé hasonlóak.**

**Hasonlósági mértékek**: euklideszi távolság, ha az attribútumok
folytonosak, egyéb, a feladattól függőmérőszámok.

**Csoportosítás alkalmazása**

**Piaci szegmentáció:** ügyfelek csoportosításamás marketing eszközöket
használunk

**Dokumentumok csoportosítása**: kulcsszavak alapján (pl. gyakori
kifejezések azonosítása)

**Társítási szabályok (Asszociációs szabályok)**

Adott rekordok egy halmaza, amely **tételek** (termékek) egy összességét
tartalmazza. Keressünk olyan **összefüggéseket, következtetéseket,**
amely **egyes tételek előfordulását előrejelzi** más **tételek
előfordulása alapján.**

**Társítási szabályok alkalmazása**

**Marketing és reklám**: vásárlói kosár előrejelzése mit reklámozzunk
együtt

**Bevásárlóközpont polckezelés**: gyakori tételcsoportok meghatározása
az áruházakban

**Alkatrész gazdálkodás**: szerviz vállalat megfelelő alkatrészeket
tárolja és megfelelő mennyiségben

**Szekvenciális mintázatok**

Adott *objektumok* egy halmaza úgy, hogy minden **objektumhoz** tartozik
***eseményeknek egy sorozata*.** Keressünk olyan **szabályokat,**
amelyek a különböző **események között** minél erősebb szekvenciális
**függéseket** jeleznek előre. (A B) (C) (D E)

A **szabályokat** az első felfedezett **mintázatok alakítják** ki. A
mintázatokban előforduló eseményeknek időbeli peremfeltételeknek kell
eleget tenniük.

**Szekvenciális mintázatok alkalmazása**

**Hibaüzenet**: (hiba_üzenet túlfeszültség) (belső_riadó) (tűzoltókat
hívjuk)

**Tranzakciók sorozata automatizált vásárlásnál:** vesz futócipőt és
nadrágot futódzseki

**Regresszió**

**Jelezzük előre** egy adott **folytonos változó értékét** más
**változók értékeit felhasználva**, lineáris vagy nemlineáris
**függőséget feltételezve**. Alaposan vizsgálták a statisztika és a
neurális hálók területén.

**Regresszió alkalmazása**

Új termék keresletének előrejelzése; Időjárás előrejelzése (szél nap
párahány fok lesz?); Részvényárfolyamok alakulása.

**Eltérés/Rendellenesség keresés**

A **normális** viselkedéstől szignifikáns **eltérések keresése.**

**Eltérés/Rendellenesség keresés alkalmazása**

Hitelkártya csalások keresése

Hálózati behatolás érzékelése

**Kihívások az adatbányászatban**

-Skálázhatóság

**-Dimenzió probléma**

-Összetett és heterogén adatok

-Nem-hagyományos elemzés

**-Adatminőség**

-Jogosultság kezelés és elosztott adatok

-Adatvédelem

-Adatfolyamok

**Adatfeltárás**

Az adatok előzetes feltárása (vizsgálata) segít jellemzőinek jobb
megértésében.

**Motiváció**i: segít a helyes módszer kiválasztásában az
előfeldolgozásban és az elemzésnél

**Módszerei**: Leíró statisztikák, Megjelenítés, grafikus
eszközök, OLAP: közvetlen analitikus feldolgozás.

**Leíró statisztikák**

Olyan **mutatószámok**, melyek az adatok tulajdonságait **összegzik**,
tömörítik. Ezek a tulajdonságok lehetnek **gyakoriságok**, **helyzet**
(átlag, percentilisek, medián, módusz), **szóródás** (terjedelem,
variancia, std. dev.) és **alakmutatók**.

A legtöbb leíró statisztika az adatállomány egyszeri átfésülésével
számolható.

**Gyakoriság:** egy attribútumérték **hányszor fordul elő az
adatállományban**. (pl. 5-ös érték hányszor van; (ált. **diszkrét
(kategorikus**) attribútumoknál használjuk)

**Helyzetmutatók**

**Módusz:** a **leggyakoribb** attribútum érték (ált. diszkrét
attribútumoknál)

**Percentilisek**: X attribútum esetén a p-edik percentilis az az X~p~
érték, amelynél az X-re megfigyelt értékek **p%-a kisebb**(0≤p≤100).
(folyt attr; sorrendi, különbség skálán)

**Medián**: az 50%-os percentilis, attribútum értékek 50%-a kisebb.

**Átlag**: legáltalánosabb mutató, **érzékeny a kiugró értékekre**, ezt
a mediánnal vagy a nyírott átlaggal (min és max elhagyásával számolt
átlag) kivédhetjük

**Szóródás mutatók**

**Terjedelem**: a maximum és minimum eltérése

**Variancia** (standard deviáció): a **szóródás** legelterjedtebb
mérőszáma. Érzékeny a **kiugró értékekre**, ezért helyette: átlagos
abszolút eltérés, medián abszolút eltérés, interkvartilis terjedelem.

**Alakmutatók**

**Normális eloszlás**: teljesen jellemzi a várható értéket és a
szórást.(nevezetes eloszlás)

**Hatvány-eloszlás**: log-log grafikon, egy lineáris kapcsolat a log-log
koordinátarendszerben pl. szavak eloszlása, bejövő és kimenő linkek
web-lapokon fájlok mérete, jövedelem eloszlása

**Megjelenítés, grafikus eszközök \-- Vizualizáció**

Megjelenítés az adatoknak **vizuális vagy táblázatos** formában való
átalakítása a célból, hogy az adatok **jellemzői** és a közöttük lévő
**kapcsolat** vizsgálható és elmondható legyen.

Az adatok megjelenítése az adatfeltárás egyik legerősebb,
leglátványosabb és legvonzóbb eszköze.

--Az embernek jól kifejlett képessége, hogy **képileg megjelenített**
nagy információt elemezzen.

--Általános **mintázatokat, trendeket** észlelhetünk.

--**Kiugró értékeket** és szokatlan mintázatokat találhatunk.

pl. tengerfelszín hőmérséklete

**Reprezentáció**: Az információ vizuális formába való leképezése. attr.
és kapcsolatok grafikusan

-Objektumokat gyakran pontokkal ábrázolunk; értékeket koordinátával +
szín, méret

**Elrendezés**: Vizuális elemek elhelyezése egy képernyőn. Nagyban
befolyásolja, hogy milyen könnyű az adatainkat megérteni.

**Szelekció**: Egyes objektumok és attributumok **elhanyagolása.** A
szelekció magába foglalhatja attributumok egy részhalmazának
kiválasztását.

--Gyakran használunk **dimenzió csökkentést**, hogy a dimenziót kettőre
vagy háromra redukáljuk.

--Más megközelítés: vegyünk **attributum párokat**.

**DE** óvatosan kellkapcsolatok ne torzuljanak;

-ha túl sok a pont leolvashatatlan a kapcsolat és a kiugró értékekkel is
vigyázni kell

**Megjelenítési módszerek**

**Hisztogram**: Egy változó értékeinek **eloszlását** mutatja.
Osszuk az értékeket diszjunkt intervallumokba és ábrázoljuk a
**gyakoriságokat** egy oszlopgrafikonon. A oszlopok magassága az
intervallumba eső objektumok száma. A hisztogram alakja függ a
**beosztás finomságától.**

**Kétdimenziós hisztogram**: Két attribútum értékeinek együttes
eloszlását mutatja.

**Dobozábra**: Adatok **eloszlásának** szemléltetése a
**percentilisek** használatával, attribútumok **összehasonlítására**
használható.

**Pontdiagram**: Az attribútum értékek **pontoka**t határoznak meg a
síkban (térben). 2 dimenzió, néha 3D Plusz dimenziók: méret, alak, szín
markereket. Sokszor hasznos **pontdiagramok egy mátrixát** elkészíteni,
amely **több attribútum pár kapcsolatát** összegzi kompakt módon.

**Kontúrábra**: Hasznos amikor egy **folytonos attribútumot**
mérünk egy **térbeli rácson.** A síkot tartományokra bontjuk a hasonló
értékek alapján. A **kontúr vonalak**, amelyek az **egyenlő értékeket**
kötik össze, alkotják ezeknek a tartományoknak a határait. A
legismertebb példa a **tengerszint feletti magasság domborzati
térképeken**. Szintén megjeleníthetünk így hőmérsékletet, csapadékot,
légnyomást stb.

**Mátrix ábra:** Egy teljes adatmátrixot jeleníthetünk meg vele. Hasznos
amikor az objektumok egy **osztályozó változó szerint vannak rendezve**.
Általában az attribútumokat normalizálni kell, hogy megelőzzük azt, hogy
egy attribútum domináljon. A **hasonlóság** és **távolságmátrix** ábrája
szintén hasznos az objektumok közötti kapcsolatok megjelenítésére.

**Párhuzamos tengelyek**: **Magas dimenziós** adatok attribútum
értékeinek megjelenítésére szolgál. Merőleges **koordinátatengelyek**
helyett használjunk **párhuzamosakat.** Minden objektum attribútum
értékeit a megfelelő koordinátatengelyen egy pontként ábrázolva a
pontokat vonallal kötjük össze. Minden **objektumot egy vonal
reprezentál**. Gyakran a vonalak teljesen vagy egyes attribútumok mentén
**csoportosulnak** az objektumok különböző csoportjaira utalva. Ennek
felimerésére előbb rendezzük az attribútumokat.

**Csillag ábra**: A párhuzamos koordinátákhoz hasonló azzal az
eltéréssel, hogy a koordináták egy **centrumból sugarasan indulnak**.
Egy objektum értékeit összekötő vonalak egy poligont alkotnak.

**Chernoff arcok**: A módszer Herman Chernoff-tól származik. Az
attribútumokhoz az **arc egy-egy jellemzőjét** kapcsoljuk. Minden egyes
**attribútum érték** a megfelelő **arc-jellemző** megjelenését határozza
meg. Mindegyik **objektum egy külön arc lesz.** Az emberek
arcfelismerési képességére támaszkodik.

## 2. Adatbányászati folyamat. Adattípusok, mérési skálák. Adatállomány típusok. Adatminőségi problémák. Előfeldolgozás: aggregálás, mintavétel, dimenziócsökkentés, jellemzőszelekció és transzformáció. OLAP eszközök.

**Adatelemzési folyamat**

Adat előfeldolgozása Adatbányászat Eredmények utófeldolgozása

**Előfeldolgozás**: a valós adatok zajosak, hiányosak és
inkonzisztensek(ellentmondó, következetlen). **Adattisztítás** is
szükséges az adatok megértéshez

--Módszerek: Mintavétel, Dimenziócsökkentés, Jellemző szelektálás.

--Piszkos munka, de gyakran a legfontosabb lépés az elemzésben.

**Utófeldolgozás**: Tegyük az eredményeket hasznossá és cselekvésre
ösztönzővé a felhasználó számára

--A kapott eredmény fontosságának statisztikai vizsgálata

--Vizualizáció.

Az **elő-és utófeldolgozás** gyakran maga is egy **adatbányászati
feladat.**

**Adatbányászati folyamat (5 lépcsős folyamat)**

\-**Mintavétel**: az adatok előkészítése az adattárházból

**-Feltárás:** új összefüggések, mintázatok keresése

\-**Módosítás:** attribútumok, rekordok, mezők módosítása, kitöltése

\-**Modellezés**: analitikus (elemző) modellek illesztése

\-**Kiértékelés**: a modell(ek) jóságának, hasznosságának mérése

**Adat**: Objektumok attribútumainak numerikusan jellemzett összessége.

**Attribútum**: egy objektum tulajdonsága, jellemzője. (változó,
jellemző)

**Objektum**: Attribútumok értékeinek egy összessége. (rekord, pont,
eset, mintaelem, egyed, entitás)

**Attribútumok típusai; tulajdonságai (Adattípusok)**

\-**Névleges** (nominális) pl. ID, szemszín, irányítószám; **egyezőség**

\-**Sorrendi** (ordinális) pl. rangsorolás (burgonyaszirom íze 1-10
skálán), fokozat, magasság mint {magas,átlagos, alacsony}; **egyezőség
és rendezés**

\-**Intervallum** pl. dátum, hőmérséklet; **egyezőség, rendezés és
összeadás**

\-**Hányados** pl. abszolút hőmérséklet, hosszúság, idő; **egyezőség,
rendezés, összeadás és szorzás**

**Attribútum értékek tulajdonságai**

Egy attribútum típusa attól függ, hogy milyen tulajdonságokkal
rendelkezik.

-Egyezőség, különbözőség: = ≠

-Rendezés: \< \>

-Összeadás, kivonás: + -

-Szorzás, osztás: \* /

**Diszkrét attribútumok**

--**Véges** vagy megszámlálható végtelen sok értéke lehet. Pl:
irányítószám, darabszám, szavak száma dokumentumokban.

--Gyakran **egész** értékű változókkal reprezentáljuk.

--Megjegyzés: **a bináris attribútumok** a diszkrét attribútumok egy
speciális esete, csak 2 érték: 0 v. 1

**Folytonos attribútumok**

--Az attribútum értékek **valós számok**. Pl: hőmérséklet, magasság,
súly.

--Gyakorlatban a valós értékek csak véges sok tizedesjegyig mérhetőek és
ábrázolhatóak.

--A folytonos attribútumokat általában lebegőpontos változókkal
reprezentáljuk.

**Állományok típusai**

**Rekord**: Adatmátrix (adatbázisok), Dokumentum mátrix
(szövegbányászat), Tranzakciós adatok

**Gráf**: World Wide Web (webgráf), Molekula szerkezetek

**Rendezett**: Térbeli adatok, Időbeli adatok, Szekvenciális adatok,
Génszekvenciák adatai

**Strukturált adatok fontos jellemzői**

**Dimenzió**: dimenzió probléma

**Ritkaság**: Csak az előforduló esetek elemezhetőek

**Felbontás**: A mintázat függ a skálától

**Rekordokból álló adatok**

Olyan adatok, amelyek rekordok egy halmazából állnak, ahol mindegyik
rekord attribútum értékek egy adott halmazából áll.

**Adatmátrix**

Ha az objektumokat leíró adatok **numerikus attribútumok** egy adott
halmazából állnak, akkor gondolhatunk rájuk úgy, mint **pontokra a
többdimenziós térben**, ahol minden egyes dimenzió egy attribútumot
reprezentál.

Az ilyen adatokat egy **n x p --es mátrixszal** reprezentálhatjuk,
amelynek n sora az objektumoknak, p oszlopa pedig az attribútumoknak
felel meg.

**Dokumentum mátrix**

Minden dokumentumot **kifejezések egy vektorával** írunk le. Minden
**kifejezés** egy **attribútuma** a vektornak. Minden attribútum
**érték** annak a száma, hogy az attribútumhoz tartozó **kifejezés
hányszor fordul** elő a dokumentumban.

**Tranzakciós adatok**

Speciális rekord típusú adatok, ahol minden rekord(tranzakció) **tételek
egy halmazát** tartalmazza.

--Pl.: tekintsünk egy élelmiszerboltot. A tranzakció azon árucikkekből
áll, amelyeket a vásárló vesz egy vásárlás során, míg a tételek a
vásárolt árucikkek.

**Gráf adatok**

Pl: általános gráf, HTML linkek

**Kémiai adatok**

Pl: Benzin molekul: C~6~H~6~ (ábrája)

**Rendezett adatok**

Tranzakciók sorozatai, génszekvenciák, tér és időbeli adatok

**Adatminőségi problémák**

Milyen adatminőségi problémák léphetnek fel? Hogyan ismerjük fel ezeket
az adatainkon? Hogyan kezeljük?

Pl: **zaj** (hiba) és **kiugró** adatok, **hiányzó** adatok,
**duplikált** adatok

**Zajos adatok**

Zaj alatt az **eredeti** (igazi) **érték módosulását** értjük. Pl: az
emberi hang torzulása, ha rossz telefonon beszélünk, szemcsésedés a
képernyőn.

**Kiugró adatok**

A kiugró adatok olyan objektumok adatai, amelynek jellemzői **jelentősen
eltérnek** az adatállományban lévő más objektumok adataitól.

**Hiányzó adatok**

**Okai**: Az információt nem gyűjtöttük össze (pl. az emberek
visszautasították a koruk és súlyuk megadását).

--Egyes attribútumok nem alkalmazhatóak minden esetben (pl. a
gyerekeknek nincs jövedelme).

**Kezelése:**

--Objektumok (rekordok) **törlése.**

--**Hiányzó adatok becslése.**

--A hiányzó értékek figyelmen kívül hagyása az elemzésnél.

--**Helyettesítés** az összes lehetséges értékkel (a valószínűségek
alapján).

**Duplikált adatok**

Az adatállomány tartalmazhat olyan rekordokat, amelyek **más rekordok**
pontos ill. kevésbé pontos **ismétlődései.** Főként akkor merül fel, ha
heterogén forrásokból egyesítjük az adatokat.

Pl: Ugyanaz az ember többféle e-mail vagy lakcímmel.

**Adattisztítás**

Az a folyamat, mely során az **ismétlődő adatokat kezeljük.**

**Adatok előfeldolgozása**

\-**Aggregálás** (Attribútumok összevonása)

\-**Mintavétel**

**-Dimenzió csökkentés**

-Jellemzők, attribútumok **létrehozása** (jellemzők szelektálása)

-Diszkretizáció és binarizálás

-Attribútum **transzformáció**

**Aggregálás**

Kettő vagy több attribútum (objektum) **kombinálása** egy attribútummá
(objektummá).

Cél:

--Adatcsökkentés: Csökkentsük az attribútumok vagy az objektumok számát.

--A skála megváltoztatása: A városokat régiókba, megyékbe, országokba
fogjuk össze.

--Az adatok stabilitásának növelése: Az aggregált adatok ingadozása
csökken (simítás).

**Mintavétel**

Az **adatszelekció** fő módszere. Egyaránt használatos az adatok
előzetes vizsgálatánál és a végső adatelemzésnél.

A statisztikusok azért használnak mintavételezést mivel a teljes
populáció megfigyelése túl drága vagy túl időigényes. Az adatbányászok
azért használnak mintavételezést mivel a teljes adatállomány
(adattárház) feldolgozása túl drága vagy túl időigényes.

**A hatékony mintavétel alapelve:**

--A mintával ugyanolyan jól tudunk dolgozni, mint a teljes
adatállománnyal, amennyiben a minta **reprezentatív.**

--A minta akkor reprezentatív, ha a számunkra **fontos tulajdonságok**
szempontjából ugyanúgy viselkedik, mint a teljes adatállomány.

**Mintavételi módok**

**Egyszerű véletlen minta:** Ugyanakkora valószínűséggel választunk ki
minden objektumot.

**Visszatevés nélküli mintavétel:** Ha egy objektumot már
kiválasztottunk, akkor azt töröljük az adatállományból.

**Visszatevéses mintavétel:** Az objektumot nem töröljük az
adatállományból akkor sem, ha a mintavétel kiválasztotta. Ekkor egy
objektumot többször is kiválaszthatunk.

**Rétegzett mintavétel:** Osszuk fel az adatállományt részekre, majd
vegyünk véletlen mintákat minden részből.

**Mintanagyság**

Mekkora mintanagyság szükséges, hogy 10 csoport mindegyikéből
kiválasszunk legalább egy objektumot?

**Dimenzió probléma**

Amikor a **dimenzió nő** a rekordok (pontok) egyre **ritkábbak** lesznek
a **térben**, ahol elhelyezkednek.

A rekordok (pontok) közötti **távolság és sűrűség**, melyek alapvetőek
csoportosításnál és kiugró adatok meghatározásánál, **fontossága
csökken.**

**Dimenzió csökkentés**

Cél:

--Elkerülni a **dimenzió problémát.**

--Csökkenteni az adatbányászati algoritmusokhoz szükséges **időt és
memóriát**.

--Segíteni az adatok könnyebb **megjelenítését.**

--Segíteni a hiba csökkentését és a **lényegtelen** jellemzők
meghatározását majd elhagyását.

Módszerek:

--Főkomponens analízis (PCA)

--Szinguláris felbontás (SVD)

--Egyéb felügyelt és nemlineáris módszerek, pl. többdimenziós skálázás
(MDS)

**Főkomponens analízis (PCA)**

Célja olyan **vetítés** (projekció) meghatározása, amely leginkább
megőrzi az adatokban lévő **variációt**, **sokszínűséget.**

-Határozzuk meg a **kovariancia mátrix sajátvektorait.**

-Az **új teret** (koordinátatengelyeit) ezek a **sajátvektorok**
határozzák meg.

**ISOMAP**

-Állítsuk elő a **szomszédsági gráfot**.

-A gráf minden pontpárára számoljuk ki a **legrövidebb út
hosszát**--geodetikus távolság.

-Erre a távolság mátrixra alkalmazzuk az MDSt (többdimenziós
skálázást---dim. csökkentő eljárás).

**Jellemzők részhalmazainak szelekciója**

A **dimenzió csökkentés** egy másik útja.

**Felesleges jellemzők**: Egy vagy több attribútum által hordozott
**információt** részben vagy teljesen **megismétel**. Pl: egy termék
vételára és az utána fizetendő adó.

**Lényegtelen jellemzők**: **Nem** tartalmaznak az aktuális
adatbányászati feladat számára **hasznos** információt. Pl: a hallgató
NEPTUN kódja többnyire nem befolyásolja a tanulmányi eredményt.

**Szelekciós módszerek:**

--Nyers erő (**brute force)** megközelítés: Próbáljuk ki a jellemzők
összes részhalmazát az adatbányászati algoritmus inputjaként.

--**Beágyazott** megközelítés: A jellemzők szelekciója az adatbányászati
feladat szerves részét alkotja.

--**Szűrő** megközelítés: A jellemzőket az adatbányászati algoritmus
futása előtt szelektáljuk.

--Borító (wrapper) megközelítés: Az **adatbányászati algoritmust**
fekete dobozként használjuk a **legjobb attribútum részhalmaz**
megtalálására.

**Új jellemzők (attribútumok) létrehozása**

Olyan új attribútumok létrehozása, amelyek az adatállományban lévő
lényeges információkat **használhatóbb formában** tartalmazzák, mint az
eredeti attribútumok.

Három általános módszer

--**Jellemző kinyerés** (feature extraction): terület függő (pl.
képfeldolgozás, földrajz)

--**Új térre** való leképezés

--Jellemző **szerkesztés**: jellemzők kombinálása

**Új térre való leképezés**

-Fourier transzformáció

-Wavelet (hullám) transzformáció

**Felügyelt diszkretizálás**

Entrópia alapú megközelítés

**(Nem-Felügyelt diszkretizálás)**

**Attribútumok transzformációja**

Olyan függvény, amely adott attribútum értékeinek halmazát **képezi le**
helyettesítő értékek egy **új halmazára** úgy, hogy minden **régi
érték** egy **új értékkel azonosítható**.

--Elemi függvények: x^k^, log(x), e^x^, \|x\|

--Standardizálás és normalizálás

**OLAP**

A **közvetlen analítikus feldolgozás** (OLAP: On-Line Analytical
Processing)

A relációs adatbázisok az **adatokat** táblákban, míg az OLAP
**többdimenziós tömbökben** tárolja.

Számos olyan **adatelemzési** és **adatfeltárási** módszer van, amely
ezzel az adattárolási móddal **könnyebbé** válik.

**Többdimenziós tömbök létrehozása**

A táblázatos adatok többdimenziós tömbökké való átalakításának **két fő
lépése.**

--Először határozzuk meg mely attribútumok lesznek a
**dimenziók** és mely attribútum lesz a **cél attribútum**, amelynek
értékei a többdimenziós tömb elemei lesznek.

-A **dimenzió attribútum**oknak **diszkrétek**nek kell lenniük.

-A **cél attribútum** általában a darabszám vagy egy **folytonos**
változó, pl. egy tétel költsége.

> -Előfordulhat, hogy egyáltalán nincs cél attribútum csak olyan
> objektumok darabszáma, melyeknek ugyanazok az attribútum értékei.

--Másodszor számoljuk ki a többdimenziós tömb minden elemének
értékét **a célattribútum értékeinek összegzésével**, vagy az összes
olyan objektum **összeszámolásával**, amely attribútum **értékei**
**megfelelnek az adott elemnek.**

**OLAP műveletek**

**Adatkocka**

Az OLAP alapvető művelete az adatkocka létrehozása.

Az adatkocka az adatoknak a **többdimenziós megjelenítése** az **összes
lehetséges összesítésükkel.**

Az összes lehetséges összesítés: összesítések melyeket úgy kapunk, hogy
**kiválasztjuk dimenziók egy részhalmazát** és az **összes többire
összegzünk.**

Pl. alfaj dimenziót választjuk az írisz adatoknál és az összes többi
dimenzió mentén összegzünk: egy egydimenziós tömb 3 elemmel, ahol az
elemek az egyes alfajba tartozó virágok számát mutatják.

pl. Tekintsünk egy olyan adatállományt, ahol a rekordok termékek
boltokban különböző időpontokban eladott mennyisége. Ezek az adatok egy
3 dimenziós tömbbel reprezentálhatóak. A kétdimenziós összegzések száma
3 (3 alatt 2), az egydimenziós összegzések, száma 3 és 1 db
nulla-dimenziós összegzés van (ez a teljes összeg).

**Szeletelés**

A szeletelés **cellák** egy olyan **csoportjának a kiválasztását**
jelenti a teljes többdimenziós tömbből, amelyet értékeknek **egy vagy
több dimenzió menti rögzítésével** kapunk. (attribútum szerint)

**Kockázás**

A kockázás **cellák** egy olyan **részhalmazát** jelenti, amelyet
**attribútum értékek** egy **tartományának megadásával** kapunk. Ez
ekvivalens azzal, hogy a teljes tömbből egy résztömböt választunk ki.

(attribútum érték szerint)

**Göngyölítés és lefúrás**

Az attribútum értékek gyakran **hierarchikusan** szerveződnek.

--Minden dátumhoz tartozik év, hónap és nap.

--A helyhez tartozik kontinens, ország, megye és település.

--A termékek különféle osztályokba sorolhatóak, pl. ruházat,
elektronika, bútor.

Ezek az osztályok gyakran **beágyazódnak egymásba** és fát alkotnak
(taxonómia)

--Az év hónapokból, a hónap napokból áll.

--Az ország megyéket, a megyék városokat tartalmaz.

Ez a **hierarchia teszi lehetővé a göngyölítés és lefúrás műveleteket.**

--Az eladási adatokat **összegezhetjük (göngyölíthetjük**) az összes
dátumra egy hónapon belül.

--Megfordítva egy olyan adattábla esetén, ahol az idő dimenzió hónapokra
van **bontva**, a havi eladásokat bonthatjuk napi szintre **(lefúrás**).

--Hasonlóan göngyölíthetünk vagy lefúrhatunk a hely vagy a termék
azonosító mentén.

**\
**

## 3. Osztályozási alapfogalmak. Döntési fa alapú osztályozók. Fa építési algoritmusok: Hunt, CART, CHAID, C4.5. Osztályozók kiértékelése: tévesztési mátrix, metrikák, ROC görbe.

**Osztályozás**

Adott **rekordok** egy halmaza (***tanító adatállomány***). Minden
rekord attribútumok értékeinek egy halmazából áll, az **attribútumok
egyike** az ún. **osztályozó** vagy célváltozó.

Találjunk olyan ***modellt*** az osztályozó attribútumra, amely más
attribútumok **függvényeként** állítja elő.

Cél: **korábban nem ismert** rekordokat kell olyan **pontosan
osztályozni** ahogyan csak lehetséges.

A ***tesztadat állomány*** a modell **pontosság**ának meghatározására
szolgál. Általában az adatállományt két részre bontjuk, a tanítón
illesztjük a modellt, a tesztelőn pedig validáljuk.

O**sztályozás** egy olyan **f** célfüggvény **megtanulása**, amely az
**x** attribútumhalmazt képezi le **y címkék** egy előredefiniált
halmazára.

Az **f** célfüggvényt osztályozási modellnek nevezzük.

**Leíró modellezés:** **Magyarázó eszköz** arra, hogy
**különbséget** tegyünk objektumok különböző **osztályai között** (pl.
megértsük, hogy miért csalják el egyes emberek az adójukat).

**Prediktív modellezés: Jelezzük előre** korábban nem
látottrekordok osztályát.

**Tanuló adatállomány**: olyan rekordokból áll, amelyeknél **ismerjük az
osztály címkét**. A tanuló adatállományt arra használjuk, hogy egy
osztályozó **modellt építsünk.**

**Teszt adatállomány**: Korábban nem használt rekordok **címkézett**
teszt adatállományát használjuk a **modell** jóságának
**kiértékelésére**

**Alkalmazás:** Az osztályozási modellt olyan **új rekordokra**
alkalmazzuk, amelyeknél **ismeretlen az osztály** címke.

pl. A daganatos sejtek előrejelzése: jó vagy rossz indulatú; Hitelkártya
tranzakciók osztályozása: legális vagy csalás; Újsághírek
kategórizálása: üzlet, időjárás, szórakozás, sport stb.

**Osztályozási módszerek**

**-Döntési fák**

-Szabály alapú módszerek

-Memória alapú módszerek (legközelebbi *k-társ*)

**-Logisztikus regresszió**

-Neurális hálók

-Naív Bayes módszer és Bayes hálók

-Vektorgépek: SVM

**Döntési fa alapú következtetés**

--Hunt algoritmusa (az egyik legkorábbi)

--CART (Classification & Regression Trees \--osztályozási és regressziós
fák)

--ID3 (Interaction Detection), C4.5

--AID, CHAID (Automatic Interaction Detection, Chi-Square based AID)

--SLIQ, SPRINT

**Hunt**

Legyen ***D~t~*** **a tanító rekordok halmaza** a *t* csúcspontban.

-- Ha *D~t~* csak olyan rekordokat tartalmaz, amelyek **ugyanahhoz az
*y~t~* osztályhoz tartoznak**, akkor a *t* csúcspont **címkéje legyen
*y~t~ . ***

-- Ha *D~t~* **üres** halmaz, akkor a *t* levél kapja az *y~d~*
**default** címkét.

-- Ha *D~t~* **egynél több osztályból** tartalmaz rekordokat, akkor egy
attribútum szerinti teszt alapján **osszuk fel a rekordok** halmazát
kisebb **részhalmazokra**. Majd **rekurzívan** alkalmazzuk az eljárást
minden kapott részhalmazra.

**Mohó stratégia**

Vágjuk **részekre a rekordok halmazát** egy **attribútum szerinti**
teszt alapján egy alkalmas **kritériumot optimalizálva.**

**Szempontok**

--Hogyan vágjuk részekre a rekordokat?

-Hogyan határozzuk meg az attributumok szerinti teszt feltételeket?

-Hogyan határozzuk meg a legjobb vágást?

--Mikor álljunk le a vágással?

**Hogyan határozzuk meg a tesztfeltételt?**

Függ az attribútumok **típusátó**l:

--névleges, (= ≠)

--sorrendi, (\< \>)

--folytonos (különbségi, hányados).

Függ attól, hogy **hány részre** vágunk:

--két részre, ágra (bináris) vágás,

--több részre, ágra vágás.

**Vágás névleges attribútum alapján**

**Több részre vágás**: Annyi részt használjunk **amennyi különböző
érték** van.

**Bináris vágás**: Osszuk az értékeket **két részre**. Az optimális
partíciót találjuk meg.

**Vágás sorrendi attribútum alapján**

**Több részre vágás**: Annyi részt használjunk **amennyi különböző
érték** van.

**Bináris vágás**: Osszuk az értékeket **két részre**. Az optimális
partíciót találjuk meg.

**Vágás folytonos attribútum alapján**

Többféle módon kezelhető:

**-Diszkretizáció**, hogy **sorrendi** kategorikus attribútumot
állítsunk elő

-statikus -- egyszer, **kezdéskor** diszkretizálunk,

> -dinamikus -- a tartományokat kaphatjuk **egyenlő** hosszú v. egyenlő
> gyakoriságú **intervallumokra** való beosztással, illetve
> klaszterosítással.

--**Bináris döntés**: (A \< v) vagy(A ≥ v)

-Tekintsük az **összes lehetséges** vágást és találjuk meg a legjobbat.

-Számításigényes lehet.

**Mi lesz a legjobb vágás?**

Mohó megközelítés:

-- A **homogén** osztály-eloszlást eredményező csúcspontokat
preferáljuk.

**Szennyezettségi mérőszámra** van szükségünk:

-Nem homogén, nagyon szennyezett

-Homogén, kicsit szennyezett

**\
**

**Szennyezettség mérése**

Gini index

Entrópia -- (Rendezettlenségi mérték)

Téves osztályozási hiba

**1. Gini index**

Gini index egy t csúcspontban

$$G(t) = 1 - \sum_{j}^{}\left\lbrack \text{p\ }\left( \text{j\ } \middle| \text{\ t} \right) \right\rbrack^{2}$$

(p( j \| t) a *j* osztály relatív gyakorisága a *t* csúcspontban).

-- A maximum *(1 - 1/n~c~)* amikor a rekordok **egyenlően oszlanak** meg
az osztályok között, ahol *n~c~* az osztályok száma (legkevésbé hasznos
információ).

-- A minimum ***0.0*** amikor minden rekord **ugyanahhoz az osztályhoz**
tartozik (leghasznosabb információ).

**Vágás a Gini index alapján**

A **CART,** SLIQ, SPRINT algoritmusok használják.

Ha **a *t* csúcspontot** (szülő) ***k* részre** (gyerekek) osztjuk fel,
akkor a **vágás jóságát** az alábbi képlettel számoljuk:

$$G_{vágás} = \sum_{i = 1}^{k}{\frac{n_{i}}{n}G(i)}$$

ahol *n*~i~= rekordok száma az *i*--edik gyereknél,

*n=* rekordok száma a *t* csomópontban,

*G(i)* = az *i*-edik gyerek Gini indexe.

**Gini index bináris attribútumokra**: Két ágra vágás, Az ágak
**súlyozásának** hatása: minél nagyobb és tisztább ágakat keresünk.

**Gini index diszkrét attribútumokra**: Minden **különböző vágó
értékre** határozzuk meg az egyes osztályok előfordulási
**gyakoriságát** az egyes ágakra. Használjuk a gyakorisági mátrixot a
döntésnél.

**Gini index folytonos attribútumokra:** Használjunk egy
**értéken alapuló bináris döntéseket**.

Számos lehetséges vágó érték: Lehetséges vágások száma = Különböző
értékek száma

Mindegyik **vágó értékhez** tartozik egy **gyakorisági mátrix:** Az ágak
mindegyikében számoljuk össze az A \<v és A ≥ v osztályok
**gyakoriságait.**

Heurisztika a legjobb v megtalálására:

-- Minden *v*-re fésüljük át az adatbázist a gyakorisági mátrix
meghatározására és számoljuk ki a **Gini indexet.**

-- Numerikusan nem hatékony! (Sok ismétlés)

**Hatékony számolási algoritmus**: mindegyik attribútumra

-- **Rendezzük** az attribútumot értékei mentén.

-- Lineárisan végigfésülve ezeket az értékeket mindig frissítsük a
**gyakorisági mátrixot** és számoljuk ki a **Gini indexet.**

-- Válasszuk azt a vágó értéket, amelynek **legkisebb a Gini indexe.**

**2. Entrópia alapú vágási kritérium (C4.5 használja)**

Entrópia (rendezetlenségi fok) a *t* csúcsban:

$$E(t) = - \sum_{j}^{}{p\left( j \middle| t \right)\log_{2}}p(j|t)$$

(ahol *p( j \| t)* a *j*-edik osztály relatív gyakorisága a *t*
csúcsban).

--Egy csúcs **homogenitását** méri.

> -Maximuma *log*~2~*n*~c~, amikor a rekordok **egyenlően** oszlanak meg
> az osztályok között, ahol *n*~c~ az osztályok száma (legrosszabb
> eset).

-Minimuma *0.0*, amikor **minden rekord egy osztályba** tartozik
(legjobb eset).

--Az entrópia számolása hasonló a Gini index számolásához.

**Entrópia alapú vágás**

**Információ nyereség** (INY):

$$\text{INY}_{vágás} = E(p) - \left( \sum_{i = 1}^{k}{\frac{n_{i}}{n}E(i)} \right)$$

A t szülő csúcsot *k* ágra bontjuk: *n~i~* a rekordok száma az *i*-edik
ágban

--Az **entrópia csökken** a vágás miatt. Válasszuk azt a vágást,
amelynél a **csökkenés a legnagyobb** (maximalizáljuk a nyereséget).

--Az ID3 és **C4.5** algoritmusok használják.

--Hátránya: olyan **vágásoka**t részesít előnyben, amelyek **sok
kicsi**, de tiszta ágat hoznak létre.

**Nyereség hányados** (NYH):

$$\text{NYH}_{vágás} = \frac{I_{vágás}}{\text{VE}}\ \ \ \ \ \ VE = - \sum_{i = 1}^{k}{\frac{n_{i}}{n}\log\frac{n_{i}}{n}}$$

A *p* szülő csúcsot *k* ágra bontjuk: *n~i~* a rekordok száma az
*i*-edik ágban

-- Az **információ nyereséget** módosítja a **vágás entrópiájával**
(VE). A nagy entrópiájú felbontásokat (sok kis partíció) bünteti!

-- A **C4.5** algoritmus használja.

-- Az információ nyereség hátrányainak kiküszöbölésére tervezték.

**3. Téves osztályozási hiba alapú vágás**

Osztályozási hiba a t csúcsban:

$$H(t) = 1 - maxP(i|t)$$

Egy **csúcspontbeli téves osztályozás hibáját** méri.

-Maximuma *1 -1/n~c~*, amikor a rekordok **egyenlően** oszlanak meg az
osztályok között, ahol *n~c\ ~*az osztályok száma (legrosszabb eset).

-Minimuma *0.0*, amikor minden rekord **egy osztályba** tartozik
(legjobb eset).

**Megállási szabály döntési fáknál**

**Ne osszunk** tovább egy csúcsot, ha minden rekord **ugyanahhoz** az
osztályhoz tartozik.

**Ne osszunk** tovább egy csúcsot, ha minden rekordnak **hasonló
attribútum értékei** vannak.

Korai megállás (később tárgyaljuk).

**Döntési fa alapú osztályozás**

Előnyök: --**Kis költséggel** állíthatóak elő.

--Kimagaslóan **gyors** **új** rekordok osztályozásánál.

--A kis méretű fák könnyen interpretálhatóak.

--Sok egyszerű adatállományra a pontosságuk **összemérhető** más
osztályozási módszerekével.

**C4.5**

Egyszerű, **egy mélységű keresés**.

**Információ nyereséget használ.**

Minden csúcsnál rendezi a folytonos attribútumokat.

Az összes adatot a memóriában kezeli.

Alkalmatlan nagy adatállományok kezelésére.

--Memórián kívüli rendezést igényel (lassú).

**Az osztályozás gyakorlati szempontjai**

Alul-és túlillesztés

Hiányzó értékek

Az osztályozás költsége

**1. Túlillesztés**

A túlillesztés döntési fák esetén azt eredményezheti, hogy a fa
**szükségtelenül nagy** (összetett) lesz.

A tanítás hibája nem ad jó becslést arra hogyan fog működni a fa új
rekordokra.

A hiba becslésére új módszerek kellenek.

**Az általánosítási hiba becslése**

**Behelyettesítési hiba**: hiba **a tanító** állományon(∑e(t) )

**Általánosítási hiba**: hiba **a teszt** állományon(∑e'(t))

Módszerek az általánosítási hiba becslésére:

--**Optimista megközelítés**: e'(t) = e(t) (az entrópia(hom.) legyen
egyenlő a tanító és a tesztállományon)

--**Pesszimista megközelítés:**

-Minden levélre: e'(t) = (e(t)+0.5)

-Teljes hiba: e'(T) = e(T) + N × 0.5 (N: levelek száma)

-Egy 30 levelű fára 10 tanítási hiba mellett (1000 rekord): Tanítási
hiba= 10/1000 = 1%

Általánosítási hiba= (10 + 30 × 0.5)/1000 = 2.5%

--**Hiba csökkentés tisztítással** (REP--reduced error pruning):

-használjunk egy ellenőrző adatállományt az általánosítási hiba
becslésére.

**Occam borotvája**

Két **hasonló általánosítási hibájú modell** esetén az **egyszerűbbet**
részesítjük előnyben a bonyolultabbal szemben. Bonyolult modelleknél
nagyobb az esélye annak, hogy az csak véletlenül illeszkedik az
adatokban lévő hiba miatt. Ezért figyelembe kell venni a modell
**komplexitását** amikor kiértékeljük.

**Túlillesztés kezelése**

Előtisztítás

-Állítsuk le az algoritmust mielőtt a fa teljes lesz

Utótisztítás

-Építsük fel a fát, metsszük alulról felfelé, ha javul azt
általánosítási hiba, a metszett részt helyettesítjük egy levéllel.

-MDL elvet is használhatjuk

**2. Hiányzó attribútum értékek kezelése**

--Hogyan számoljuk **a szennyezettségi** mutatókat?

--Hogyan oszlanak el a hiányzó értékeket tartalmazó rekordok a gyerek
csúcsok között?

--Hogyan osztályozzuk a hiányzó értékeket tartalmazó teszt rekordokat?

**További szempontok**

Adat-töredezettség

Keresési stratégiák

Kifejezőképesség

Fa ismétlődés

**1. Adat-töredezettség**

A rekordok száma egyre kevesebb lesz ahogy lefelé haladunk a fában.

A **levelekbe eső rekordok** száma **túl kevés** lehet ahhoz, hogy
statisztikailag szignifikáns döntést hozzunk.

**2. Keresési stratégiák**

Az (egy) **optimális döntési fa** megtalálása NP-nehéz feladat.

Az eddig bemutatott algoritmusok mohó, fentről lefelé haladó rekurzív
partícionáló stratégiák, melyek elfogadható megoldást eredményeznek.

**3. Kifejezőképesség**

A döntési fa **kifejező reprezentációt** ad diszkrét értékű függvények
tanításánál.

**Döntési határ**

Két különböző osztályhoz tartozó szomszédos **tartomány közötti
határvonalat** döntési határnak nevezzük. A döntési határ párhozamos a
tengelyekkel mivel a teszt feltétel egy időben csak egy attribútumot
tartalmaz.

**Ferde döntési fa**

A **teszt feltétel több attribútumot** is tartalmazhat. Kifejezőbb
reprezentáció. Az optimális teszt feltétel megtalálása számítás igényes.

**4. Fa ismétlődés**

**Ugyanaz a részfa** fordul elő **több ágban.**

**Modellek kiértékelése**

**Metrikák** hatékonyság kiértékelésre

**Módszerek** a hatékonyság kiértékelésére

Módszerek modellek **összehasonlítására**

**Metrikák hatékonyság kiértékelésre**

A hangsúly a modellek **prediktív képességén** van, szemben azzal, hogy
milyen gyorsan osztályoz vagy épül a modell, skálázható-e stb.

**Egyetértési mátrix**

+----------+----------------------+-------------------+-------------------+
|          | Előrejelzett osztály |                   |                   |
+==========+======================+===================+===================+
| Aktuális |                      | Osztály=Igen      | Osztály=Nem       |
|          |                      |                   |                   |
| osztály  |                      |                   |                   |
+----------+----------------------+-------------------+-------------------+
|          | Osztály=Igen         | TP: igaz pozitív  | FN: hamis negatív |
+----------+----------------------+-------------------+-------------------+
|          | Osztály=Nem          | FP: hamis pozitív | TN: igaz negatív  |
+----------+----------------------+-------------------+-------------------+

**Pontosság -** Leggyakrabban használt metrika

Pontosság=$\frac{TP + TN}{TP + TN + FP + FN}$

**3. Költségmátrix**

+----------+----------------------+---------------+--------------+
|          | Előrejelzett osztály |               |              |
+==========+======================+===============+==============+
| Aktuális | C(i\|j)              | Osztály=Igen  | Osztály=Nem  |
|          |                      |               |              |
| osztály  |                      |               |              |
+----------+----------------------+---------------+--------------+
|          | Osztály=Igen         | C(Igen\|Igen) | C(Nem\|Igen) |
+----------+----------------------+---------------+--------------+
|          | Osztály=Nem          | C(Igen\|Nem)  | C(Nem\|Nem)  |
+----------+----------------------+---------------+--------------+

*C(i\|j):* **a téves osztályozás költsége**, a *j* osztályba eső
rekordot az *i* osztályba soroljuk

**Módszerek hatékonyság kiértékelésére**

Egy modell hatékonysága a tanító algoritmus mellett más faktoroktól is
függhet:

--**osztályok eloszlása,**

--a **téves osztályozás** költsége,

--a tanító és tesz adatállományok **mérete.**

**Tanulási görbe**

A tanulási görbe mutatja hogyan változik **a pontosság** a
**mintanagyság függvényében**.

Mintavételi ütemterv szükséges a tanulási görbe elkészítéséhez.

**Becslési módszerek**

**Felosztás**: Tartsuk fenn a 2/3 részt tanításra, az 1/3 részt
tesztelésre.

**Véletlen részminták:** Ismételt felosztás

**Keresztellenőrzés**: Osszuk fel az adatállományt *k* diszjunkt
részhalmazra. Tanítsunk *k-1* partíción, teszteljünk a fennmaradón.
Hagyjunk ki egyet: *k=n*(diszkriminancia analízis).

**Rétegzett mintavétel**: Felül-vagy alulmintavételezés

**Bootstrap**: Visszatevéses mintavétel

**\
Módszerek modellek összehasonlítására**

**ROC** (Receiver Operating Characteristic)

Vevő oldali működési jellemző. Az 50-es években fejlesztették ki a
jelfeldolgozás számára zajos jelek vizsgálatára.

A **pozitív találatok** és a **hamis riasztások** közötti
**kompromisszumot** írja le.

A ROC görbe a IP (igaz-pozitív) (y tengely) eseteket ábrázolja a HP
(hamis pozitív) (x tengely) függvényében.

Minden **osztályozó hatékonysága** reprezentálható **egy ponttal** a ROC
görbén.

--Az algoritmusbeli küszöbértéket megváltoztatva a mintavételi eloszlás
vagy a költség-mátrix módosítja a pont helyét.

**ROC görbe**

Egy dimenziós adatállomány, amely **két osztályt** tartalmaz (pozitív és
negatív).

Minden x \> t pontot pozitívnak osztályozunk, a többi negatív lesz. (t:
valamilyen határérték)

(IP,HP):

-(0,0): mindenki a negatív osztályba kerül

-(1,1): mindenki a pozitívosztályba kerül

-(1,0): ideális

**Diagonális vonal (átló)**: Véletlen találgatás, A diagonális vonal
alatt: Az előrejelzés a valódi osztály ellentéte

**Hogyan szerkesszünk ROC görbét**

Alkalmazzunk egy olyan osztályozót, amely minden rekordra meghatározza a
P(+\|A) poszterior valószínűséget.

Rendezzük a rekordokat P(+\|A) szerint csökkenően.

Válasszuk küszöbnek minden egyes különböző P(+\|A) értéket.

Minden küszöb értéknél számoljuk össze: IP, HP, IN, HN.

**IP ráta**, IPR = IP/(IP+HN)

**HP ráta**, HPR = HP/(HP + IN)

A görbe alatti terület (**AUC**) egy egyszerű mutató a
**kiértékelésre.**

**Szignifikancia vizsgálat + Konfidencia intervallum vizsgálat a
modellek pontosságának összehasonítására.**

## 4. Osztályozási módszerek: szabály alapú osztályozók, naív Bayes módszer, k legközelebbi szomszéd.

**Osztályozási szabályok (Szabály alapú osztályozók)**

**„Ha...akkor..."** szabályok összességével osztályozzuk a rekordokat.

Szabály: (*Feltétel*) *y*

ahol

*-Feltétel* **attributumok konjunkciója**

-y **osztály címke**

Baloldal: a szabály **feltétele**, előzménye

Jobboldal: a szabály **következménye**

Példák osztályozási szabályokra:

-(Vértípus=Meleg) Ʌ (Tojásrakás=Igen) Madarak

-(Adózott jövedelem\< 50K) Ʌ (Visszatérítés=Igen) Adóelkerülés=Nem

**Osztályozási szabályok alkalmazása**

Az ***r*** szabály **lefedi** az **x** esetet, ha az eset **attribútumai
kielégítik a szabály feltételeit.**

**Lefedettség**

Azon **rekordok aránya**, amelyek **kielégítik a szabály feltételét.**

**Pontosság**

Azon **rekordok aránya**, amelyek egyaránt **kielégítik a szabály
feltételét** és **következményét.**

**Osztályozási szabályok jellemzése**

**Teljesen kizáró szabályok**

--Egy osztályozó teljesen kizáró szabályokból áll, ha a **szabályok
függetlenek** egymástól (a feltételek metszete üres).

--Minden rekordot legfeljebb egy szabály fed le.

**Kimerítő szabályok**

--Egy osztályozó **kimerítő lefedés**, ha az attribútum **értékek**
minden **lehetséges kombinációját** tartalmazza **a feltételekben.**

--**Minden rekordot lefed legalább egy szabály.**

**Döntési fáktól a szabályokig**

A szabályok teljesen **kizáróak** és **kimerítőek**. A szabály halmaz
pontosan annyi információt tartalmaz, mint a fa. (közvetett módszer)

**Szabályok egyszerűsítése**

Visszatérítés és házas helyett csak a házast nézem, mert így is ugyan
oda jutok

**Az egyszerűsítés hatása**

A szabályok már **nem** lesznek **teljesen kizáróak.**

--Egy rekord egynél több szabályt is kiválthat.

--Megoldás?

**-Szabályok rendezése**

-Rendezetlen szabályok--használjunk szavazási sémákat

A szabályok már **nem** lesznek **kimerítőek.**

--Egy **rekord** **egyetlen szabályt sem** vált ki.

--Megoldás?

-Használjunk egy **alapértelmezett osztályt.**

**Rendezett szabály halmazok**

A szabályokat prioritásuk szerint **sorba rendezzük.**

-- Egy rendezett szabályhalmazt **döntési listának** nevezünk.

Egy teszt rekordot inputként kap az osztályozó.

-- A legelső osztályhoz rendeljük, amelyet kivált.

-- Ha egyetlen szabályt sem vált ki, akkor az alapértelmezett osztályba
kerül.

**\
**

**Szabály rendező sémák**

Szabály alapú rendezés

--Az egyedi szabályokat **minőségük** alapján rendezzük.

Osztály alapú rendezés

--Az egy **osztályhoz tartozó** szabályok együtt fordulnak elő.

**Osztályozási szabályok építése**

**Közvetlen módszerek:**

-Szabály kinyerés **közvetlenül az adatokból.**

-Példák: RIPPER, CN2, Holte 1R módszere.

**Közvetett módszerek:**

-Szabály kinyerés **más osztályozási módszerekből** (pl. döntési fák,
neurális hálók stb.).

-Példa: C4.5 szabályok.

**Közvetlen módszer: Szekvenciális lefedés**

1.Induljunk ki az **üres szabályból.**

2.Hozzunk létre egy **szabályt** a Learn-One-Rule függvény segítségével.

3.**Távolítsuk el** azokat a tanító rekordokat, amelyeket **lefed a
szabály.**

4.Ismételjük a (2) és (3) lépést ameddig a megállási kritérium nem
teljesül.

**A szekvenciális lefedés szempontjai**

Szabály építés

Eset kizárás

Szabály kiértékelés

Leállási kritérium

Szabály tisztítás

**Szabály építés**

Két általános stratégia

**1. CN2** algoritmus:

--Induljunk ki az **üres szabályból**: {}.

--Bővítsük úgy, hogy közben az **entrópiát minimalizáljuk**: {A}, {A,B},
...

--Határozzuk meg a szabály **következmény**ét a szabály által lefedett
esetek többségi osztályát véve.

**2. RIPPER** algoritmus:

--Induljunk ki az **üres szabályból** : {} =\> osztály.

--Bővítsük úgy, hogy a FOIL-féle **információ nyereséget
maximalizáljuk:**

-R0: {} =\> osztály (kezdeti szabály)

-R1: {A} =\> osztály (szabály a bővítés után)

-Nyereség(R0, R1) = t \[ log (p1/(p1+n1)) --log (p0/(p0 + n0)) \],

-ahol t: R0 és R1 által lefedett pozitív esetek száma,

> p0: R0 által lefedett pozitív esetek száma,
>
> n0: R0 által lefedett negatív esetek száma,
>
> p1: R1 által lefedett pozitív esetek száma,
>
> n1: R1 által lefedett negatív esetek száma.

**Eset kizárás**

Miért van szükség eset kizárásra?

--Különben a **következő szabály megegyezik az előzővel.**

Miért töröljünk pozitív eseteket?

--Biztosítsuk a következő **szabály különbözőségét.**

Miért töröljünk negatív eseteket?

--Megelőzzük a szabály **pontosságának alulbecslését.**

**Szabály kiértékelés**

Mérőszámok:

**Pontosság**=$\ \frac{n_{c}}{n}$

**Laplace**=$\frac{n_{c} + 1}{n + k}$

**M-becslés**=$\frac{n_{c} + kp}{n + k}$

*n :* a szabály által lefedett esetek száma

*n~c~ :* a szabály által lefedett pozitív esetek száma

*k :* osztályok száma

*p :* a pozitív eset apriori valószínűsége

**Leállási feltétel**

Számoljuk ki a nyereséget. Ha a **nyereség nem szignifikáns**, akkor
dobjuk el az új szabályt.

**Szabály tisztítás**

Hasonló döntési fák utótisztításához.

**Hiba csökkentés** tisztítással:

-Hagyjunk el a szabályból egy kifejezést.

-Hasonlítsuk össze a tisztítás előtti és utáni hibát az ellenőrző
adatállományon.

\-**Ha a hiba javul, akkor tisztítsunk a kifejezés elhagyásával.**

**A közvetlen módszer vázlata**

Építsünk egy **egyszerű szabályt.**

**Távolítsunk el** eseteket a szabály alapján.

**Egyszerűsítsük** a szabályt (ha szükséges).

**Adjuk hozzá** a szabályt az aktuális szabály halmazhoz.

**Ismételjük** a fenti lépéseket.

**Közvetlen módszer: RIPPER**

**Bináris** feladat esetén válasszuk **pozitív osztálynak** az egyik és
**negatív** osztálynak a másik osztályt.

--Tanítsunk **szabályokat a pozitív** osztályra.

--Legyen a **negatív** osztály az **alapértelmezett** osztály.

**Több osztályos** feladat esetén:

**--Rendezzük** az osztályokat növekvő **osztály--gyakoriság
szerint**(azoknak az eseteknek az aránya, melyek egy osztályhoz
tartoznak).

--Először tanítsunk **egy szabály** halmazt a **legkisebb osztályra**,
kezeljük a maradékot negatív osztályként.

--Ismételjük meg a **következő legkisebb** osztállyal, mint **pozitív
osztály.**

**Szabály építés:**

--Induljunk ki **az üres szabályból.**

--Bővítsük addig míg a FOIL **információ nyereség javul.**

--**Álljunk** meg amikor a szabály tovább már **nem fedi le a negatív
eseteket.**

--Közvetlenül tisztítsuk a szabályt **járulékos hiba tisztítással.**

--A tisztítás mérőszáma: *v = (p-n)/(p+n)*

p: a szabály által lefedett pozitív esetek száma az ellenőrző
adatállományban,

n: a szabály által lefedett negatív esetek száma az ellenőrző
adatállományban.

--Tisztítási módszer**: töröljük** a **feltételek** olyan véges
sorozatát, amely **maximalizálja *v*-t.**

**Szabály halmaz építése:**

--Használjunk **szekvenciálisan lefedő algoritmust.**

-Keressük meg azt a **legjobb szabályt**, amely lefedi a pozitív esetek
aktuális halmazát.

-Elimináljuk a szabály által lefedett pozitív és negatív eseteket.

--Mindig mikor egy szabállyal **bővítjük** a szabály halmazt számoljuk
ki az **új leíró hosszt.**

> -Álljunk le az új szabály hozzáadásával, ha annak leíró hossza *d*
> bittel nagyobb, mint az eddig kapott legkisebb leíró hossz.

**Optimalizáljuk a szabályhalmazt:**

--Az ***R*** szabályhalmaz minden *r* szabályára

-Tekintsünk 2 alternatív szabályt:

> --**Helyettesítő** szabály(r\*): építsünk új szabályt elölről.
>
> --**Módosított** szabály (r'): bővítsünk az *r* kiterjesztésével.

-Hasonlítsuk össze az *r* szabályhalmazt az *r\** és *r'*
szabályhalmazokkal.

-Válasszuk azt a szabályhalmazt, amely minimális lesz az MDL elv
alapján.

--Ismételjük a szabály generálást és optimalizálást a fennmaradó pozitív
esetekre.

**\
**

**Közvetett módszerek: C4.5szabályok**

**Nyerjünk ki szabályokat** egy tisztítatlan (teljes) döntési fából.

Minden **r: A y** szabályra

--Tekintsünk egy *r': A'* *y* **alternatív szabályt**, ahol *A'*-t úgy
kapjuk, hogy *A*-ból **törlünk egy kifejezést.**

--**Hasonlítsuk** össze az *r* és az összes *r'* pesszimista **hiba
rátáját.**

--**Tisztítsunk** amennyiben egy *r'*-nek kisebb a pesszimista hiba
rátája.

--Ismételjük amíg már nem tudjuk javítani az általánosítási hibát.

A szabályok rendezése helyett **rendezzük szabályok részhalmazait**
(osztály rendezés).

--Minden részhalmaz szabályoknak egy olyan összessége, melynek
**következménye ugyanaz**(osztály).

--Számoljuk ki minden részhalmaz **leíró hosszát.**

-Leíró hossz= L(error) + g L(model),

> -g egy olyan paraméter, amely figyelembe veszi a szabályhalmazban lévő
> redundáns attribútumokat (alapérték= 0.5).

**Osztályozási szabályok előnyei**

Legalább annyira **kifejezőek** mint a **döntési fák.**

**Könnyen interpretálhatóak.**

Könnyen **generálhatóak.**

**Gyorsan** osztályozhatóak általuk az új esetek.

Hatékonyságuk **összevethető** a döntési fákéval.

**Bayes osztályozó**

Egy **valószínűségszámítási módszer** **osztályozási problémák
megoldására.**

Feltételes valószínűség:

P(C\|A) =$\ \frac{P(A,C)}{P(A)}$ P(A\|C) =$\ \frac{P(A,C)}{P(C)}$

**Bayes tétel:**

P(C\|A) =$\ \frac{P(A|C)P(C)}{P(A)}$

pl. Agyhártyagyulladás miatti nyakfájás 50% valséggel van;
agyhártyagyulladás valsége 1/50 000; nyakfájás valsége 1/20. Ha fáj a
nyakam mennyi a valsége hogy agyhártyagyulladásom van?P(M\|S)=
$\frac{0.5*1/50000}{1/20} = 0.0002$

Tekintsük **valószínűségi változónak** az **összes attribútumot** és a
**cél** (osztály) **változót.**

Legyen **adott egy rekord** az *(A~1~, A~2~,...,A~n~)* attribútum
értékekkel

--A cél a ***C* osztályozó** változó **előrejelzése.**

--Azt az értékét keressük *C*-nek, amely **maximalizálja *P****(C\|
A~1~, A~2~,...,A~n~ )*-t.

Tudjuk-e közvetlenül becsülni *P(C\| A~1~, A~2~,...,A~n~ )-t* az
adatokból?

**Megközelítés:**

--Számoljuk ki a **P(C \| A~1~, A~2~, ..., A)** poszteriori
valószínűséget minden C értékre a **Bayes tétellel.**

--Válasszuk azt a **C értéket**, amely **maximalizálja** P(C \| A~1~,
A~2~, ..., A~n~)-t.

--**Ekvivalens** annak a **C** értéknek megtalálásával, mely
maximalizálja P(A~1~, A~2~, ..., A~n~\|C) P(C)-t.

Hogyan becsüljük P(A~1~, A~2~, ..., A~n~ \| C )-t?

Tételezzünk fel **függetlenséget** az **A~i~ attributumok
között** ha az osztály adott:

--P(A~1~, A~2~, ..., A~n~ \|C) = P(A~1~\| C~j~) P(A~2~\| C~j~)...
P(A~n~\| C~j~)

--Az P(A~i~\| C~j~) valószínűséget becsülhetjük minden *A~i\ ~*és
*C~j\ ~*esetén.

--Egy új rekord a **C~j~ osztályba kerül** ha a P(C~j~) ∏P(A~i~\| C~j~)
**maximális.**

**Naív Bayes**

**Feltételezi**, hogy az **összes attribútum között feltételes
függetlenség van.** (karhossz -- olvasási készség)

Robusztus izolált hibás pontokra.

Kezeli a **hiányzó értékeket** a valószínűségek becslésénél ezen esetek
**figyelmen kívül hagyásával.**

Robusztus az **irreleváns attribútumokra.**

A **függetlenségi feltétel nem teljesül** egyes attribútumokra.

--Használjunk más módszereket, Bayes hálók (Bayesian Belief
Networks,BBN).

**Eset alapú osztályozók**

Letároljuk a tanító rekordokat. A tanító rekordokat használjuk az új
esetek osztályainak **előrejelzésére.**

pl.

Rote tanuló algoritmusa: A teljes tanító adatállományt memorizálja, és
csak akkor hajtja végre az osztályozást, ha az új rekord attributum
értékei pontosan illeszkednek egy tanító esetre.

Legközelebbi szomszéd: Használjuk a k ,,legközelebbi" pontot
(legközelebbi szomszédok) az osztályozás végrehajtására.

**Legközelebbi szomszéd osztályozók**

**def.:** Az **x** rekord **k legközelebbi szomszédja** azok a rekordok,
melyek **távolsága** x-től a k **legkisebb távolság.**

**Alapgondolat**: Ha valami úgy totyog, mint egy kacsa, úgy hápog, mint
egy kacsa, akkor az valószínűleg egy kacsa.

Három dolog szükséges

--**Rekordok** egy halmaza

--A rekordok közötti **távolság** számolására szolgáló metrika

--A ***k*** szám, a meghatározandó legközelebbi szomszédok száma

Egy **új rekord** osztályozása:

--Számoljuk ki a **távolságot** a többi tanító rekordtól.

--Határozzuk meg a *k* **legközelebbi szomszédot**.

--Használjuk a **legközelebbi szomszédok osztálycimkéit** az új rekord
besorolására (pl. többségi szavazást véve).

Számoljuk ki két pont **távolságát**:

**--Euklideszi távolság**: d(p,q)=
$\sqrt{\sum_{i}^{}\left( p_{i} - q_{i} \right)^{2}}$

> -baj vele: sok dimenziós adatok, dimenzió probléma; a természetes
> szemlélettel ellenkező eredményt is adhat

A legközelebbi szomszédok alapján határozzuk meg az osztályt:

--Vegyük a **többségi osztályt** a *k* szomszéd közül.

--**Súlyozzuk** a szavazatokat a **távolság**nak megfelelően.

-súly: w = 1/d^2^

A ***k* érték megválasztása**:

--Ha *k* túl **kicsi**, akkor a módszer **érzékeny a hibás** rekordokra.

--Ha *k* túl **nagy**, akkor a **szomszédság** más osztálybeli pontokat
is tartalmazhat.

**Skálázási szempontok:**

--Az attributumokat **átskálázhatjuk** így előzve meg azt, hogy egy
**attributum dominálja** a távolságot.

--Példa:

-Egy személy magassága 1.5m és 1.8m között van.

-Egy személy súlya 90lb és 300lb között van.

-Egy személy bevétele \$10K és \$1M között van.

**Hátrányok:**

A legközelebbi szomszéd osztályozók lusta tanuló algoritmusok.

--**Nem építenek** explicit **modelleket.**

--Mások, mint a mohó tanító algoritmusok, ld. döntési fák és
osztályozási szabályok.

--Az **új rekordok** osztályozása viszonylag **költséges.**

pl. PEBLS, ahol k=1

## 5. Osztályozási módszerek: mesterséges neuron hálók, támaszvektor gépek (SVM), logisztikus regresszió, együttes osztályozók.

**Mesterséges neurális hálók (ANN)**

A **modell** egymással **összekötött** **csúcsok** és **súlyozott élek**
együttese.

Az **output** csúcs **összegzi** az hozzátartozó **input
értékeket** az éleken lévő **súlyok szerint.**

Vessük össze az **output** csúcsban kapott értéket egy *t* **küszöb
számmal.**

Egy MNH **tanítása** a **neuronjai súlyának** meghatározását jelenti.

(paraméterek = súlyok )

**(Perceptron modell)**

Vannak **bemenő** és **kimenő** adatok. A bemenő adatok egy **fekete
dobozba** kerülnek, ahol **súlyok** rendelődnek hozzá, ezek alapán
létrejön egy **modell**, a megad egy **kimeneti** értéket. (nincs
rejtett réteg)

Aztán ha egy **ismeretlen kimeneti értékű** inputunk van, akkor a modell
segítségével meg tudjuk mondani az output értéket.

(Általánosan **aktivációs függvény**nek hívhjuk, amik a rétegek között a
neuronokat tartalmazzák.)

akt fv. pl. ReLu

**Algoritmus MNH tanítására**

Inicializáljuk a (w~0~, w~1~, ..., w~k~) **súlyokat.**

**Módosítsuk úgy a súlyokat**, hogy az MNH outputja minél jobban
**egyezzen** meg a **tanító** esetek **osztály címkéivel.**

-Célfüggvény:
E=$\sum_{i}^{}\left\lbrack Y_{i} - f\left( w_{i},X_{i} \right) \right\rbrack^{2}$

--Határozzuk meg azon ***w*~i~ súlyokat**, amelyek **minimalizálják** a
fenti célfüggvényt.

-Pl. hiba visszacsatolás algoritmusa (error back propagation).

(Bemeneti réteg + **rejtett rétegek** + kimeneti réteg)

Sok rejtett réteg mélytanulásnál van. (pl. képfeldolgozás)

**Támasz vektorgépek (SVM)**

Keressünk olyan **hipersíkot (döntési határ**), amely **elválasztja** az
adatokat. egyenestlin. szeparálható

Végtelen sok megoldás, de melyik a jobb?

Keressük azt a hipersíkot, mely **maximalizálja a margót** (az
egyeneshez a **legközelebbi pont távolságát** minimalizáljuk)

Ez kényszerfeltétel melletti optimalizációs feladat.

-- Numerikus módszerek (pl. kvadratikus programozás).

**Nemlineáris támasz vektorgépek**

(Ha a **döntési határ nem lineáris**. Bevezetünk **lötyögő változókat**
és beépítjük a célfüggvénybe.)

Transzformáljuk az adatokat egy **magasabb dimenziójú** térbe (kernel
trükk). (hiper sík nagyobb dimbe)

**Osztályozás regresszió útján**

Ahelyett, hogy egy rekord osztályát jeleznénk előre próbáljuk meg
**előrejelezni az osztály valószínűségét,** amely már egy
**folytonos mennyiség**.

Egy folytonos mennyiség előrejelzését **regressziós feladat**nak
nevezzük

**Általános megközelítés**: találjunk egy olyan **folytonos függvényt**,
amely jól modellezi (illeszkedik) a folytonos pontfelhőre.

**Lineáris regresszió**

Egy adott adatállomány, i.e.,{ (𝑥~1~,𝑦~1~),...,(𝑥~𝑛~,𝑦~𝑛~)}, esetén
találjunk egy olyan **lineáris függvényt**, amely adott 𝑥~𝑖~ vektor
esetén az 𝑦~𝑖~ értéket úgy jelzi előre mint 𝑦~𝑖~′=𝑤^𝑇^𝑥~𝑖~

--Találjunk egy olyan **𝑤 súlyvektort**, amely minimalizálja a
**négyzetösszeg hibát:**

$$\sum_{i}^{}\left( y_{i}^{'} - y_{i} \right)^{2}$$

--A probléma megoldására számos módszer ismert.

**Logisztikus regresszió**

Találjunk egy olyan **w vektort**, amely **maximalizálja** a
**megfigyelt adatok valószínűségét.**

Lineáris regresszió a **log-odds hánydoson.**

Előállítja az **osztályhoz való tartozás valószínűségének becslését**,
amely gyakran hasznos és egy pontosabb leírását adja a döntés
megbízhatóságának.

A **súlyok** hasznosak lehetnek a **jellemzők fontosságának
megértésében.**

Viszonylag **nagy méretű** adatállományokon is működik.

**Gyors** az **alkalmazásokon** mivel az osztályok becslése csak a
súlyvektortól függ.

**Együttes módszerek**

**Osztályozók egy halmazát** hozzuk létre a tanító állományon. Egy új
rekord osztályát úgy jelezzük előre, hogy a **sok osztályozó** által
kapott előrejelzéseket **összesítjük.**

**Miért működhet?**

Tegyük fel, hogy adott 25 egyszerű osztályozónk.

--Minden osztályozó hibája ε= 0.35.

--Tegyük fel, hogy az osztályozók **függetlenek.**

--Annak valószínűsége, hogy az együttes osztályozó hibás döntést hoz:
0.06

(Binomiális eloszlás: az egyes osztályozó jól döntött vagy nem)

**Folyamatábrája**

Bemeneti adatok sok (különböző) adatállományt generálaz adatállományokra
egyenként illesztjük a különböző modelleket osztályozókaz osztályozók
eredményeit összesíti többségi szavazás elvével

pl. --Bagging (bootstrap aggregating)

--Boosting (gyorsítás)

**Bagging**

**Visszatevéses mintavétel**. (Egy adatállományból előállítok több
adatállományt, **ismétlődhetnek az elemek**, akár több adatállományba is
vagy egy adatállományba többször)

Minden bootstrap mintán építsünk fel egy osztályozót (pl. döntési fa).

Minden egyes rekordot (1 --1/n)^n^ valószínűséggel választunk ki.

**Boosting (gyorsítás)**

Egy olyan iteratív eljárás, amely a **tanító rekordok eloszlását**
adaptívan **változtatva** a korábban **tévesen osztályozott rekordokra
fókuszál.**

--Kezdetben mind az összes N rekord **egyenlő súlyt** kap.

--A bagging-gel szemben a **súlyok változhatnak** egy iterációs ciklus
befejeztével.

A **rosszul osztályozott** rekordoknak **nő**ni fog a **súlya**. A
**helyesen osztályozott** rekordoknak **csökkenni** fog a súlya.

**AdaBoost**

A s**úlyok** mindig **visszaállnak 1/n-re** ha a közbenső **hiba 50%
fölé** megy és a mintavételi **folyamat megismétlődik.**

## 6. Hasonlóság és távolság. Klaszterezés: definíciók, K-közép módszer és variánsai. A klaszterezés kiértékelése: hasonlósági mátrix, korreláció, SSE, árnyék együttható.

**Hasonlóság (s)**

Két objektum (rekord) **hasonlóságát** méri. Minél **nagyobb** az értéke
annál nagyobb a **hasonlóság.** Általában a \[0,1\] intervallumban veszi
fel az értékeit.

**Távolság (d)**

Két objektum (rekord) **különbözőségét** méri. Minél **kisebb** annál
nagyobb a hasonlóság. A **minimális** távolság általában **0**. A felső
korlát változó.

A **szomszédság** fogalma egyaránt utalhat hasonlóságra és távolságra.

**Távolság (dissimilarity) egyszerű attribútumnál (s+d=1)**

**Névleges**: d = $\left\{ \begin{matrix}
0\ \ \ ha\ p = q \\
1\ \ \ ha\ p \neq q \\
\end{matrix} \right.\ $

**Sorrendi**: d = $\frac{|p - q|}{n - 1}$ n: értékek száma

**Intervallum**: d = $|p - q|$ ( s = -d; s = $\frac{1}{1 + d}$; vagy s =
1 - $\frac{d - min\_ d}{{max\_ d}{- \ min\_ d}}$ )

**Euklideszi távolság**

$$\text{dist}(p,q) = \sqrt{\sum_{k = 1}^{n}\left( p_{k} - \ q_{k} \right)^{2}}$$

A képletben *n* jelöli a dimenziót (attribútumok száma), *p~k~* és
*q~k~* pedig a *k*-adik attribútum értéke (koordinátája) a *p* és *q*
objektumoknak (rekordoknak).

Ha a skálák különbözőek, akkor előbb **standardizálni** kell.

**\
**

**Minkowski távolság**

Az **euklideszi** távolság **általánosítása.**

$$\text{dist}(p,q) = \left( \sum_{k = 1}^{n}\left| p_{k} - \ q_{k} \right|^{r} \right)^{\frac{1}{r}}$$

A képletben *r* paraméter, *n* a dimenzió (attribútumok száma) *p~k~* és
*q~k~* pedig a *k*-adik attribútum értéke (koordinátája) a *p* és *q*
objektumoknak (rekordoknak).

**r=1**: háztömb (Manhattan, taxi, L~1~ norma) távolság.

--Egy ismert példa az ún. Hamming távolság, amely éppen a különböző
bitek száma két bináris vektorban.

**r=2**: euklideszi távolság

r ∞: „szupremum" (L~max~ norma, L~∞~ norma) távolság.

--Két vektor koordinátái közötti különbségek abszolút értékének
maximuma.

Ne tévesszük össze *r* és *n* szerepét, ezek a távolságok minden
dimenzió, azaz *n* mellett értelmezhetőek.

**Mahalanobis távolság**

$$\text{mahalanobis}(p,q) = (p - q)\sum_{}^{- 1}(p - q)^{T}$$

∑ az *X* input adatok kovariancia mátrixa.

**A távolság általános jellemzői**

A különböző távolság fogalmak, pl. euklideszi, néhány jól ismert
jellemzővel bír.

*1. **d(p, q) ≥0*** minden *p* és *q* esetén, továbbá ***d(p, q) = 0***
akkor és csak akkor ha ***p= q*** (**nemnegativitás**),

*2. **d(p, q) = d(q, p**)* minden *p* és *q* esetén (**szimmetria**),

3\. **d*(p, r)* ≤ *d(p, q) + d(q, r) ***minden *p*, *q*, és *r* pontra
(**háromszög egyenlőtlenség**),

ahol *d(p, q)* a *p* és *q* pontok (objektumok) közötti távolságot
jelöli.

Az olyan **távolságot,** amely eleget tesz a fenti tulajdonságoknak
**metrikának** nevezzük.

**\
**

**A hasonlóság általános jellemzői**

A hasonlóságoknak szintén van néhány jól ismert tulajdonsága.

*1. **s(p, q) = 1** (*vagy a maximális hasonlóság) akkor és csak akkor
ha ***p= q*,**

*2. **s(p, q) = s(q, p)*** minden *p* és *q* esetén (**szimmetria**),

ahol *s(p, q)* jelöli a *p* és *q* pontok (objektumok) közötti
hasonlóságot.

**Bináris vektorok hasonlósága**

Gyakran előfordul, hogy objektumoknak, *p* és *q*, csak bináris
attribútumai vannak.

Hasonlóságokat a következő mennyiségek révén definiálhatunk:

M~01~= azon attribútumok száma, ahol p=0 és q=1,

M~10~ = azon attribútumok száma, ahol p=1 és q=0,

M~00~= azon attribútumok száma, ahol p=0 és q=0,

M~11~= azon attribútumok száma, ahol p=1 és q=1.

**Egyszerű egyezés**

SMC = egyezők száma/ attribútumok száma = (M11+ M00) / (M01+ M10+ M11+
M00)

**Jaccard együttható**

J = az 11 egyezések száma/ a nem mindkettő 0 attribútumok száma = (M11)
/ (M01+ M10+ M11)

**Koszinusz hasonlóság**

Ha *d~1~* és *d~2~* két dokumentumot leíró vektor (nemnegatív egész
koordinátájúak), akkor

cos(d~1~,d~2~)=(d~1~ ● d~2~)/\|\|d~1~\|\| \|\|d~2~\|\|,

ahol ● jelöli a skaláris szorzatot \|\|*d*\|\| pedig a *d* vektor
hossza.

**Tanimoto együttható**

A Jaccard együttható általánosítása

A Jaccard együttható módosítása azért, hogy alkalmazható legyen
**folytonos**, illetve **egész** értékű attribútumokra.

--Bináris attribútumok esetén a Jaccard együtthatót kapjuk vissza

**Korreláció**

Az objektumok vagy attribútumok közötti **lineáris kapcsolat erősségét**
méri.

Két objektum (attribútum), p és q, közötti korreláció kiszámításához
először **standardizáljuk** őket, majd **skaláris szorzatot** veszünk

$$p_{k}^{'} = \frac{\left( p_{k} - \overline{p} \right)}{s(p)}$$

$$q_{k}^{'} = \frac{\left( q_{k} - \overline{q} \right)}{s(q)}$$

$$\text{korrel}á\text{ci}ó(p,q) = \ p^{'}{\ ●\ q}^{'}$$

ahol $\overline{p}\ $az átlag, *s(p)* pedig a szórás.

**Hasonlóságok összekapcsolása**

Előfordul, hogy az attribútumok nagyon különböző típusúak viszont egy
átfogó hasonlóságra van szükségünk.

**Hasonlóságok összekapcsolása súlyokkal**

Nem mindig akarjuk az összes attribútumot ugyanúgy kezelni.

--Használjunk w~k~ súlyokat, melyek 0 és 1 közé esnek úgy, hogy az
összegük 1.

**Sűrűség**

A sűrűség alapú csoportosításhoz szükséges a sűrűség fogalmának
tisztázása.

Példák:

--Euklideszi sűrűség= egységnyi térfogatba eső pontok száma

--Valószínűségi sűrűség

--Gráf alapú sűrűség

**Cella alapú euklideszi sűrűség**

Osszuk egyenlő térfogatú téglalap alakú cellákra a tartományt és
definiáljuk a **sűrűséget** úgy, mint amely arányos a **cellákba eső
pontok számával**.

**Középpont alapú euklideszi sűrűség**

A sűrűség egy pontban arányos a pont körüli **adott sugarú környezetbe**
eső pontok számával.

**Mi a klaszterezés (csoportosítás)?**

Találjunk olyan **csoportokat** objektumok egy halmazában, hogy az egy
csoportban lévő objektumok **egymáshoz hasonlóak,** míg a **más
csoportokban** lévők pedig **különbözőek.**

**A klaszterezés alkalmazásai**

**Megértés**: Böngészésnél kapott kapcsolódó dokumentumok csoportjai,
hasonló funkcionalitással bíró gének és fehérjék csoportjai, hasonló
ármozgású részvények csoportjai.

**Összegzés**: Nagy adatállományok méretének csökkentése.

**Mi nem klaszterezés?**

**Felügyelt osztályozás:** Adott egy osztályozó attribútum.

**Egyszerű szegmentáció:** Osszuk fel a diákokat különböző csoportokba a
vezeték nevük alapján ábécé szerint.

**Egy lekérdezés eredményei:** A csoportok egy külső specifikáció
eredményei.

**Gráf partícionálás**: Kölcsönös fontosság vagy együttműködés az
objektumok (rekordok) között, azonban különböző területeken.

**Klaszterezések fajtái**

Egy **klaszterosítás** klaszterek (csoportok) egy halmaza.

**Felosztó klaszterezés:**

--Az objektumok felosztása **nem átfedő** részhalmazokra(klaszterekre)
úgy, hogy minden objektum **pontosan egy** részhalmazban szerepelhet.

**Hierarchikus klaszterezés:**

--**Egymásba ágyazott** klaszterek egy hierarchikus fába szervezett
halmaza.

**Kizáró vagy nem-kizáró**

--A **nem-kizáró** kleszterezésnél a pontok **több klaszterhez** is
tartozhatnak.

--Egy pont, a ,,határ" pont, több osztályt is képviselhet.

**Fuzzy vagy nem-fuzzy**

--A fuzzy klaszterezésnél egy pont az **összes klaszterhez** tartozik 0
és 1 közötti **súllyal.**

--A súlyok összege 1.

--A **valószínűségi klaszterezés** hasonló tulajdonsággal bír.

**Részleges vagy teljes**

--Bizonyos esetekben az adatok **egy részét** akarjuk klaszterezni.

**Heterogén vagy homogén**

--**Nagyon különböző** méretű, alakú és sűrűségű klaszterek.

**Klaszterek típusai**

**Jól elválasztott klaszterek**: Egy klaszter pontoknak olyan
halmaza, hogy a klaszter **bármely pontja közelebb van** (vagy
hasonlóbb) a **klaszter összes további pontjához** mint bármelyik nem
klaszterbeli pont.

**Középpont alapú klaszterek:** Egy klaszter objektumoknak egy
olyan részhalmaza, hogy egy klaszterbeli objektum **közelebb van**
(hasonlóbb)a klaszter **,,középpontjához"**, mint bármelyik más
klaszterközépponthoz. Egy klaszter középpontja gyakran az ún.
**centroid**, a klaszterbeli összes pont átlaga, vagy a **medoid**, a
klaszter legreprezentatívabb pontja.

**Összefüggő klaszterek** (legközelebbi szomszéd): Egy klaszter
pontoknak olyan halmaza, hogy egy klaszterbeli pont közelebb van
(hasonlóbb) a klaszter más pontjaihoz mint bármelyik nem klaszterbeli
ponthoz.

**Sűrűség alapú klaszterek:** A **klaszter sűrűn elhelyezkedő
pontok** halmaza, amelyet **alacsony sűrűségű tartományok választanak
el** hasonlóan nagy sűrűségű klaszterektől. Akkor használjuk, ha a
klaszterek szabálytalanok vagy egymást átfedőek, illetve **hiba** vagy
**kiugró** értékek vannak.

**Tulajdonság** vagy **fogalom alapú klaszterek**: Keressünk
olyan klasztereket, amelyek valamilyen **közös tulajdonságon**
osztoznak, illetve egy speciális fogalmat jelenítenek meg.

**Egy célfüggvény által leírt klaszterek**: Keressük meg azokat a
klasztereket, amelyek egy **célfüggvényt minimalizálnak vagy
maximalizálnak**. Számoljuk össze az összes klaszterosítást és
értékeljük ki minden lehetséges klaszterosítás ,,jóságát" a célfüggvény
alapján. (NP-nehéz feladat)

Lehetnek **globális és lokális** célfüggvények. A hierarchikus
klaszterosítási algoritmusok általában több lokális célfüggvénnyel
dolgoznak. A felosztó módszerek általában egy globális célfüggvényt
használnak.

A **globális** célfüggvényes megközelítés egy **paraméteres modellt
illeszt az adatokra**. A modell paramétereit az adatokból határozzuk
meg. A keverék modellek feltételezik, hogy az adatok valószínűségi
eloszlások egy ,,keverékét" követik.

Képezzük le a klaszterezési feladatot egy másik tartományba és oldjuk
meg a kapcsolt feladatot abban a tartományban. A **közelségi mátrix**
egy súlyozott gráfot definiál, ahol a csúcsokat kell klaszterezni és a
súlyozott élek reprezentálják a pontok közötti hasonlóságot. A
klaszterezés a gráf összefüggő komponensekre való felbontásával
ekvivalens, a komponensek lesznek a klaszterek. A klasztereken belüli
élek súlyát minimalizálni, a klaszterek közötti élek súlyát pedig
maximalizálni szeretnénk.

**\
**

**Klaszterezési algoritmusok**

**1. K-közép módszer** és változatai

**2. Hierarchikus** klaszterezés

**3. Sűrűség alapú** klaszterezés

**1. K-közép (McQueen) módszer**

**Felosztó** megközelítés.

Minden klaszterhez egy **középpontot** (centroid) rendelünk.

Minden pontot ahhoz a klaszterhez rendelünk, amelynek a középpontjához a
**legközelebb van.**

A **klaszterek száma**, K, **adott** kell, hogy legyen. Az algoritmus
egyszerű.

**Algoritmus. Alap *K*-közép módszer**

1\. Válasszunk ki ***K* kezdeti középpontot.**

2\. **repeat**

3\. **Hozzunk létre *K* klasztert** a pontoknak a **legközelebbi
középpontokhoz** való **hozzárendelésével.**

4\. **Számoljuk újra a középpontot** minden klaszternél.

5.**until** A **középpontok nem változnak** vagy elértük a **max
iterációt**

A **kezdeti középpontok** általában **véletlenszerűek**. A kapott
klaszterek futásról futásra változhatnak.

A középpont (általában) a **klaszterbeli pontok átlaga**.

A ,,közelséget" mérhetjük az **euklideszi távolsággal**, **koszinusz
hasonlósággal, korrelációval** stb.

A K-közép módszer konvergál a fenti általános hasonlósági mértékekre. A
konvergencia legnagyobb része az első néhány iterációban megtörténik.

Általában a leállási feltétel arra módosul, hogy ,,Viszonylag kevés pont
vált klasztert"

**Komplexitás**: O( n \* K \* I \* d ), ahol n: pontok száma, K:
klaszterek száma, I: iterációk száma,

> d: attribútumok száma.

**SSE (hiba négyzetösszeg) (Belső mérték)**

Összetett alakzatoknál a klaszterek nem jól szeparálódnak.

**Belső index:** A **klaszterezés jóságának mérésére használható**
anélkül, hogy külső információkra támaszkodnánk.

Az SSE jó két klaszterosítás vagy két klaszter **összehasonlítására**
(átlagos SSE).

Szintén használható a **klaszterek számának becslésére.**

**K-közép módszer kiértékelése**

Az általános mérőszám: **hiba négyzetösszeg** (SSE -Sum of Squared
Error)

Minden pontra a **hiba** a **legközelebbi klasztertől (középponttól)
való távolság.**

Az **SSE** ezen hibák négyzetének összege:

$$SSE = \sum_{i = 1}^{K}{\sum_{x \in C_{i}}^{}\text{dist}^{2}}\left( m_{i},x \right)$$

--x egy pont a *C*~i~ klaszterben, *m~i~* a *C*~i~ klaszter
reprezentánsa, általában m~i~ a klaszter középpontja (átlaga)

--Két klaszterezés közül azt választjuk, amelyiknek **kisebb a hibája.**

--A legegyszerűbb módja az **SSE csökkentésének** a **K növelése**. Egy
jó klaszterezésnek kisebb K mellett lehet kisebb SSE-je mint egy
rosszabb klaszterezésnek nagyobb K mellett.

**Előfeldolgozás**

Normalizáljuk (standardizáljuk) az adatokat.

Távolítsuk el a kiugróakat.

**Utófeldolgozás**

Távolítsuk el a kis klasztereket, amelyekben **kiugró adatok** lehetnek.

Vágjuk **ketté a ,,széteső"** klasztereket, azaz amelyeknek viszonylag
**nagy az SSE-jük.**

**Vonjuk össze** azokat a klasztereket, amelyek **,,közel" vannak**
egymáshoz és viszonylag **kicsi az SSE-jük**.

Ezeket a lépéseket használhatjuk a klaszterezés során is.

**Felező K-közép módszer**

Egy olyan ***K*-közép variáns**, amely **felosztó**, illetve
**hierarchikus** klaszterezésre egyaránt alkalmazható.

**\
**

**Algoritmus. Felező K-közép módszer**

1.**Inicializálás.** A klaszterlista tartalmazzon egy **klasztert,**
amelynek az **összes pont legyen az eleme.**

2.**repeat**

3\. Válasszunk ki egy klasztert a listából. (Többször is
próbálkozhatunk.)

4\. **for** i=1 **to** iterációk_száma **do**

5\. **Osszuk fel** a kiválasztott **klasztert** az alap **K-közép**
algoritmussal.

6\. end for

7\. **Adjuk hozzá** azt a két klasztert a **klaszterlistához,**
amelyeknek a **legkisebb az SSE-jük.**

8.**until** Ismételjünk addig, amíg a **klaszterlista *K* klasztert**
nem tartalmaz.

**Variációk**

**K-medoid:** A feladat definíciója hasonló a K-középhez kivéve,
hogy egy klaszter **középpontját** úgy definiáljuk, hogy a **klaszter
egy pontja** legyen (pl.medián)(a K-középnél ez általában nem teljesül)

**K-center:** A feladat definíciója hasonló a K-középhez kivéve,
hogy a célfüggvény a **klaszterek maximális átmérőjének a
minimalizálása** (egy klaszter átmérője: a klaszter bármely két pontja
közötti maximális távolság).

**Árnykép együttható (Belső mértékek)**

Az árnykép együttható az **összetartás és az elválasztás** ötletét
**kombinálja** mind egyedi pontokra, mind pedig klaszterekre és
klaszterezésekre.

Egy *i* egyedi pontra

--Számoljuk ki ***a***= az *i* **átlagos távolságát** a **klaszteren
belüli** pontoktól.

--Számoljuk ki ***b***= **min** (az *i* **átlagos távolságát** **más
klaszterektől**)

--Egy pont **árnykép együtthatóját** az alábbi módon definiáljuk: **s =
1 --a/b** ha a \< b,

(vagy s = b/a -1 ha a ≥ b, nem szokványos eset)

--Általában **0 és 1** közé esik.

--Minél **közelebb** van az **1-hez** annál **jobb.**

Az átlagos árnykép szélességet ezután klaszterekre és klaszterezésekre
is ki tudjuk terjeszteni.

**\
**

## 7. Klaszterezés: hierarchikus és sűrűség alapú módszerek. Egyszerű, teljes és átlagos kapcsolás, Ward módszere, dendrogram, DBSCAN.

**2. Hierarchikus klaszterezés**

**Egymásba ágyazott** klaszterek egy **hierarchikus fába** szervezett
halmazát állítja elő.

Egy ún. **dendrogram**mal jeleníthetjük meg.

-- Ez egy **fa alakú diagram**, amely a rekordokat **összevonások** vagy
**szétvágások sorozataivá** rendezi.

**Előnye,** hogy **nem** kell feltételezni semmilyen **konkrét
klaszterszámot.**

Értelmes **osztályozásoknak** (taxonómiáknak) is megfelelhet.

**Két fő típusa:**

**-Összevonó**: Induljunk **minden pontot külön klaszterként**
kezelve. Minden lépésnél **vonjuk össze** a két **legközelebbi**
klasztert amíg csak egy (vagy k) klaszter nem marad.

**-Felosztó**: Induljunk egy minden **pontot tartalmazó
klaszterből**. Minden lépésnél **vágjunk ketté** egy klasztert amíg
minden klaszter csak egy pontot nem tartalmaz (vagy amíg k klasztert nem
kapunk).

A hagyományos hierarchikus algoritmusok **hasonlósági vagy távolság
mátrixot** használnak. **Egyszerre egy klasztert** vonjunk össze vagy
vágjunk szét.

**Klaszter-hasonlóság**

**MIN vagy egyszerű kapcsolás**

Két klaszter **hasonlósága** a klaszterekbeli **két leghasonlóbb
(legközelebbi) ponton** alapszik.

\-**Egy pontpár által**, azaz a közelségi gráfban **egy kapcsolat
által** (a többitől függetlenül) meghatározott.

**Előnye**: Nem elliptikus alakot is tud kezelni.

**Korlátai:** Érzékeny a hibára és a kiugró adatokra

**MAX vagy teljes kapcsolás**

Két klaszter közötti **hasonlóság** a klaszterekbeli **két legkevésbé
hasonló (legtávolabbi) ponttól függ.**

-- A két **klaszter összes pontja** által meghatározott.

**Előnyei:** Kevésbé érzékeny a hibára és a kiugró adatokra.

**Korlátai:** Hajlamos a nagy klasztereket kettévágni. Torzít a gömbölyű
klaszterek irányába.

**Csoport-átlag (Átlagos kapcsolás)**

Két klaszter közötti **közelség** a klaszterekbeli **pontok közötti
mérőszámok átlaga.**

Azért kell a **skálázhatóság** miatt átlagos összekapcsolhatóságot
használni, mert a teljes közelség előnyben részesíti a nagy
klasztereket.

Az **egyszerű** és a **teljes** kapcsolás közötti **kompromisszum.**

**Előnyei:** Kevésbé érzékeny a hibára és a kiugró adatokra.

**Korlátai:** Torzít a gömbölyű klaszterek irányában.

**Ward módszer**

Két klaszter közötti **hasonlóság** azon alapszik, hogy az
**összevonásuk** után **mennyivel nő a négyzetes hiba.**

--Hasonló a **csoport-átlag**hoz amennyiben a pontok közötti távolság a
**négyzetes euklideszi távolság**.

**Előnyei:** Kevésbé érzékeny a hibára és a kiugró adatokra.

**Hátránya**i: Torzít a gömbölyű klaszterek irányában.

A ***K*-közép** módszer **hierarchikus** változata

--A *K*-közép inicializálására is használható.

**Hierarchikus klaszterezés:**

**Idő és tár korlátok**

O(N^2^) **tárigény** mivel a közelségimátrixot használja.

--N a pontok száma.

O(N^3^) **időigény** az esetek többségében.

--**N lépést** kell végrehajtani és minden egyes lépésben egy N^2^
méretű közelségimátrixot kell **frissíteni** és kell benne **keresni.**

--Egyes megközelítéseknél az időigény O(N^2^log(N))-re redukálható.

**\
**

**Problémák és korlátok**

Ha egyszer **döntést hozunk** arról, hogy két klasztert **összevonun**k,
akkor azt már **nem lehet meg nem történtté tenni.**

**Nincs célfüggvény,** melyet közvetlenül **minimalizálunk.**

A különböző eljárásoknál az alábbi **problémák** közül léphet fel **egy
vagy több:**

--**Érzékenység a hibára** és a **kiugró** adatokra.

--Nehéz kezelni a **különböző méretű klasztereket** és **konvex**
alakzatokat.

--Hajlam **nagy klaszterek szétvágására.**

**3. Sűrűség alapú**

**DBSCAN**

Density-Based Spatial Clustering of Applications with Noise--**Sűrűség
alapú térbeli klaszterezés hiba mellett**

A DBSCAN egy sűrűség alapú algoritmus.

--**Sűrűség** = egy rögzített sugáron (Eps) belüli pontok száma

--Egy pont **belső pont,** ha egy **előírtnál** (MinPts) **több
pont** van Eps **sugarú környezetében.**

-Ezek lesznek egy klaszter belsejének pontjai.

--A **határ pontnak** **az Eps sugarú környezetben** **MinPts-nél
kevesebb pontja** van, azonban **van belső** pont ebben a környezetben.

--A **zajos pont** az összes olyan pont, amelyik **nem belső**
illetve **határ pont.**

**Előnyei**: **Ellenálló a zajjal** szemben. **Különböző méretű** és
**alakú** klasztereket egyaránt tud kezelni.

**Hátrányai**: **Változó sűrűség**, **Magas dimenziójú** adatok esetén
**nem jól** működik

**\
**

## 8. Vásárlói kosár adatok. Gyakori tételcsoport és támogatottság. Az Apriori elv és algoritmus. Jelöltgenerálás. Asszociációs szabályok. Megbízhatóság. Mintázat-kiértékelés: statisztikus mérőszámok, lift érték.

**Vásárlói kosár adatok**

**Termékek** egy nagy halmaza, pl. egy szupermarket kínálata.

**Kosarak** egy **nagy halmaza**, amelyek mindegyike **termékek egy kis
halmaza**, pl. azok a termékek, melyeket egy vásárló egy vásárlás
alkalmával vesz (a kosarába tesz).

Valójában egy **általános leképezés** (hozzárendelés) kétféle dolog
között, ahol az **egyik** (kosarak) a **másik** (termékek) egy
**részhalmaza.**

--Azonban mi a **termékek** és nem a kosarak **közötti kapcsolatokra**
vagyunk kíváncsiak.

A módszer a **gyakori eseményekre** és nem a ritkákra fókuszál ("hosszú
farok").

**Tételcsoport**

--**Egy** vagy **több tétel összessége.**

-Példa: {Tej, Kenyér, Pelenka}

--k-tételcsoport

k számú tételt tartalmazó tételcsoport

**Támogatottsági érték (σ)**

--Egy **tételcsoport előfordulási gyakorisága**.

--Pl. σ({Tej, Kenyér,Pelenka}) = 2

**Támogatottság**

--Egy **tételcsoportot tartalmazó tranzakciók aránya.**

--Példa: s({Tej, Kenyér, Pelenka}) = 2/5

**Gyakori tételcsoport**

--Egy olyan tételcsoport, amely **támogatottsága nagyobb vagy egyenlő**
egy ***minsup* küszöb értéknél.**

**Alkalmazások**

Tételek= termékek; kosarak= termékek összessége melyet egy vásárló a
kosarába tesz a boltban.

--Példa: adott, hogy sok vásárló vesz együtt **sört és pelenkát**:
akciózzuk a pelenkákat és emeljük a sör árát.

--Csak akkor hasznos, ha sokan vesznek együtt pelenkát és sört.

Kosarak= **Web lapok**; tételek**= szavak.**

--Példa: Szokatlan szavak melyek együtt fordulnak elő nagy számú
dokumentumban, pl."Brad" és "Angelina," egy érdekes kapcsolatot
jelölhet.

Kosarak= **mondatok**; tételek= **dokumentumok** melyek ezeket a
mondatokat tartalmazzák.

--Példa: Azok a tételek melyet túl gyakran fordulnak elő együtt
plágiumot jelenthetnek.

--Vegyük észre, hogy a tételeknek nem kell benne lenniük a kosarakban.

**Gyakori tételcsoportok bányászata**

**Input:** A tranzakciók **T halmaza** tételek egy I halmaza felett

**Output:** Tételeknek az **összes** olyan halmaza **I-ben** melyre

--**support ≥ *minsup* threshold** (támogatottság ≥ min_támogatottsági
érték)

Feladat paraméterei:

--N = \|T\|: tranzakciók száma

--d = \|I\|: (különböző) tételek száma

--w: a tranzakciók maximális szélessége

--A lehetséges tételcsoportok száma?

M = 2^d^

Feladat mérete:

--WalMart 100 000 tételt árusít és kosarak **millióit** tartja nyilván.

--A Web szavak **milliárdjait** és sok milliárd lapot tartalmaz.

**Gyakori tételcsoportok előállítása**

Adott d számú tétel-nél 2^d^ számú **jelölt** van tételcsoportra.

**Nyers erő** megközelítés:

--**Minden csúcs** a gráfban egy **jelölt** gyakori tételcsoportra.

--Számítsuk ki minden **jelölt támogatottságát** az adatbázis
átfésülésével.

--Vessünk össze **minden tranzakciót** **minden jelölttel**!

--Komplexitás \~ O(NMw) =\> **Költséges mivel M = 2^d^**!!!

**Kiszámítási komplexitás**

Adott *d* számú tétel esetén:

-- Az összes tételcsoport száma = 2^d^

-- Az **összes lehetséges társítási szabály** száma: R = 3^d^ -- 2^d+1^
+ 1

Ha d=6 akkor R = 602 szabály

**A számítási modell**

Általában az adatokat egy **flat fájlban** tároljuk és nem egy
adatbázisban.

--Ezt a fájl a **lemezen tároljuk.**

--A tárolás **kosaranként** történik.

--A kosarakat párokká, hármasokká stb. bontjuk ki ahogy beolvassuk őket.

A kibontás során **k** **egymásba ágyazott ciklust** használunk, hogy az
összes **k** **elemű halmazt előállítsuk.**

**Gyakori tételcsoportok előállítása**

**Csökkentsük** a **jelöltek számát**(*M*)

--Teljes keresés: *M=2^d^*

--Használjunk **vágási módszereket** *M* csökkentésére.

Csökkentsük a **tranzakciók számát**(*N*)

--Csökkentsük N-et a **tételcsoportok számának növekedésével.**

--Használjunk DHP (direct hashing and pruning --**közvetlen hasító és
vágó**) illetve **vertikálisan bányászó algoritmusokat.**

**Csökkentsük** az **összehasonlítások számát**(NM)

--Használjunk **hatékony adatszerkezeteket** a jelöltek és a tranzakciók
tárolására.

--Nem szükséges minden jelöltet és tranzakciót összehasonlítani.

**\
**

**A jelöltek számának csökkentése**

**Apriori elv**

--Ha egy tételcsoport **gyakori,** akkor **minden részhalmaza is
gyakori**.

Az apriori elv a **támogatottság** következő **tulajdonságán alapszik:**

∀ X, Y: (X ⊆ Y) =\> s(X) ≥ s(Y)

--Egy **tételcsoport támogatottsága sohasem haladhatja meg
részhalmazainak támogatottságát.**

--Ez a támogatottság ún. **anti-monoton** tulajdonsága.

**Az Apriori algoritmus**

**Szintenkénti megközelítés**

C~k~= k méretű tételcsoport jelöltek

L~k~= k méretű gyakori tételcsoportok

1\. k = 1, C~1~= összes tétel (egy elemű tételcsoportok)

2\. While C~k~ nemüres

3\. Adatbázis átfésülésével találjuk meg **C~k~-ban a gyakori
tételcsoportokat** és **tegyük L~k~-ba**

(gyakori tételcsoport generálás)

4\. Használjuk **L~k~**-t a **tételcsoport jelöltek** k+1 méretű C~k+1~
**halmazának előállítására**

(jelölt generálás)

5\. k = k+1

**Jelölt generálás**

Alapelv (Apriori):

--Egy **(k+1)-tételcsoport** csak akkor lehet **gyakori jelölt** ha az
**összes** k méretű **részhalmaza** (biztosan) **gyakori.**

Alapötlet:

--Konstruáljunk egy k+1 méretű jelöltet k méretű gyakori tételcsoportok
**összekombinálásával**.

-Ha k = 1 akkor vegyük a gyakori tételcsoportok összes párját

> -Ha k \> 1 akkor **egyesítsük** tételcsoportok olyan párjait melyek
> csak **egy tételben** **különböznek**
>
> -Minden egyes generált tételcsoport **jelöltnél** győződjünk meg, hogy
> az **összes k elemű részhalmaza gyakori-e.**

**A C~k+1~-beli jelöltek generálása**

Feltevés: a tételcsoportokban a **tételek rendezettek**

-Pl., ha az egészek nagyság szerint növekvő sorba rendezettek, ha a
rekordok lexikografikusan rendezettek

> -A rendezettség biztosítja, hogy ha y \> x esetén y előfordul x előtt,
> akkor x nincs benne a tételcsoportban

Az L~k~-beli tételek szintén rendezettek

Hozzunk létre egy (k+1)-tételcsoportot két olyan **k-tételcsoport
egyesítésével** amelyeknek **az első k-1 tétele ugyanaz.**

**Tisztítási lépés:**

--Minden egyes (k+1)-tételcsoport jelöltnél állítsuk elő az összes
**k-rész-tételcsoportját**

--**Töröljük** azt a jelöltet, amely részhalmazként egy olyan
k-tételcsoportot tartalmaz, amely **nem gyakori**

Adott az összes gyakorik-tételcsoport L~k~ halmaza

1\. lépés: self-join L~k~

> \-**Hozzuk** létre a C~k+1~ halmazt azon **gyakorik-tételcsoport**
> párok egyesítésével, amelyeknek az elsők-**1 tétele közös**

2\. lépés:tisztítás

> \-**Töröljük** C~k+1~--ból azokat a tételcsoportokat, amelyek olyan
> rész k-tételcsoportot tartalmaznak, amelyek **nem gyakoriak**

**Az összehasonlítások csökkentése**

Jelöltek leszámlálása:

--A tranzakciós adatbázis átfésülésével határozzuk meg minden
**tételcsoport jelölt támogatottságát**.

--**Az összehasonlítások számának csökkentése** érdekében a jelölteket
tároljuk **hash szerkezetben.**

> -Ahelyett, hogy minden tranzakciót minden jelölttel összehasonlítunk,
> használjunk hasított kupacokat a jelöltekre.

**A komplexitást befolyásoló tényezők**

A **minimális támogatottság** megválasztása

--Csökkentése **több gyakori tételcsoportot** eredményez.

--Növelheti **a jelöltek számát** és a **gyakori tételcsoportok
hosszát.**

Az adatállomány **dimenziója** (tételek száma)

--Több hely szükséges a tételek támogatottságának tárolására.

--Ha a **gyakori tételek** száma is **nő,** akkor a **számításigény** és
az **I/O költség is nő.**

Az adatbázis **mérete**

--Mivel az apriori többször végigfésüli az adatbázist a **futási idő nő
a tranzakció számmal.**

Átlagos **tranzakció szélesség**

--A **tranzakció szélesség** együtt **nő az adathalmaz** (tételek)
**növekedésével.**

--Növelheti a gyakori tételcsoportok maximális hosszát és a hasító fa
szélességét(a tranzakcióbeli részhalmazok száma együtt nő a
szélességével).

**Gyakori tételcsoportok kompakt reprezentációja**

Egyes tételcsoportok **redundánsa**k mivel azonos a támogatottságuk
egyes bővítéseikével.

Kompakt reprezetációra van szükség!

**Maximális gyakori tételcsoport**

Egy gyakori tételcsoport **maximális**, ha **közvetlen bővítéseinek**
egyike **sem gyakori.**

**Zárt tételcsoport**

Egy tételcsoport **zárt**, ha **közvetlen bővítéseinek** egyikével **sem
egyezik meg a támogatottsága.**

**További módszerek gyakori tételcsoportok előállítására**

Átkelés a tételcsoport gráfon

--Általánostól a speciálisig vagy speciálistól az általánosig

--Ekvivalencia osztályok

--Szélességi vagy mélységi keresés

Az adatbázis reprezentációja

--Horizontális vagy vertikális elrendezés

**Társítási szabályok bányászata**

Tranzakciók egy adott halmazában keressünk olyan **szabályokat**,
amelyek egyes **tételek előfordulását előrejelzik** más tételek
előfordulása alapján.

**Társítási szabály fogalma (Asszociációs szabály)**

-- Egy X Y alakú következtetés, ahol X és Y tételcsoportok.

-- Példa: {Tej, Pelenka} {Sör}

**Szabály kiértékelési metrikák**

**-- Támogatottság (s)** (support)

-Azon **tranzakciók aránya**, amelyek az **X és Y tételcsoportot**
egyaránt **tartalmazzák.**

-- **Megbízhatóság (c)** (confidence)

> -Azt méri, hogy az **Y-beli tételek** milyen **gyakran** jelennek meg
> olyan tranzakciókban, melyek **tartalmazzák X-et.**

**Társítási szabályok bányászatának feladata**

Tranzakciók egy adott T halmaza esetén a társítási szabály bányászat
**célja** az **összes** olyan **szabály** megtalálása, amelyre

**--támogatottság ≥ *minsup* küszöb,**

**--megbízhatóság ≥ *minconf* küszöb.**

**Nyers erő** megközelítés:

--Vegyük lajstromba az **összes társítási szabályt.**

--Számoljuk ki a **támogatottságot** és a **megbízhatóságot**.

--**Távolítsuk el** azokat a szabályokat, melyek a *minsup* és *minconf*
**küszöbnek nem tesznek eleget.**

**Kiszámítási szempontból végrehajthatatlan!**

Az ugyanarra a tételcsoportra visszavezethető szabályoknak **azonos a
támogatottsága** a **megbízhatósága** viszont **eltérő lehet.**

Így a támogatottsági és megbízhatósági követelményeket elválaszthatjuk.

**\
**

**Társítási szabályok bányászata**

1\. lépés **Gyakori tételcsoportok előállítása**

--Állítsuk elő az összes olyan tételcsoportot, melyre **támogatottság ≥
minsup.**

**2.** lépés **Szabály generálás**

--Állítsuk elő azokat a magas **megbízhatóságú szabályokat** minden
**gyakori tételcsoportra**, amelyek a **tételcsoport bináris
partíciói.**

A gyakori tételcsoportok előállítása még mindig kiszámításilag
**költséges.**

Szabály generálás az **apriori algoritmussal.**

**Mintázat kiértékelés**

A társítási szabály algoritmusok hajlamosak **túl sok szabályt**
szolgáltatni.

--Sok közülük nem érdekes vagy redundáns.

--Redundáns ha {A,B,C} {D} és{A,B} {D} szabályoknak **megegyezik a
támogatottsága és a megbízhatósága.**

**Érdekességi mértékeket** használhatunk az eredményül kapott **minták
törlésére** vagy **sorba rendezésére.**

A társítási szabályok bevezetésekor csak a támogatottság és
megbízhatóság mértékeket alkalmazták.

**Érdekességi mértékek meghatározása**

Egy adott X Y szabály esetén az érdekességi mértékek meghatározásához
szükséges információk egy **kontingencia táblából** kaphatóak.

Számos mérőszám definiálására használható: támogatottság, megbízhatóság,
lift, Gini, J-mérték stb.

**Statisztika alapú mérőszámok**

Az alábbi mérőszámok figyelembe veszik a statisztikus **függetlenséget**

**Lift** = $\frac{P(Y|X)}{P(Y)}$

**Érdekesség** = $\frac{P(X,Y)}{P(X)P(Y)}$

**Egy jó M mértéknek az alábbi 3 tulajdonságot kell kielégíteni
(Piatetsky-Shapiro)**

\- **M(A, B) = 0**, ha A és B **statisztikusan független**

\- **M(A, B) monoton nő P(A, B)-vel** , amennyiben P(A) és P(B)
változatlan marad

\- **M(A, B) monoton csökken P(A)-val** , amennyiben P(A, B) és P(B)
változatlan marad

## 9. Rendellenesség-keresés: definíció, feladatok, alkalmazások. Módszerek: grafikus, statisztikus, távolság alapú, modell alapú.

**Mit értünk rendellenes/kiugró adat alatt?**

A rekordoknak egy olyan halmaza, amely **számottevően eltér a többi
adattól.**

**Kapcsolódó feladatok:**

--Adott *D* adatbázisban **találjuk meg** az összes olyan ***x***∊*D*
rekordot, amely **rendelleneségi pontszáma nagyobb, mint egy t küszöb.**

--Adott *D* adatbázisban találjuk meg az összes olyan ***x***∊*D*,
rekordot, melynek ***f(x)* rendellenessége az *n* legnagyobb között
van.**

--Adott *D* adatbázisban, mely jobbára normális rekordokat tartalmaz, és
egy ***x*** tesztpont esetén számoljuk ki ***x* rendellenességi
értékét** *D*-re vonatkozóan.

**Alkalmazások:** Hitelkártya csalások, telekommunikációs csalások,
hálózati betörések, csalások keresése.

**Rendellenességek keresése**

Kihívások

--**Mennyi kiugró érték** van az adatok között?

--**Nemfelügyelt** feladat

-Az ellenőrzés (éppen, mint a klaszterezésnél) nehéz is lehet.

--Tű keresése a szénakazalban.

Munka hipotézis

--Jóval több ,,normális" mint ,,abnormális" (kiugró/rendellenes)
megfigyelés van az adatállományban.

**Rendellenesség keresési sémák**

Általános lépések

--Alkossunk profilt a **,,normális"** viselkedésről.

-Ez lehet **mintázat vagy összegző statisztika** a teljes populációra.

--Alkalmazzuk ezt a ,,normális" profilt **rendellenesség**
**keresésre.**

> -Azokat a megfigyeléseket nevezzük rendellenesnek, amelyek
> **lényegesen eltérnek a normális profiltól.**

**Rendellenesség keresési sémák osztályozása**

--Grafikus és statisztikus alapú

--Távolság alapú

--Modell alapú

**1. Grafikus megközelítések**

Doboz ábra(1-D), pont diagram(2-D), térbeli diagram(3-D)

**Korlátok:**

--Idő igény

--Szubjektív

**Konvex burok módszer**

Az **extrém helyű** pontokat **kiugróaknak** tekintjük.

Használjuk a konvex burkot ezen pontok meghatározására.

Mi történik, ha a kiugró adat középen van?

**2. Statisztikus megközelítések**

Tegyük fel, hogy egy **paraméteres modell** írja le az adatok
**eloszlását** (pl. normális eloszlás).

Alkalmazzunk **statisztikai próbákat**, melyek függnek

--az adatok **eloszlásától,**

--az eloszlás **paramétereitől** (pl. várható érték, variancia),

--a **kiugró** értékek **várható számától** (konfidencia határ).

**Grubbs próba**

**Kiugró értékeket** keres **egydimenziós** adatokban. Felteszi az
adatok **normális eloszlását.**

Egyszerre **egy kiugró értéket keres**, azt **eltávolítja,** majd
megvizsgálja az alábbi **hipotéziseket**

-- H0: Nincs kiugró érték az adatokban

-- HA: Van legalább egy kiugró érték

Grubbs próba statisztika:
$G = \frac{\max\left| X - \overline{X} \right|}{s}$

**Likelihood módszer**

Tegyük fel, hogy a D adatállomány **két valségi eloszlás keverékéből**
származó mintát tartalmaz:

--M (**többségi** eloszlás),

--A (**rendellenes** eloszlás).

Általános megközelítés:

--Tegyük fel kezdetben, hogy az összes rekord *M*-beli.

--Legyen *L~t~(D)* a ***D* loglikelihoodja a *t* időpillanatban.**

--Minden M-hez tartozó *x~t~* rekordot mozgassunk át *A*-ba.

-Legyen *L~t+1~(D)* az új loglikelihood.

-Számoljuk ki a **differenciát** Δ*= L~t~(D) --L~t+1~(D).*

> -Ha **Δ*\> c ***(küszöbérték), akkor ***x~t~*-t rendellenesnek**
> minősítjük és **véglegesen átmozgatjuk** *M*-ből *A*-ba.

Az adatok eloszlása: D = (1 --λ) M + λA

M egy az adatokból becsülhető **valségi eloszlás.**

--A becslés alapulhat bármilyen modellen (naívBayes, maximális entrópia
stb).

A-t kezdetben **egyenletes eloszlásúnak** feltételez-zük.

**A statisztikus megközelítés korlátai**

A legtöbb próba csak **egy attribútumra** működik.

Legtöbbször **nem ismert** az adatok **eloszlása.**

Magas dimenzióban **nehéz becsülni az igazi eloszlást.**

**3. Távolság alapú módszerek**

Az adatokat **jellemzők egy vektorával reprezen**-táljuk.

Három fő megközelítés

--Legközelebbi társ módszer

--Sűrűség alapú

--Klaszter alapú

**\
**

**Legközelebbi társ alapú megközelítés**

--Számoljuk ki az **összes pontpár** közötti **távolságot.**

--A **kiugró értékek** definiálásának többféle módja van:

> -Azok a pontok, amelyeknek egy adott ***d* sugarú környezetében**
> **kevesebb mint *p* számú pont van.**

-Az az *n* pont, amelynek a ***k*-adik legközelebbi szomszédjától** vett
**távolsága a legnagyobb**.

> -Az az *n* pont, amelynek az **átlagos távolsága** a *k* darab
> **legközelebbi szomszédjától a legnagyobb.**

**Kiugró értékek vetületekben**

Osszunk fel minden attribútumot φ egyenlő mélységű **intervallumra.**

--Minden intervallum *f = 1/*φ részt tartalmaz a rekordokból.

Tekintsünk egy ***k* dimenziós kockát**, melyet *k* különböző dimenzió
menti **részintervallum kijelölése ad.**

--Ha az attribútumok **függetlenek** akkor várhatóan ***f^k^*** részét
tartalmazza a **rekordoknak.**

--N pont esetén a *D* **kocka ritkaságát mérhetjük**

--**Negatív ritkaság** a **vártnál kisebb számú pontot** jelez a
kockában.

**Sűrűség alapú megközelítés: LOF**

Számoljuk ki az összes **pont lokális környezetének sűrűségét.**

Számoljuk ki egy ***p* minta** **lokális kiugró faktorát** (LOF) úgy,
mint a **minta** és az ő **legközelebbi szomszédjai sűrűségének az
átlagát.**

**Kiugróak** a **legnagyobb LOF értékkel** rendelkező **pontok.**

**Klaszter alapú megközelítés**

**Klaszterosítsuk** az adatokat **különböző sűrűségű csoportokra.**

Válasszuk **kiugró jelölteknek** a **kis klaszterek pontjait.**

Számoljuk ki a **kijelölt pontok** és a **nem kijelölt** klaszterek
**közötti távolságot.**

-Ha a kijelölt pontok **messze** vannak a nem kijelölt pontoktól, akkor
**ők kiugróak.**

**\
**

**Téves következtetési arány (Modell alapú??)**

Bayes tétel:
$P\left( A \middle| B \right) = \frac{P(A)\ ·\ P(B|A)}{P(B)}$

Pl. Tegyük fel, hogy egy orvos által végzett **teszt pontossága 99%,**
azaz egy beteg populáción 99%-osan jelez betegséget, és egy egészségesen
99%-ban ad negatívat. Vizit után az orvosnak van egy jó és egy rossz
híre. Rossz hír: a teszt pozitív lett. Jó hír: a (betegség) előfordulása
a teljes populációban 1/10000.

Mennyi a valószínűsége, hogy **valóban betegek vagyunk?**

Bár a teszt 99%-osan pontos, annak esélye, hogy mégis **betegek
vagyunk** **1%**, mivel a populáció-ban az **egészséges emberek** jóval
**többen vannak, mint a betegek**.
