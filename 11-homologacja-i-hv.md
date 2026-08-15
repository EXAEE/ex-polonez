# 11. Homologacja (PL) + schemat HV high-level

## Ścieżka legalizacji konwersji w Polsce (stan 2026)

1. Dokumentacja techniczna konwersji (opis, schematy, masy, moce, lista komponentów).
2. Opinia rzeczoznawcy (PZM / ITS lub uprawniony) – weryfikacja bezpieczeństwa HV i zgodności.
3. Badanie techniczne w uprawnionej stacji (pojazdy zmodyfikowane).
4. Wpis zmian w dowodzie rejestracyjnym (rodzaj zasilania → energia elektryczna, nowe dane mocy/masy).
5. Ubezpieczenie OC (często wymaga potwierdzenia zmian).

Koszt orientacyjny formalności: 2–6 tys. PLN.  
Czas: zwykle 4–10 tygodni w zależności od obciążenia rzeczoznawców i stacji.

**Uwaga:** Im bardziej modularna i przejrzysta dokumentacja + oznaczenia HV, tym łatwiejsza opinia rzeczoznawcy.

Dla Borewicza (wartość kolekcjonerska) warto dodatkowo udokumentować odwracalność.

## Schemat HV – high-level (Maintainability First)

```
[Gniazdo ładowania Type2/CCS]
         │
         ▼
[On-board Charger] ──► [Bateria modularna – kasety]
                              │
                              ▼
                         [BMS master]
                              │
              ┌───────────────┼───────────────┐
              ▼               ▼               ▼
        [Stycznik główny] [Monitoring izolacji] [DC-DC 12V]
              │
              ▼
        [Inwerter / Kontroler]
              │
              ▼
     [Power Pack: Silnik + Reduktor]
              │
              ▼
           [Wał → Most]

Punkty serwisowe (łatwy dostęp):
- Service Box (BMS + styczniki + bezpieczniki)
- Dock power packu
- Szybkozłącza każdej kasety baterii
- Wyłącznik awaryjny (kabina + zewnętrzny)
```

Wszystkie złącza HV z interlockiem.  
Kolorystyka: pomarańczowy.  
Każde złącze oznaczone numerem zgodnym z dokumentacją.

## Rekomendacja dokumentacyjna

Do każdego auta:
- Pełny schemat HV i LV (PDF)
- Lista momentów dokręcania
- Procedury wymiany kaset i power packu
- Raport z pomiarów izolacji po montażu
- Zdjęcia przed/po kluczowych etapów

To wszystko ma być w repo + kopia w aucie.
