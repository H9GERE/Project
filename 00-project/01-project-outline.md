---
name: Villányi Olivér
neptun: H9GERE
id: 2026-OG-02
github: https://github.com/H9GERE
github_project: https://github.com/H9GERE/Project.git
---
# Konzisztens dinamikus játékvilág megvalósítása nagyméretű nyelvi modellekre épülő szöveges kalandjátékban

A projekt egy AI-alapú szöveges kalandjáték megvalósítása, amely egy nagyméretű nyelvi modell (LLM) segítségével dinamikusan generálja a narratívát a játékos döntései alapján. A legnagyobb kihívást a játékvilág konzisztenciájának fenntartása jelenti a hosszabb játékmenetek során. A projekt végére a játékos egy letisztult felhasználói felületen keresztül hozhat döntéseket, miközben a rendszer a világ fontos állapotait egy különálló, strukturált, determinisztikus modellben kezeli, és tartósan eltárolja a játék haladását.

## Célok

- **Elsődleges cél:** Egy olyan LLM-alapú szöveges kalandjáték elkészítése, amely képes hosszú távon is fenntartani a játékvilág logikai konzisztenciáját.
- **Célfelhasználók / érintettek:** Szöveges és szerepjátékok kedvelői, valamint az AI-alapú játékkészítés iránt érdeklődők.
- **Mérhető sikerkritériumok:** A játékos döntéseket hozhat és történetet alakíthat; a világállapot (helyszínek, karakterek, tárgyak) újratöltés után is észrevehető logikai ellentmondások nélkül, tartósan tárolva és megjelenítve marad.
- **Korlátok:** Strukturált determinisztikus modell; LLM API-kommunikáció; perzisztens adattárolás; hitelesítő adatok és API-kulcsok nem kerülhetnek a repóba.

## Hatókör

### Benne van a hatókörben

- Szöveges kalandjáték indítása, mentése és betöltése a felhasználói felületen.
- Játékos döntéseinek és szabad szöveges vagy opcióalapú inputjainak feldolgozása.
- Dinamikus narratívagenerálás LLM segítségével.
- A világállapot (szereplők, helyszínek, tárgyak) változásainak strukturált kinyerése és determinisztikus validációja.
- Reszponzív, letisztult webes vagy asztali felhasználói felület.

### Nincs benne a hatókörben

- Többjátékos játékmód.
- Grafikus 2D/3D játékvilág-megjelenítés.
- Online ranglisták vagy közösségi funkciók.

## Jegyzetek

Az első prototípus két memóriakezelési stratégiát hasonlít össze (pl. kontextus-összegzés és vektoriális/RAG-alapú keresés). Összetettebb történetszálak és világméretek csak akkor merülhetnek fel, ha az alap játékkör és az állapotkonzisztencia már megbízhatóan működik.
