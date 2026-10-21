<!-- @slide Cím -->

# Konzisztens dinamikus játékvilág megvalósítása LLM-alapú szöveges kalandjátékban

<!-- @gap 3 -->

<!-- @set-align left -->

Szerző: **Villányi Olivér**

Neptun: **H9GERE**

Projektvezető: **Oláh Gábor**

Projektazonosító: **2026-OG-02**

---

<!-- @slide Probléma -->

# Probléma

<!-- @set-align left -->

- A nagyméretű nyelvi modellek (LLM) képesek dinamikusan generálni a narratívát a játékos döntései alapján, de a hosszú játékmenetek során komoly kihívást jelent a játékvilág konzisztenciájának fenntartása.
- Az LLM-ek hajlamosak "elflejteni" korábbi eseményeket, vagy logikai ellentmondásokba keveredni a világ állapotát illetően.
- Szükség van egy olyan hibrid rendszerre, amely a szabad narratívát ötvözi egy különálló, strukturált és determinisztikus modell megbízhatóságával.

---

<!-- @slide Célfelhasználók -->

# Célfelhasználók

<!-- @set-align left -->

- **Szöveges és szerepjátékok kedvelői**, akik egyedi, dinamikusan alakuló történetekre vágynak kötöttségek nélkül.
- **Az AI-alapú játékkészítés iránt érdeklődők**, akik szeretnék látni a generatív AI és a hagyományos játéklogika integrációját.

---

<!-- @slide Tervezett hatókör -->

# Tervezett hatókör

<!-- @set-align left -->
<!-- @columns 2 5 -->

## Benne van

- Játék indítása, mentése és betöltése a felületen.
- A játékos döntéseinek és szabad szöveges/opcióalapú inputjainak feldolgozása.
- Dinamikus narratívagenerálás LLM segítségével.
- A világállapot-változások strukturált kinyerése és determinisztikus validációja.
- Reszponzív, letisztult webes vagy asztali UI.

<!-- @col-break -->

<!-- @slide Nincs benne -->

## Nincs benne

- Többjátékos (multiplayer) játékmód.
- Grafikus 2D vagy 3D játékvilág-megjelenítés.
- Online ranglisták és közösségi funkciók.

---

<!-- @slide Kezdeti felhasználói utak -->

# Kezdeti felhasználói utak

<!-- @set-align left -->

1. **Játékkezdés és döntések:** A játékos elindítja a történetet, szabad szöveges választ ad meg, a rendszer pedig az LLM segítségével továbbfűzi a cselekményt.
2. **Állapotváltozás:** A játékos valahogy a világgal kölcsönhatásba lép; a háttérben futó determinisztikus modell frissíti az eseménytárat, és validálja.
3. **Mentés és Betöltés:** A játékos elmenti a haladást, majd egy későbbi időpontban pontosan ugyanabban a konzisztens világállapotban folytatja a játékot.

---

<!-- @slide Következő lépések -->

# Következő lépések

<!-- @set-align left -->

- **Memóriakezelési stratégiák összehasonlítása:** A kontextus-összegzés és a vektoriális keresés tesztelése az első prototípusban.
- **Alap játékkör stabilizálása:** Az állapotkonzisztencia és a core loop megbízható működésének elérése.
- **Világméretek növelése:** Összetettebb történetszálak és nagyobb világok bevezetése, miután az alapok már szilárdak.
