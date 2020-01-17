0. Vezetői összefoglaló
kereste egy XY cég aki szeretné ha az önéletrajz kitoltésére készítenénk egy programot amely megkönnyíti a hozzájuk valo jelentkezést.

1. A rendszer céljai, és nem céljai
Egy felület létrehozása amelyel leegyszerűsítia a önéletrajz készítését és ezzel könyebben jelentkezve az adott céghez. Nem célunk a kitöltés után kapott adatok további feldolgozása.

2. Jelenlegi helyzet leírása
Egy olyan oldal készítése amely megkönnyíti az önéletrajz készítését.
Az oldal használójátol kéri be az adatait ilyen adatok például: név, elért eredmények, holtanult stb stb.

3. A vágyálomrendszer leírása
Az oldal bekéri a nevet, emailt elérhetőséget, lakhely nemet, oktatást, továbbá rövid ismertetőt önmagárol, szuletési dátumát. Ezekről az adatokrol valos idejű visszajelzést kap a kitöltött adtokrol,
ezt követöen tudja modosítani az adatai ha nem etszenek illetve rosszul irt le valamit, majd lehetősége nyilik további feldolgozásra.

4. A rendszerre vonatkozó külsõ megszorítások
A rendszerre vonatkozó külsö megszorítások közé tartoznak az alábbiak: - pályázat - törvények - rendeletek - szabványok és ajanlások Tekintsük először a pályázatot. Pályázat elnyerése esetén eleget kell tenni a pályázatban leírt feltételeknek is. Nem elegendő a saját magunk elé kitűzott céldátum, hanem figyelembe kell venni azt is, hogy a pályázat mennyi időre szól és mikor jár le. Mindezek mellett pályázat esetén meghatározottak azok is, hogy a pályázaton elnyert pénzt, a projekt mely részében, a projekt mely elemeire használhatjuk fel. Törvény esetében figyelembe kell venni azt a tényt, hogy a projekt mely országon belül készül és mely országban/országokban szeretnék a későbbiekben ezt forgalmazni és használni. A programnak eleget kell tennie az összes forgalmazni kívánt ország törvényeinek. Esetünkben, mivel egy játékos oktatásról van szó, így korhatáros tartalmakat nem tartalmazhat, illetve egyéb olyan ábrákat, szövegeket sem, amelyek a gyermekre káros hatással vannak és befolyásolják őt fejlődésében. Ezeken kívül még lehetnek külön erre a célra alkalmazott rendeletek, amelyeket szinten figyelembe kell venni. Mivel Magyarországon készül el a program, így ez esetben törvényileg a MAGYAR törvénykönyv szabályozásainak is meg kell felelnie. Összességét tekintve a gonololatjelek között és kapcsolat van, vagyis mindennek érvényesülnie kell egyszerre. Figyelembe kell venni a pályázati feltételeket, a törvényeket és rendeleteket és ügyelni kell a szabványokra. Ha az összes tényező közül bármelyik is hiányzik vagy hibás, akkor a projekt nem megfelelő és nem tökéletes.

5. Jelenlegi üzleti folyamatok modellje

 	1. Ügyelni a veboldal jó optimalizálására.
 	2. Biztosítani kell az oldal megfelelő biztonságát hogy más az illetéktelen személyek ne férjenek hozzá.
 	3. Ügyelni az oldal Url cím egyértelműségére.

6. Igényelt üzleti folyamatok modellje
	
	1. Szeretnénk hogy átátható legyen minél egyszerübb letisztultabb.
	2. Megfelelő mezőkbe megfelelő adatok kerüljenek.
	3. Szeretnénk hogy az oldal mobil eszközökre is optimalizált legyen.
	4. Az oldal a kitoltott adatokkat a feldolgozo program számára megfelelő formátumban küldje el
	5. A cégünk eléggé nyitott gondolkozásü ezért szeretnénk a nemek kőzé egy harmadik opciót ha egyik közé se valja a személy magát.

7. Követelménylista

K1: Ügyelni a veboldal jó optimalizálására.
K2: Biztosítani kell az oldal megfelelő biztonságát hogy más az illetéktelen személyek ne férjenek hozzá.
K3: Ügyelni az oldal Url cím egyértelműségére.
K4: Legördülő menüben kategóriánként való listázás

8. Szereplők: - Felhasználó, vendég, szerkesztő

Felhasználó használati esetei: Személyes adatok megadása és tovább küldése feldolgozásra.

9. Követelményspecifikáció megfeleltetése

? - Nem biztos, hogy release napi funkció

☒ - Regisztráció
☒ - Bejelentkezés
☒ - Vendég felület
☒ - Admin felület
☑ - Adatbázis feltöltése adatokkal
☑ - Főoldal
☑ - felhasználóbarát

10. Képernyőtervek

11. Forgatókönyvek:
Felhasználó: Ellátogat az URL cimre és ott feltolthet a személyes adataival egy önéletrajzot.
Az oldalon ugy tud atatokat bevinni hogy megkeresi a megfelelő mezőt és azokba belekattintva tud bele billenytű segítségével bevinni adatokat, illetve vannak legördülő memüsorok amiket rakantitva érhet el és választhat ki.

12. fejezet

-[felhasználó felület]: A felhasználónak lehetősége van szémely adatokat feltölteni egy adatbázisba.
-[frontend]:  egy réteg ami feladata a rendszerbõl kijutó adatok prezentálása, illetve a bejövõ adatok fogadása
-[backend]: A kiszolgáló, ahonnan az alkalmazást el lehet érni 
-[bug]: fejlesztési hiba ami által a program nem a várt eredményt hozza 
-[web-service]: Különbözõ programnyelveken írt és különbözõ platformokon futó szoftveralkalmazások interneten keresztül történõ adatcseréjére használt webszolgáltatások.