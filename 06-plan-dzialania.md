# 06. Plan działania – etapy konwersji

## Faza 0: Przygotowanie (1–4 tygodnie)

1. Wybór konkretnego egzemplarza (stan, korozja, kompletność dokumentacji).
2. Pełna diagnostyka mechaniczna i elektryczna oryginału.
3. Pomiar mas (najlepiej na wagach najazdowych) – rozkład przód/tył/lewo/prawo.
4. 3D skan lub szczegółowe pomiary komory silnika, tunelu, bagażnika.
5. Decyzja: budżet, cel (zasięg vs moc vs autentyczność), poziom odwracalności.
6. Zakup kluczowych komponentów z długim lead time (baterie, silnik).

## Faza 1: Demontaż i przygotowanie nadwozia (2–4 tygodnie)

1. Usunięcie silnika, skrzyni, wału, zbiornika paliwa, wydechu, chłodnicy, osprzętu.
2. Czyszczenie komory i podwozia, ocena korozji.
3. Naprawy blacharskie + zabezpieczenie antykorozyjne (krytyczne).
4. Wzmocnienie punktów mocowania silnika i konstrukcji nośnej baterii.
5. Demontaż lub modernizacja zawieszenia i hamulców.

## Faza 2: Fabrication (3–6 tygodni)

1. Projekt i wykonanie adapterów silnika / reduktora.
2. Konstrukcja obudów i mocowań baterii (crash-safe).
3. Modyfikacja tunelu / podłogi jeśli potrzeba.
4. Przygotowanie instalacji HV (trasowanie, osłony).
5. Adaptery do mostu / wału.

## Faza 3: Montaż napędu i baterii (3–5 tygodni)

1. Montaż silnika + reduktora + chłodzenia.
2. Montaż pakietów baterii + BMS.
3. Podłączenie HV, styczników, wyłączników.
4. Montaż wału i mostu (po przeglądzie).
5. Instalacja DC-DC, ładowarki, gniazda.

## Faza 4: Systemy niskonapięciowe i integracja (2–3 tygodnie)

1. Nowa instalacja 12 V / oświetlenie / sygnały.
2. Integracja deski rozdzielczej / wyświetlacza SoC / mocy.
3. Systemy bezpieczeństwa (crash cut-off, izolacja).
4. Klimatyzacja / ogrzewanie PTC.
5. Testy izolacji, ciągłości, komunikacji CAN.

## Faza 5: Uruchomienie, strojenie, testy (2–4 tygodnie)

1. Pierwsze uruchomienie na podnośniku (bez kół lub z blokadą).
2. Kalibracja map momentu, regeneracji, limitów.
3. Testy drogowe (stopniowo: niskie prędkości → pełne obciążenie).
4. Pomiary temperatur, zasięgu, hamowania.
5. Poprawki i dokumentacja.

## Faza 6: Homologacja i finalizacja

1. Przygotowanie dokumentacji technicznej.
2. Badania techniczne / ewentualna homologacja indywidualna.
3. Rejestracja zmian.
4. Instrukcja użytkownika i serwisowa.

## Checklist bezpieczeństwa przed jazdą

- [ ] Izolacja HV > 1 MΩ
- [ ] Wszystkie wyłączniki działają
- [ ] Brak wycieków chłodziwa
- [ ] Hamulce sprawne (regen + hydraulika)
- [ ] Oświetlenie i sygnały OK
- [ ] SoC i temperatury w normie
