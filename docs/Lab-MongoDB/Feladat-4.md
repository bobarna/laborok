# Feladat 4: Vevők listázása (4p)

Ebben a feladatban a vevőket fogjuk listázni — az általuk megrendelt termékek összértékével együtt. Ehhez a második feladathoz hasonlatosan aggregációs utasítást és C# kódban történő "összefésülést" kell majd használnunk.

A `Models.Vevo` entitás adattagjai:
* `Nev`: a vevő neve
* `IR`, `Utca`, `Varos`: a vevő központi telephelyéhez tartozó cím
* `OsszMegrendeles`: a vevőhöz tartozó összes megrendelés összértékének (lásd előző feladat) összege. Amennyiben még nincs az adott vevőhöz tartozó megrendelés, akkor ennek az értéke legyen `null`!

A feladat megoldásához ajánlott lépések:

1. Vedd fel és inicializáld a `vevoCollection`-t!

1. Listázd ki az összes vevőt. A vevő entitásban megtalálod a telephelyek listáját és a központi telephely azonosítóját is. Ez utóbbit kell megkeresned az előbbi listában, hogy megkapd a központi telephelyet (és így a hozzá tartozó címet).

1. A megrendelések kollekcióján aggregációs pipeline-t használva meg tudod állapítani az adott `VevoID`-hez tartozó összmegrendelések értékét.

1. Végezetül csak a meglevő információkat kell "összefésülnöd". Központi telephelye minden vevőnek van, viszont megrendelése nem garantált — figyelj oda, hogy ekkor az `OsszMegrendeles` elvárt értéke `null`!

1. A kód kipróbálásához a weboldal `Vevők` menüpontjára kell navigálni. Itt táblázatos formában megjelenítve láthatod az összegyűjtött információkat. Teszteléshez alkalmazhatod az előző feladatban elkészített `Új megrendelés felvétele` funkciót — itt új megrendelés felvétele esetén `Grosz János` mellett növekednie kell a hozzá tartozó megrendelések összértékének.

1. Készíts egy képernyőképet implementált függvény kódjáról. (A képernyőképpel kapcsolatos elvárásokról lásd a kezdőoldalon.)

   > A képet a megoldásban `f4-vevok.png` néven add be.
   >
   > A képernyőkép 1 pontot ér.

## Következő feladat

Nincs több feladat. Add be a megoldásod az [itt](README.md) leírtak szerint.