# Tesztelési terv 
### Main Project

|  Dokumentum címe: (azonosítója) |  K&B |
|---|:-:|
| **Minősítés: (állapot)**  |  Jóváhagyott |
| **Verziószám:**  |  ALFA 1.0 |
| **Projekt név:** |  önéletrajz |
| **Készítette:** | K@B Team |
| **Utolsó mentés kelte:** | 2020 @ 01.15 00:00 |
| **Dokumentum célja:** | A projekt aktualis állapotának bemutatása   |
| **Fájlnév** | Tesztterv.md |

### Projektben résztvevő fejlesztők:

|  Név | Szerepkör |
|---|:-:|
| Kiss Mián | Dokumentáció |
| Tolvaj Balázs:  | fejlesztő |

## 1. Bevezetés
Java - maven , JSON alapú adatkezelő. Celunk az esetlehges hibák feltárása.

### 1.1 Tesztelési terv hatóköre, célja:

- A tesztelési terv célja a tesztelés teljes körűségének biztosítása, a tesztelés során alkalmazott eljárások és megoldások meghatározásával.
- A teszt végrehajtásáért ez esetben a test manager fele (Kiss Milán), és a tesztelést azt általa összeállított tesztcsapat hajtja végre a 2.1. fejezetben meghatározott módon.

### 1.2 Elvárások
#### Az alábbi alap elvárások képezik ennek a teszttervnek az alapját:
- Az olvasó ismeri az alapdokumentumokat, amelyek meghatározzák a rendszert. 
- Az M&B egység / projektcsapat felelős a tesztadatok előállításáért.

## 2 Szükséges erőforrások
Ez a fejezet a teszteléshez szükséges erőforrásokat fejti ki.

### 2.1 Feladatkörök és felelősségek (tesztcsapat meghatározása)
| Feladatkör  |  Felelősség/tevékenység |  Személy  |
|---|---|---|
|  **Tesztelő, Teszt-koordinátor:** |  A teszt végrehajtása, észrevételek dokumentálása, teszt dokumentáció archiválása.Teszt terv készítése.  A tesztterv jóváhagyatása a projektmenedzserrel.  Teszt forgatókönyvek létrehozása  Inkonzisztenciák kezelése.  Helyes és időbeni hibakezelés.  Szükség esetén problémák eszkalálása a projekt menedzsernek.  Végső riport készítése.  Teszt dokumentum archiválása.  Az észrevételek státuszának követése, ill. dokumentálása |  Kiss Milán |
| **Szakértő:**  |  A szakértő az észrevételek elemzi és megoldást javasol. | Tolvaj Balázs |
|**Projektvezető:**| Teszt terv jóváhagyása  Teszt forgatókönyv (testscript)| Tolvaj Balázs |

### 2.2 Tesztkörnyezet
| Környezet neve és feladata  |  A hozzáférés módja | Konfiguráció  |
|---|---|---|
| Java - maven | Offline - Szabad szoftver | Linux kernel 5.3 |

### 2.3 Tesztadatok
A teszt végrehajtásához szükséges rekordok (tesztadatok) száma: 3
A tesztadatok elkészítéséért és feltöltéséért felelős személy: Kiss Milán

A tesztadatoknak az alábbi követelményeknek kell megfelelniük:
- Meg kell felenie annak hogy hibás adatokat ne lehessen felvinni.
- Minden reszt illetve adatbekérést meg kell adni anélkül ne lehessen továbblépni illetve feldolgozásra küldeni az adatot.

