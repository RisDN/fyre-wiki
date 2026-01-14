---
sidebar_position: 7
description: Itt minden hasznos infót megtalálsz, ami a Gens Tycon szerverrel kapcsolatos!
---
# 🪷 Gens Tycoon

### Mi az a Gens Tycoon?

> A **Gens Tycoon** szerver egy farmolásra alapuló, hosszú távon is élvezhető játékmód. Ha farmolásra, generátorokra, : ***itt az idő, csatlakozz!***

#### Általános cél: Generátoraid, kapdád segítségével pénzt szerezni, és a ranglisták élére kerülni.

---

### 1.Rendszerarchitektúra áttekintése

- erőforrás termelő rendszer: Generátor(ok) (Generators)
- hosszú távú gazdasági és elszámoltatási rendszer(ek)
- haladási, kritérium alapú metarendszerek

***Ezek egymáson alapuló rendszerek, mely a játékos előrehaladásának számszerűsíthető változókként határozza meg.***

---

### 2. Erőforrás termelő rendszer
#### 2.1 Generátor definíció
- A **generátor** egy olyan "entitás", mely:
    - meghatározott időintervallumban termel bizonyos mennyíségű erőforrást
    - fejleszthető, ami bővebb tárgylistai lehetőséget ad a játékosoknak
    - fix, vagy skálázott mennyiségű erőforrást állít elő

*A termelés függ a játékos aktív jelenlététől is.*

#### 2.2 Generátor paraméterei
- A **generátor** a következő tulajdonságokkal rendelkezik:
    - termelési ciklusidő
    - kibocsátott tárgy típúsa
    - kibocsátott tárgy mennyisége
    - gazdasági érték
    - szint / fejletségi állapot

---

### 3. Terület,- és kapacitás kezelés
#### 3.1 Tycoon terület (Island)
- Minden játékos egy **dedikált területnek** örülhet, mely:
    - elkülöníti más játékosoktól
    - saját generátorai elheyezésére szolgál
    - külön kapacítás korlátokkal rendelkezik

*Ez a terület a játékos képzelete szerint is alakítható, szabad kezet kap bizonyos szabályok mellett.*

#### 3.2 Slot rendszer
- A slot rendszer korlátok közt alkalmazható. A korlátok a következőek:
    - maximálisan elhelyezhető generátor szám
    - területhez kötött kapacítás
- A slotok száma növelhető:
    - ládák, jutalmak álltal szerzett voucherek segítségével
    - metaszintekkel

*A játékos aktívan töltött ideje segíti ez növekedését is.*

---

### 4. Gazdasági modell
#### 4.1 Valutarendszer
- A játékmód több valutát alkalmaz (elixír, FyreCoin, és a megszokott egyenleg), amelyek:
    - különböző funkciókra használhatóak (fejlesztés, kereskedés)
    - egymással nem minden esetben konvertálhatóak (kivétel a játékosokkal való kereskedés)

#### 4.2 Ármeghatározás
- Az erőforrás értéke függ a **játékos**októl is, de az alap értékek:
    - statikus árlista alapján
    - vagy dinamikus ármeghatározási model 
*alapján kerül meghatározásra.*

#### 4.3 Elszámolás
- Az elszámolás történhet:
   - manuális eladással
   - automatizált rendszereken keresztül
   - játékosokkal való kereskedés során

---

### 5. Haladási és metarendszerek
#### 5.1 Szintezés
- A szintek:
   - funkciók feloldását
   - hatékonyság,- és kapacításnövelést 
*biztosítanak.*

#### 5.2 Prestige rendszer
- A prestige:
   - ciklikus haladási modell
   - reseteli az alrendszerek egy meghatározott részét
   - permanens bónuszokat is biztosíthat bizonyos esetekben

---

### 6. Kiegyensúlyozás és korlátozások
- A rendszerek következőképp biztosítják az egyensőlyt:
   - magas felső határ
   - csökkenő hozam
   - időalapú korlátok

---

### 7. Ranglisták és összehasonlítás
- A ranglisták objektív mutatók alapján működnek:
   - összvagyon (egyenleg, elixír)
   - haladási szint
   - kiütött növényi mennyiség

---

### 8. Szezonális struktúra
- A játékmód időszakos szezonra van bontva, mely:
   - teljes statisztikai resetet alkalmaz
   - új paraméterezést, frissítést vezethet be

---

### 9. Terminológia
   - Generátor(ok) (Generators) - időalapú erőforrás-termelő egység
   - Slot - kapacításkorlát
   - Prestige - ciklikus haladási szint


### 10. Tippek / Hasznos parancsok
#### 10.1 Kezdő, alap parancsok:
- Az alábbi parancsok segítséget nyújtanak a játék elkezdéséhez:

| Parancs     | Használhatóság                                        | 
|-------------|-------------------------------------------------------|   
| /genshop    |Generátor vásárlási menü                               |           
| /is create  |Saját szigeted létrehozása                             |
| /is disband |Szigeted feloszlatása                                  |
| /is leave   |Sziget elhagyása                                       |    
| /is invite  |Más játékos meghívása szigetedre                       |
| /is accept  |Meghívó elfogadása más játékostól (sziget)             |
| /is panel   |Sziget panel megnyitása (megtalálható minden beállítás)|
| /is balance |Sziget / Játékos bankjának megtekintése                |
| /is ban     |Játékos kitiltása szigetedről                          |    
| /is unban   |Játékos kitiltásának megvonása                         |
| /is bank    |Sziget bankjának megnyitása                            |
| /is biome   |Sziget biomjának megváltoztatása                       | 
| /is border  |Szigeted borderének színváltoztatása                   | 
| /is chest   |Sziget ládájának megnyitása / megtekintése             |
| /is visit   |Más szigetének meglátogatása                           | 
| /is close   |Szigeted bezárása a látogatók elől                     | 
| /is coop    |Sziget segítő hozzáadása                               | 
| /is uncoop  |Sziget segítő eltávolítása                             | 

---

### Összegzés
- A FyreMC Gens Tycoon játékmódja egy **determinista**, **skálázható gazdasági rendszer**, amely passzív termelésre, és hosszútávú optimalizálásra épül a játékélményt megtartva.

:::warning
- Minden season (szezon) végén az összes játékos egyenlege, generátora, és tárgya, valamint szigete is eltűnik. A season lezárás lényege az új kezdet, nem az érték elvesztése.
:::