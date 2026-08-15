# ex-polonez

**Szczegółowa, techniczna koncepcja konwersji FSO Polonez na napęd elektryczny**

Modele: Caro Plus · Karetka/Cargo · Truck · Borewicz

**Aktualne domyślne podejście (od 15.08.2026): Maintainability First**  
Cała architektura została przeprojektowana pod kątem łatwości naprawy i serwisu (moduły kasetowe baterii, power pack jako jeden blok, Service Box, quick-disconnecty, dokumentacja w aucie).

> To nadal projekt koncepcyjny. Realna realizacja wymaga pomiarów konkretnego egzemplarza, obliczeń i kompetentnego warsztatu HV.

## Decyzja strategiczna

Po analizie trzech ścieżek:
- konwersja istniejącego dawcy
- kupno samej karoserii
- budowa od zera (spaceframe + panele)

**Pozostajemy przy konwersji solidnego dawcy**, bo daje najlepszy stosunek koszt / czas / legalność / charakter.  
Full custom chassis zostaje opcją na osobną gałąź, jeśli celem będzie prototyp lub pojazd poza standardową rejestracją drogową.

Szczegóły w pliku `09-maintainability-first.md`.

## Struktura repozytorium

- `01`–`08` – analizy bazowe, napęd, baterie, koszty, plany, innowacje, specyfikacje modeli
- `09-maintainability-first.md` – **kluczowy** – nowe zasady projektowe
- `10-safety-checklist.md` – checklisty bezpieczeństwa i serwisowe
- `11-homologacja-i-hv.md` – ścieżka legalizacji + schemat HV
- `rysunki/` – opisy i diagramy

## Szybki przegląd (Maintainability First)

- Silnik + reduktor = jeden wymienny **power pack**
- Baterie = **kasety** 5–10 kWh z szybkozłączami
- Centralny **Service Box** (BMS, styczniki, diagnostyka)
- Dostęp serwisowy zaprojektowany z góry i z boków
- Pełna dokumentacja + QR w aucie

Cel mocy i zasięgu bez zmian (80–150 kW, 180–280 km).

## Status

Projekt żywy. Maintainability First jest teraz baseline.

---
*Nova / EXÆE*
