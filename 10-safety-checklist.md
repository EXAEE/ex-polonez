# 10. Safety & Service Checklist

## Przed pierwszym uruchomieniem (krytyczne)

- [ ] Izolacja HV zmierzona (min. 1 MΩ, lepiej >5 MΩ) – wszystkie obwody
- [ ] Interlocki na wszystkich złączach HV działają (otwarcie = odcięcie)
- [ ] Główny wyłącznik awaryjny (pomarańczowy) odcina zasilanie w <1 s
- [ ] Crash sensor / bezwładnościowy odcinacz przetestowany
- [ ] Brak uszkodzeń mechanicznych izolacji przewodów
- [ ] Wszystkie złącza HV zablokowane i oznaczone
- [ ] Chłodzenie szczelne, odpowietrzone, poziom OK
- [ ] BMS komunikuje się, SoC i temperatury realistyczne
- [ ] Hamulce hydrauliczne sprawne niezależnie od regeneracji
- [ ] Światła, sygnały, wycieraczki, wspomaganie działają na 12 V

## Checklist po każdej poważniejszej interwencji

- [ ] Test izolacji ponownie
- [ ] Momenty dokręcenia kluczowych śrub (z dokumentacji)
- [ ] Brak luźnych przewodów w strefie ruchomej
- [ ] Funkcja regeneracji i blend hamowania sprawdzona na podnośniku

## Procedury serwisowe (high-level)

### Wymiana kasety baterii
1. Wyłączenie główne + potwierdzenie braku napięcia
2. Odłączenie cooling → data → HV (kolejność!)
3. Odblokowanie prowadnic / śrub
4. Wyjęcie kasety (uchwyty)
5. Montaż odwrotny + test izolacji + komunikacja BMS

### Wymiana power packu (silnik+reduktor)
1. Odłączenie docka (HV + cooling + sygnały)
2. Odkręcenie 4–6 śrub mocujących
3. Wyjęcie całego bloku
4. Montaż nowego + kalibracja map (jeśli wymagana)

### Kontrola mostu / łożysk
Dostęp od spodu lub przez klapy – bez ruszania baterii.

## Oznaczenia obowiązkowe w aucie

- Pomarańczowe przewody HV
- Naklejki ostrzegawcze przy wszystkich punktach dostępu do HV
- Schemat awaryjny w bagażniku / schowku
- QR do pełnej dokumentacji serwisowej
