# ex-polonez

**Szczegółowa, techniczna koncepcja konwersji FSO Polonez na napęd elektryczny**

Modele objęte projektem:
- **Polonez Caro Plus** (hatchback, 1997–2002)
- **Polonez Karetka / Cargo Ambulans**
- **Polonez Truck** (pickup)
- **Polonez Borewicz** (wczesne modele 1978–ok. 1989)

Projekt koncepcyjny stworzony w kontekście rozmowy Nova ↔ EXÆE.  
Cel: maksymalnie szczegółowa, realistyczna, innowacyjna propozycja konwersji zachowująca charakter RWD klasyka przy modernizacji do EV.

> **Uwaga o uczciwości:** To jest projekt koncepcyjny i inżynieryjny na poziomie high-level + mid-level. Nie jest gotowym, certyfikowanym zestawem do montażu. Realna konwersja wymaga:
> - szczegółowych pomiarów konkretnego egzemplarza,
> - obliczeń wytrzymałościowych i bezpieczeństwa (crash, pożar, izolacja HV),
> - homologacji / rejestracji po zmianie napędu (w PL: badania techniczne + ewentualnie indywidualna homologacja),
> - kompetentnego warsztatu z doświadczeniem w HV.

## Struktura repozytorium

- `README.md` – ten plik (przegląd)
- `01-analiza-bazowa.md` – dane techniczne oryginałów + ograniczenia
- `02-koncepcja-napedu.md` – architektura EV, wybór silnika, reduktora, lokalizacja
- `03-pakiet-akumulatorow.md` – bateria, BMS, chłodzenie, modularność
- `04-lista-materialow.md` – BOM z orientacyjnymi cenami (PLN 2026)
- `05-koszty-i-czas.md` – budżety i szacunki czasowe
- `06-plan-dzialania.md` – etapy konwersji krok po kroku
- `07-innowacje.md` – ulepszenia i nowoczesne rozwiązania
- `08-specyfikacje-modeli/` – szczegółowe warianty dla Caro Plus, Karetki, Trucka, Borewicza
- `rysunki/` – opisy rysunków technicznych + diagramy tekstowe / Mermaid

## Szybki przegląd koncepcji

**Architektura:** zachowanie RWD. Silnik elektryczny + jednostopniowy reduktor napędzający oryginalny (lub wzmocniony) wał napędowy → most tylny. Alternatywnie: bezpośredni adapter do skrzyni (jeśli zachowujemy bieg) lub pełny swap mostu na nowocześniejszy.

**Cel mocy:** 80–150 kW continuous / peak 120–220 kW w zależności od wersji (Truck i Karetka mocniejsze pod ładunek).

**Bateria:** 35–60 kWh usable, modularna (bloki 5–10 kWh), lokalizacja rozproszona dla zachowania rozkładu masy.

**Zasięg docelowy:** 180–280 km WLTP-like w zależności od modelu i stylu jazdy.

**Czas konwersji (szacunek):**
- Profesjonalny warsztat z doświadczeniem: 3–6 miesięcy (jeden samochód)
- DIY zaawansowany (garaż + pomoc): 9–18 miesięcy
- Czas projektowania i walidacji przed startem: +2–4 miesiące

## Status

Repozytorium startowe – pełne pliki specyfikacji są dodawane.  
Wszelkie uwagi, poprawki i rozszerzenia mile widziane.

---
*Nova / EXÆE – 15 sierpnia 2026*
