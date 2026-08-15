# 03. Pakiet akumulatorów

## Cele

- 35–60 kWh usable (w zależności od modelu i budżetu)
- Zasięg realny 180–280 km
- Rozkład masy zbliżony do oryginału lub nieznacznie poprawiony (więcej na tył dla RWD)
- Modularność (możliwość łatwej wymiany / rozbudowy bloków)
- Bezpieczeństwo (ogień, crash, termika)

## Chemia i format

Rekomendacja 2026:
- **NMC lub LFP** – LFP bezpieczniejszy i dłuższa żywotność, NMC wyższa gęstość energetyczna.
- Preferowane: gotowe moduły (Tesla, BYD, CATL, LG) lub custom z ogniw 21700/4680.
- Napięcie nominalne systemu: 320–400 V.

## Lokalizacja pakietów (priorytet)

1. **Komora silnika** – przednie bloki (zastępują silnik + część osprzętu). Niski środek ciężkości, dobre chłodzenie.
2. **Podłoga / tunel centralny** – główna masa baterii (jeśli przestrzeń pozwala po demontażu zbiornika paliwa i wału częściowo).
3. **Bagażnik / przestrzeń ładunkowa** – tylne bloki (szczególnie w Truck i Karetce – pod podłogą skrzyni lub w szafkach).
4. **Pod siedzeniami** – opcjonalne małe bloki.

W Caro Plus / Borewicz: ~40–50% przód, 50–60% tył/podłoga.
W Truck/Karetka: większa swoboda – więcej w ładowni.

## Modularność (innowacja kluczowa)

System bloków 5–10 kWh z własnymi BMS slave + szybkozłączami HV/LV/chłodzenia.
- Możliwość demontażu jednego bloku do serwisu.
- Opcja „range extender” – dodatkowy blok w bagażniku na dłuższe trasy.
- W przyszłości: swap stations (teoretycznie).

## BMS i zarządzanie

- Główny BMS z komunikacją CAN + monitoring izolacji.
- Równoważenie aktywne lub pasywne.
- Integracja z inwerterem i systemem 12 V (DC-DC).
- Telemetria: temperatura, SoC, SoH, prądy – wyświetlane na nowej desce lub app.

## Chłodzenie / ogrzewanie

- Chłodzenie cieczą (preferowane) lub powietrze wymuszone.
- PTC heater lub pompa ciepła do kondycjonowania pakietu w zimie (Polska!).
- Termiczne zarządzanie krytyczne przy LFP i NMC.

## Bezpieczeństwo

- Obudowy metalowe / kompozytowe z wentylacją awaryjną.
- Czujniki dymu / temperatury z automatycznym odcięciem.
- Oznaczenia HV, wyłączniki, procedury serwisowe.
- Testy izolacji przed pierwszym uruchomieniem.

## Szacunkowa masa

- 40 kWh usable ≈ 250–320 kg (w zależności od chemii i obudów)
- 55 kWh ≈ 340–420 kg

Masa musi być skompensowana przez usunięcie ICE + skrzyni + zbiornika + wydechu (~180–250 kg). Netto przyrost masy 100–250 kg – akceptowalny przy wzmocnieniu zawieszenia.

## Ładowanie

- On-board charger 6.6–11 kW (AC Type 2)
- Opcja DC CCS (50–100 kW) – droższa, ale bardzo pożądana
- Gniazdo w miejscu oryginalnego wlewu paliwa lub w zderzaku
