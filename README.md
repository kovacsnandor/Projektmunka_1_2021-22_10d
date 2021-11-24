# Projektmunka_1_2021-22_10d
Projektmunka leírások
## Általános feladatok
- Feladatok szétosztása
- Projektnapló vezetés
- GitHub elkészítése
    - Readme.md (ide kerül a műszaki leírás)
    - források gyűjtése (`sources` mappa)
- Kapcsolási rajzok (fritzing)
    - Sematikus rajz
    - Bekötési rajz
- Áramkör megépítése a próba panelen
- Program fejlesztés
    - Program elkészítése kis lépések módszerével:
        - Módosítás - Tesztelés ciklus
- Prezentáció készítés a feladatról
- Prezentáció megtartása
    - Élő előadás
    - Videofelvétel
    - Előadások megbeszélése
- Értékelés
    - Felelés (teszt)    


### Projektnapló vezetés

### 

# Fényerő szabályzás potméterrel
## Csoporttagok
- Nagy Ferenc (csoportvezető)
- Polyák Alex János
## Feladat leírása
Pulzusszélesség alapon működő ledes fényerő szabályzó modell elkészítése.
- A ledet a GPIO PWM üzemmódban hajtsa meg közvetlenül egy megfelelő korlátozó ellenállással
- Szabálzó eszköz: potméter
- Szabályzási elv: 
    - A potméter áramát mérő A/D: [INA219 DC IUP mérő](https://malnapc.hu/a904-ina219-high-side-dc-current-sensor-aram-szenzor) átalakító által előállított áramtartomány érzékelése.
    - Az áramtartomány [0, 100] tartományra normálása
    - A kitöltési tényező folymatos állítása a normált tartomány segítségével.

# Fényerő szabályzás nyomógombbal
## Csoporttagok
- Molnár Krisztián (csoportvezető)
- Ledacs-Kiss Bence
## Feladat leírása
Pulzusszélesség alapon működő ledes fényerő szabályzó modell elkészítése.
- A ledet a GPIO PWM üzemmódban hajtsa meg közvetlenül egy megfelelő korlátozó ellenállással
- Szabályzó eszköz: nyomógombok (mikrokapcsolók)
    - 1. kapcsoló: fényerő növelés (egyedi és folyamatos nyomással)
    - 2. kapcsoló: fényerő csökkentés (egyedi és folyamatos nyomással)
    - 3. kapcsoló: max fényerő ki-be kapcsolás
- Szabályzási elv: 
    - A kapcsolók egyedi vagy folamatos nyomásának impulzus számlálsa [0, 100] tartományra limitálva.
    - A kitöltési tényező folymatos állítása a tartomány segítségével.

# Távolságmérő
Fehér György Márk
Juhász Gergő

## Feladat leírása

Ultrahangos távolságmérő készítése az [ULTRAHANGOS TÁVOLSÁGSZENZOR HC-SR04-4P](https://malnapc.hu/ultrahangos-tavolsagszenzor-hc-sr04-4p) szenzor segítségével.
A távolságmérő egy nyomógomb segítségével egy memóriába tárolja el a beadott távolságokat, valmint mutassa egy hétszegmenses kijelzőn: [A881 0.56 INCH CLOCK DISPLAY W/I2C BACKPACK - BLUE](https://malnapc.hu/a881-0-56-inch-clock-display-wi2c-backpack-blue)
- 1. nyomógomb: távolság rögzítése
- 2. nyomógomb: Memória törlése
- 3. nyomógomb: a memóriában tárolt távolságok váltása a hétszegmenses kijelzőn
- 4. nyomógomb: Az utolsó két mérési adat alapján számoljon területet
- 5. nyomógomb: Az utolsó három mérési adat alapján számoljon térfogatot

# Hőmérséklet szabályzó
## Csoporttagok
- Jáger Kristóf (csoportvezető)
- Suki Zsolt
## Feladat leírása
- A [DS18B20+](https://malnapc.hu/ds18b20) 1-wire (egyvezetékes) digitális hőmérséklet érzékelők egy vezetékre felfűzött (4-5 db) láncának segítségével szimulálja, hogy ezek különböző helyiségek, dolgok hőmérsékletét mérik.
- Egy kapcsoló segítségvével lehessen váltatni, hogy melyik érzékelő hőmérsékletét mutatja a 7 szegmenses kijelző: [A881 0.56 INCH CLOCK DISPLAY W/I2C BACKPACK - BLUE](https://malnapc.hu/a881-0-56-inch-clock-display-wi2c-backpack-blue)
- A hőérzékelőknél legyen egy led, ami mutatja, melyik hőmérséklete van éppen kijelezve
- A kiválasztott hőrzékelő a beprogramozott hőmérséklet határ alatt kapcsolja be a fűtést, felett pedig ki. A hiszterézis legyen 0.5 °C.
- Legyen porgramozható a hőmérséklet határ.
- Programzó gombok:
    - 

# U,I,P,R mérő
## Csoporttagok
- Hajdu István (csoportvezető)
- Kovács Levente
## Feladat leírása
A [INA219 DC IUP mérő](https://malnapc.hu/a904-ina219-high-side-dc-current-sensor-aram-szenzor) árammérő szenzor segítségével készítsen egy:
- Feszülség
- Áram
- Teljesítmény
- Ellenállás

mérő eszközt, ami egy 7 szegmenses kijelzőn mutatja az értékeket: [A881 0.56 INCH CLOCK DISPLAY W/I2C BACKPACK - BLUE](https://malnapc.hu/a881-0-56-inch-clock-display-wi2c-backpack-blue)
Egy nyomógomb segítségével lehessen váltani a különböző funkciók között.
A különböző funkciókhoz legyen egy dugalj elrendezés, ami meghatározza, hogy mit lehet vele mérni.

# Bicikli lámpa RGB leddel
## Csoporttagok
- Fehér Zsolt Dorián (csoportvezető)
- Kocsis Bence
## Feladat leírása
Az alkatrész csomagban található [RGB led(ek)](https://www.hestore.hu/prod_10037597.html) segítségével szimuláljon egy biciklilámpát
- 1. kapcsoló: Első vagy hátsó lámpa üzemmód
- 2. kapcsoló: Az üzemmódon belüli váltás

- Első lámpa üzemmód állapotok
    1. Fehér erős fény
    2. Fehér gyengébb fény
    3. Kikapcsolva
- Hátsó lámpa üzemmód állapotok
    1. Folyamtos vörös
    2. Villogó vörös
    3. Kikapcsolva 

# Közlekedési lámpa
## Csoporttagok
- Medgyes Csaba (csoportvezető)
- Oláh Péter
- Kovács János
## Feladat leírása
Egy kereszteződés autóforgalmi és gyalogos átkelőhely közlekedési lámpáit szimuláló rendszer elkészítése 5 megfelelő színű ledsorral.
- [A feladat részletes leírása](http://labtoll.hu/raspberry/algoritmus.html#algoritmus)

