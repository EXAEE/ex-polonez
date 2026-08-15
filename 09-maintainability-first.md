# 09. Maintainability First – przeprojektowanie koncepcji

## Decyzja strategiczna (uczciwa ocena)

Przed dalszym rozwijaniem konwersji sprawdziłem trzy ścieżki:

### 1. Konwersja istniejącego Poloneza (dawca)
**Zalety:** najtańsza i najszybsza droga do jeżdżącego, zarejestrowanego pojazdu. Zachowana „dusza” i historia. Procedura zmiany napędu w PL jest relatywnie znana (opinia rzeczoznawcy + badanie + wpis).
**Wady:** korozja, ograniczenia strukturalne starej karoserii, ukryte koszty napraw blacharskich.

### 2. Kupno samej karoserii / gołej skorupy
**Ocena:** zwykle najgorsza opcja. Rzadkość, transport, nadal stara struktura, a i tak trzeba projektować cały napęd i mocowania od zera. Mało korzyści przy wysokim ryzyku.

### 3. Budowa od zera (spaceframe + panele wizualnie wzorowane na Borewiczu lub własny design)
**Zalety:** pełna kontrola nad maintainability, nowoczesna sztywność, optymalne rozmieszczenie baterii, dostęp serwisowy zaprojektowany od początku.
**Wady:** znacznie wyższy koszt i czas. Homologacja indywidualna **nowego** pojazdu w PL/EU jest istotnie trudniejsza i droższa niż zmiana napędu w istniejącym aucie. Realistyczny koszt dobrze zrobionego, bezpiecznego one-off łatwo przekracza 250–400k+ PLN.
**Sensowna gdy:** celem jest prototyp, pojazd torowy/wystawowy, lub długoterminowy projekt rozwojowy z własną marką.

**Wniosek na teraz:**  
Dla większości zastosowań (użytkowe + charakter Poloneza) **pozostajemy przy konwersji solidnego dawcy**, ale **całkowicie przeprojektowujemy architekturę pod kątem łatwości naprawy i serwisu**.  
Jeśli później zechcesz iść w full custom chassis – wtedy robimy osobną gałąź projektu.

---

## Nowe zasady projektowe (Maintainability First)

1. **Modularność agresywna**  
   Każdy większy podzespół ma być wymienialny jako jednostka bez demontażu sąsiednich systemów.

2. **Dostęp z góry i z boków**  
   Unikamy wszystkiego, co wymaga podnoszenia całego auta lub demontażu podłogi do typowych czynności serwisowych.

3. **Quick-disconnect wszędzie gdzie bezpieczne**  
   HV, cooling, data, 12V – standardowe, oznaczone złącza.

4. **Jeden „crate” napędowy**  
   Silnik + reduktor + część elektroniki mocy jako jeden blok z własnymi punktami mocowania i złączami.

5. **Baterie w kasetach**  
   Bloki 5–10 kWh w sztywnych kasetach z uchwytami, prowadnicami i szybkozłączami. Możliwość wyjęcia jednego bloku w <30 min przy podstawowych narzędziach.

6. **Centralna skrzynka serwisowa**  
   BMS master, styczniki, bezpieczniki HV, DC-DC, diagnostyka – w jednej, łatwo dostępnej obudowie (najlepiej w komorze lub pod siedzeniem z klapą).

7. **Dokumentacja w aucie**  
   QR kody przy każdym module prowadzące do konkretnych procedur w repo + lokalna kopia PDF/USB.

8. **Preferencja ekosystemu części**  
   Tam gdzie możliwe – komponenty z istniejącym rynkiem wtórnym (moduły popularnych marek, standardowe złącza Amphenol/TE, pompy chłodzące z EV itp.).

9. **Serwis 1-osobowy lub 2-osobowy**  
   Typowe czynności (wymiana bloku baterii, pompy, styku, kontrola izolacji) mają być możliwe bez podnośnika warsztatowego lub z minimalnym sprzętem.

10. **Przewidywalne punkty awarii**  
    Wszystko co się zużywa (uszczelnienia, łożyska mostu, pompy, styczniki) ma być dostępne bez ruszania baterii.

---

## Konkretne zmiany w architekturze

### Napęd
- Silnik + reduktor montowane jako jeden „power pack” na wspólnej ramie adapterowej.
- Rama adapterowa ma szybkie mocowania (np. 4–6 śrub + kołki pozycjonujące).
- Złącza HV i cooling wychodzą w jedno miejsce – „dock”.

### Baterie
- System kasetowy. Każda kaseta ma:
  - własne złącze HV (high-current + interlock)
  - złącze cooling (szybkozłącza cieczy)
  - złącze danych/BMS slave
  - uchwyty i prowadnice
- Możliwość pracy z obniżoną pojemnością (jeden blok wyjęty) – oprogramowanie to obsługuje.

### Chłodzenie
- Pompa i zbiornik wyrównawczy w łatwo dostępnym miejscu w komorze.
- Odpowietrzniki i zawory serwisowe oznaczone i dostępne.
- Możliwość spuszczenia obiegu bez demontażu baterii.

### Elektronika
- Centralny „Service Box” z klapą.
- Diagnostyka OBD-style + dedykowany port do BMS.
- Wszystkie bezpieczniki HV w jednym miejscu.

### Most i wał
- Most pozostaje, ale z łatwym dostępem do łożysk i uszczelniaczy.
- Wał z łatwo demontowalnymi przegubami.

### Hamulce i zawieszenie
- Tarcze + zaciski z dobrym dostępem.
- Regeneracja nie może utrudniać wymiany klocków/tarcz.

---

## Konsekwencje dla kosztów i czasu

Maintainability First nieco podnosi koszt materiałów (lepsze złącza, kasetowy system, solidniejsze ramy adapterowe) – szacunkowo +8–15k PLN.  
Zwraca się przy pierwszej poważniejszej naprawie lub wymianie bloku baterii i dramatycznie obniża ryzyko „projektu, którego nikt nie chce ruszać”.

Czas projektowania rośnie (trzeba zaprojektować kasetę i docki), ale czas późniejszego serwisu spada mocno.

---

## Następne kroki w repo

- Zaktualizowane schematy z uwzględnieniem modularności
- Checklist serwisowy
- Procedury wymiany kluczowych podzespołów
- Szczegółowy schemat HV z punktami serwisowymi

To podejście traktuję teraz jako domyślne dla całego projektu ex-polonez.
