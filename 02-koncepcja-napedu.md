# 02. Koncepcja napędu elektrycznego

## Cel projektowy

Zachować charakter RWD Poloneza (moment na tylne koła, klasyczne zachowanie), jednocześnie uzyskać:
- znacząco lepsze przyspieszenie (szczególnie 0–60/80 km/h),
- cichą pracę,
- minimalne straty w układzie przeniesienia,
- możliwość regeneracji.

## Rekomendowana architektura (główna)

**Silnik elektryczny + jednostopniowy reduktor → wał napędowy → oryginalny/wzmocniony most tylny.**

### Dlaczego tak?
- Najmniej inwazyjne w stosunku do oryginalnej geometrii.
- Umożliwia zachowanie oryginalnego mostu (po wzmocnieniu łożysk i półosi jeśli potrzeba).
- Łatwiejsze chłodzenie i serwis w komorze silnika / tunelu.
- Możliwość modularnej wymiany silnika.

### Alternatywy
1. **Adapter do oryginalnej skrzyni biegów** + silnik zamiast ICE (zachowanie możliwości zmiany przełożeń). Dobre do „feelingu” klasycznego, ale dodaje straty i złożoność sprzęgła/hydrauliki.
2. **Pełny swap mostu** na nowocześniejszy (np. z independent lub z lepszym przełożeniem) – droższe, ale lepsza dynamika.
3. **Hub motors** na tylnej osi – bardzo zaawansowane, ciężkie, problematyczne z zawieszeniem sztywnym.

## Dobór silnika (rekomendacje 2026)

| Wariant | Moc continuous / peak | Moment | Przykłady / typ | Uwagi |
|---------|-----------------------|--------|------------------|-------|
| Caro Plus / Borewicz (osobowy) | 80–110 kW / 140–180 kW | 250–350 Nm | NetGain HyPer9, Tesla SDU small, custom PM | Wystarczający do 0–100 ~7–9 s |
| Truck | 110–150 kW / 180–220 kW | 350–500 Nm | Większy SDU, dual motor setup lub heavy duty AC | Pod ładunek |
| Karetka | 90–130 kW / 160–200 kW | 300–400 Nm | Jak Caro + zapas | Cicha praca priorytet |

Preferowane: silniki AC induction lub permanent magnet z chłodzeniem cieczą. Napięcie systemowe 300–400 V nominalne (łatwiejsze komponenty niż 800 V w klasyku).

## Reduktor / przełożenie

- Jednostopniowy reduktor 6–9:1 (dobrany do przełożenia mostu ~4.1–4.3).
- Cel: moment na kołach wystarczający do ruszania z pełnym ładunkiem + rozsądne obroty przy 120–140 km/h.
- Możliwość elektronicznej „skrzyni” (mapy momentu) zamiast fizycznych biegów.

## Montaż silnika

- Wykorzystanie punktów mocowania oryginalnego silnika + nowe łapy / adapter.
- Orientacja: wzdłużna, wyjście wału do tyłu.
- Wibracje: elastyczne poduszki + wyciszenie.
- Dostęp serwisowy: zachować możliwość wyjęcia silnika w górę lub do przodu.

## Układ chłodzenia

- Chłodnica cieczy (oryginalna lub nowa) + pompa elektryczna + termostat elektroniczny.
- Oddzielny obieg dla silnika i inwertera (lub wspólny z BMS jeśli możliwe).

## Hamowanie regeneracyjne

- Mocna regeneracja (do 50–70% energii hamowania w idealnych warunkach).
- Integracja z oryginalnym układem hydraulicznym (blend: regen + tarcze).
- Opcjonalnie pedalbox z programowalnym mapowaniem.

## Bezpieczeństwo HV

- Główny stycznik + wyłącznik awaryjny (pomarańczowy, dostępny z zewnątrz i z kabiny).
- Izolacja przewodów HV (pomarańczowe).
- Monitoring izolacji (BMS).
- Crash sensor odcinający zasilanie.

## Podsumowanie rekomendacji

Dla większości egzemplarzy: **silnik + reduktor w komorze silnika + oryginalny most (po przeglądzie i ewentualnym wzmocnieniu)**. To kompromis między autentycznością, kosztami a osiągami.
