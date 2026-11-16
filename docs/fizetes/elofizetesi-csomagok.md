---
title: Előfizetési csomagok létrehozása
description: Az előfizetési csomagok az árképzési tervek – havi, éves vagy egyszeri fizetéses opciókkal, amelyek hozzáférést biztosítanak a fizetős tartalmakhoz.
sidebar_position: 2
---

## Mi ez?

Az előfizetési csomagok az árképzési terveid – meghatározod, mennyiért és milyen időszakra (havi, éves, egyszeri) férhetnek hozzá a tagok a fizetős tartalmakhoz. Egyszerre több csomag is aktív lehet: pl. egy havi és egy éves opció párhuzamosan.

## Előfeltételek

> ⚠️ Mielőtt elkezded:
> - A Stripe-nak összekapcsoltnak kell lennie. Lásd: [Stripe beállítása és összekapcsolása](./stripe-beallitas).

## Lépésről lépésre

1. Lépj az **Admin → Előfizetések** oldalra.
2. Kattints az **„Új csomag"** gombra.
3. Add meg:
   - **Név** (pl. „Havi tagság" vagy „Éves Pro csomag")
   - **Leírás** – ez megjelenik a fizetési oldalon
   - **Ár** – forintban (Ft) vagy euróban (EUR) megadva
4. Válaszd ki a **számlázási időszakot:**
   - **Havi** – visszatérő havi fizetés
   - **Éves** – visszatérő éves fizetés (kedvezmény adható)
   - **Egyszeri** – egyszeri vásárlás, örökre szóló hozzáféréssel
5. Kattints a **Mentés** gombra.

![Előfizetési csomagok kezelése](./screenshots/elofizetesi-csomagok.png)

## Lemondási kérelmek kezelése

A tag a **Profilom → Előfizetésem** felületen az **Előfizetés lemondása** gombbal nyitja meg a kapcsolati ablakot. Az **E-mailt írok** gomb előre kitöltött levelet nyit a levelezőjében, a tag nevével, e-mail-címével és csomagjával. A tagnak ezt a levelet még el kell küldenie; a gomb megnyomása önmagában nem mondja le az előfizetést.

A lemondást a közösség adminisztrátora intézi. A kapcsolati ablak a közösséghez beállított ügyfélkapcsolati címet mutatja, ennek hiányában az **Admin → E-mailek** válaszcímét. Ha nincs megadott cím, az ablak a közösség adminisztrátorához irányítja a tagot.

Az aktív, rendezett előfizetés lemondásakor a hozzáférés a kifizetett időszak végéig megmarad. Lejárt, sikertelen megújításnál az admin azonnal lemondhatja az előfizetést; ekkor a fizetős hozzáférés is megszűnik.

A tag közösségből való eltávolítása lezárja a hozzáféréseit, de az élő Stripe-előfizetését külön kell lemondani, hogy ne folytatódjon a terhelés.

## Tippek

- Éves csomaghoz kedvezmény állítható be – mutasd meg a tagoknak, mennyit spórolnak az éves előfizetéssel a havihoz képest.
- Egyszerre több csomag is aktiválható – pl. egy havi és egy éves lehetőség is kínálható párhuzamosan.
- A csomag törlése nem törli az aktív előfizetőket – ők a következő megújítási időpontig hozzáférnek a tartalmakhoz.

## Kapcsolódó cikkek

- [Paywall konfigurálása](./paywall)
- [Fizetős kurzus beállítása](../kurzusok/fizetos-kurzus)