### 2.4 Leszállítandó teszt dokumentumok
Az összes teszt dokumentáció és leszállítandó a következő helyen érhető el: [LINK](https://github.com/afplabor2019/rip/tree/master/Main%20Project/Documents)

| Cím  |  Felelős személy | Szállítási gyakorisága  | Szállítás módja |
|---|---|---|---|
|  **Teszt terv:** |  Kiss Milán |  Egyszeri |  github repository |
|  **Teszt-esetek:** | Kiss Milán  |  Heti | github repository  |
|  **Tesztjegyzőkönyvek:** |  Kiss Milán |  Heti |  github repository |
|  **Tesztelési jelentés:** |  Kiss Milán |  2 Hetente  |  github repository |

### 2.5 Tesztelési eszközök
  - *Webstorm* [LINK](https://www.apachefriends.org/hu/index.html)
  - NPM [LINK](https://jigsaw.w3.org/css-validator/)

## 3 Tesztelési terv
Ez a fejezet leírja a teszt típusát, a metodológiáját és a riport készítés módszerét. Emellett meghatározza a teszt elvárásokat, a teszt-esetek elvárt eredményeit, sikerességének kritériumait, a kockázatok kezelését és a hatáskörön kívül eseteket.

### 3.1 Fejlesztői teszt
A fejlesztői tesztelés célja a rendszer alapvető funkcióinak ellenőrzése, a hibakezelés és az alapvető funkciók működésének vizsgálata
**Módszere:**
A tesztelés során többszöri ada tbevitellel van tesztelve a webalkalmazás.

### 3.2 Prototípus (modul) teszt
A prototípustesztelés (vagy másik nevén modultesztelés) célja a rendszer már működő moduljainak önálló tesztelése, a modulon belüli hibák azonosításának és kiküszöbölésének érdekében. 
**Módszere:** 
A program több egymásal összefügő, össze hangolt javascript kódszegmenekből épül fel amelyek mindegyik egy önálló fájl. A szegmensek validálása egyénileg történik. A tesztelés visszont a szegmensek föggőségeire is ki terjed.

### 3.3 Integrációs teszt
Az integrációs teszt célja a rendszer más rendszerekhez történő illesztésének vizsgálata, a több rendszereken keresztül átívelő funkciók tesztelésének érdekében. Az adatmigrációs tesztelés az integrációs teszteléshez tartozik, ennek lényege, hogy a bevezetendő rendszerbe áttöltik azokat az adatokat, amelyekkel a rendszer dolgozni fog és letesztelik a betöltött adatok, illetve az adatokat kezelő funkciók helyességét. 
**Módszere:**
A webalkalmazás többszöri hibás és helyes adatbevitelével teszteljük.

### 3.4 Elfogadási teszt
Az elfogadási teszt (angolul User Acceptance Test) célja a rendszer teljes funkcionalitásának vizsgálata a felhasználók szemszögéből
**Módszere:**
A teszt egy kontrol csoportal zajlik, egy külső cégen keresztül.

### 3.5 Terheléses teszt
A terheléses teszt célja a tervezett kapacitások, valamint a rendelkezésre álló növekedési potenciál meghatározása.
**Módszere:**
A próba telepítést követően egy meghívott teszt közönéggel zajlik, szimulálva egy átlagos napi használatot.

### 3.6 Biztonsági teszt (audit):
Biztonsági tesztelésre akkor van szükség, ha a rendszer szenzitív (pl. személyes vagy pénzügyi) adatokat kezel, vagy szabadon elérhető az internetről. 
**Módszere:**
A tesztett egy megbízott külső cég végzi.

### 3.7 Go live teszt
A go-live teszt egy próbaélesítés, melynek során a korábbi rendszerek továbbra is üzemelnek annak érdekében, hogy az élesítéskor keletkező problémák ne befolyásolják a normál üzemi működést.
**Módszere:**
A próba telepítés a megrendelő által választott webtárhelyen történik, a weboldalt a jövőben üzemeltető adminisztrátorok közreműködésével.

### 3.8 Tesztelési feladatok, teszt-esetek leírása
A tesztelési feladat a következő teszt-eseteket foglalja magában:
- Fejlesztői teszt
- Prototípus (modul)

## 4 Tesztelési ütemterv, függőségek – tesztforgatókönyv
### 4.1 Tesztelési jegyzőkönyv
A tesztelők a tesztforgatókönyvnek megfelelően elvégzik a tesztelést és az eredményt tesztjegyzőkönyvekben dokumentálják. A teszt kimenetelést minden esetben jelenteni kell a tesztkoordinátornak. A tesztkoordinátor a szakértőkkel együtt megoldást keres a problémákra, majd frissíti a tesztforgatókönyvet. Ha a problémát megoldották, a tesztelő újrakezdheti a tesztelést, majd dokumentálja az eredményeket. Ha a hiba továbbra is fennáll, és harmadik félen múlik a megoldása eszkalálni kell a problémát a projekt menedzsernek. 

### 4.2 Tesztelési jelentés
A tesztelési jelentést a tesztkoordinátor készíti el. Ez egy részletes áttekintése a lefutott teszteknek, azok eredményeinek, státuszának és a megjegyzéseknek.
A tesztkoordinátor juttatja el a projektmenedzsernek a tesztelési jelentést.

### 4.3 Tesztelt elvárások 
Az alábbi nem-funkcionális elvárások szerepelnek az üzleti illetve fejlesztői specifikációban, amelyek tesztelésre is kerültek: 
| #  | Leírás |
|---|---|
| 1. |  Alapvető program hibák kiszűrése |
| 2. |  Validációs hibák feltárása |
| 3. |  css hibák felderítése  |

### 4.4 Elfogadási kritériumok
- Technikai, a teszt forgatókönyvben leírtak szerint.
- A projekt menedzser jóváhagyása a teszt leszállítandókra

## 5 Tesztjegyzőkönyv
### 5.1 Tesztelési jegyzőkönyv - CSS

|   |   |
|---|---|
| A teszt-eset leírás és célja:  | Menü pontok és opciók ellenörzése, optimális CSS |
| A tesztelt folyamat/funkció leírása:  |  A teszt során lépésről lépésre tesztelésre kerülnek a menü pontok |
| A tesztelés előfeltételei:  |  A program és a dokumentáció ismerete |
| A tesztelés dátuma és időpontja:  |  2020.01.16 18:00 |
| A tesztadatok típusa:  | szöveg, dátum |
| A tesztet végző személy(ek):  | Kiss Milán  |
| A tesztelt rendszer beállításai:  | A program specifikációjában szereplő alap beálítások  |
| A teszt-eset elvárt eredménye:  |  Megfelelő formázás |
| A tesztelés eredménye:  | **Megfelelt** |
| Megjegyzések:  | Alapvető kinézet amit majd kérésre lehet változtatni. |

**Tesztelést elvégezte**
|   |   |
|---|---|
|  Név: |  Kiss Milán |
|  Szervezeti egység/ beosztás: | Test manager  |
|  Dátum: |  2020.01.15 21:00 |

### 5.2 Tesztelési jegyzőkönyv - CSS

|   |   |
|---|---|
| A teszt-eset leírás és célja:  | weboldal menüpontja tesztelése |
| A tesztelt folyamat/funkció leírása:  |  ha hibásan vagy tul hosszan irják be a telefonszámot nem fogadja el illetve ez az összes mezőre igaz.  |
| A tesztelés előfeltételei:  | Teszt adatokkal kell feltölteni |
| A tesztelés dátuma és időpontja:  |  2020.01.16 15:00 |
| A tesztadatok típusa:  | Szöveg vagy Dátum  |
| A tesztet végző személy(ek):  | Kiss Milán  |
| A tesztelt rendszer beállításai:  | A program specifikációjában szereplő alap beálítások  |
| A teszt-eset elvárt eredménye:  |  Megfelelő formázás|
| A tesztelés eredménye:  | **Megfelelt/élesíthető**  |
| Megjegyzések:  | -  |

**Tesztelést elvégezte**
|   |   |
|---|---|
|  Név: |  Kiss Milán |
|  Szervezeti egység/ beosztás: | Test manager  |
|  Dátum: |  2020.01.16 15:10 |

## 6 Tesztelési jelentés 

### 6.1 Tesztelési jelentés -  1. CSS
   |   |
|---|---|
| A hivatkozott tesztjegyzőkönyvek rövid leírása és eredménye:  | A menüpontok és opcioi megfeleltek a tesztnek |
| A tesztelt folyamatok/funkciók/modulok leírása: |  A teszt során lépésről lépésre tesztelésre kerültek a menü pontok.|
| A tesztadatok típusa:  | Szöveg vagy Dátum  |
| A tesztelt rendszer beállításai:  | A program specifikációjában szereplő alap beálítások  |
| A tesztelés eredménye:  | **Megfelelt**  |
| Megjegyzések:  | -  |

**Tesztelést elvégezte**
|   |   |
|---|---|
|  Név: |  Kiss Milán |
|  Szervezeti egység/ beosztás: | Test manager  |
|  Dátum: |  2020.01.15 21:30  |

### 6.2 Tesztelési jelentés -  2. CSS
   |   |
|---|---|
| A hivatkozott tesztjegyzőkönyvek rövid leírása és eredménye:  | weboldal menüpontja tesztelése" |
| A tesztelt folyamatok/funkciók/modulok leírása: |   A teszt során lépésről lépésre tesztelésre kerültek a menü pontok.  |
| A tesztadatok típusa:  | Szöveg vagy Dátum  |
| A tesztelt rendszer beállításai:  | A program specifikációjában szereplő alap beálítások  |
| A tesztelés eredménye:  | **Megfelelt**  |
| Megjegyzések:  | -  |

**Tesztelést elvégezte**
|   |   |
|---|---|
|  Név: |  Kiss Milán |
|  Szervezeti egység/ beosztás: |  Test manager  |
|  Dátum: |   2020.01.15 21:15  |

### 7 Jóváhagyások

|   |   |
|---|---|
|  Név: |  Tolvaj Balázs |
|  Szervezeti egység/ beosztás: | Programtervező  |
|  Dátum: |  2020.01.16 19:00  |