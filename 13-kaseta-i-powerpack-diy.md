# 13. Kaseta baterii + Power Pack – kierunek DIY / circular

## 1. Kaseta baterii (design principles)

### Cel
Jeden blok 5–10 kWh (zależnie od użytych modułów), możliwy do wyjęcia przez jedną osobę po odłączeniu trzech złączy (HV, cooling, data).

### Struktura
- **Rama nośna**: spawana z kątownika stalowego 30×30 lub 40×40 mm (lub aluminiowego jeśli masa krytyczna). Źródło: złom, resztki budowlane, stare regały.
- **Dno**: blacha 2–3 mm lub kratownica + blacha. Można użyć recyklingowanej blachy.
- **Prowadnice i dystanse wewnętrzne**: druk 3D (PETG / ABS / nylon). Konstrukcja tak, żeby moduły wchodziły z lekkim oporem i były unieruchomione w trzech osiach.
- **Pokrywa górna**: blacha lub gruba płyta + uszczelka, ewentualnie drukowana w segmentach.
- **Izolacja**: warstwa NOMEX / G10 / grubej taśmy + dystanse powietrzne. Drukowane elementy nie mogą być jedyną barierą izolacyjną.
- **Uchwyty**: spawane lub skręcane + drukowane nakładki ergonomiczne.

### Złącza
- HV: solidne, z interlockiem (kupione – tu nie oszczędzamy).
- Cooling: szybkozłącza cieczy (standardowe przemysłowe lub z donor EV).
- Data/BMS: standardowe złącze (np. XT60/90 + sygnałowe lub oryginalne z modułu).

### Warianty modułów (priorytet upcyclingu)
- Tesla Model S / X modules (łatwe do znalezienia, dobra gęstość).
- Nissan Leaf modules (tańsze, prostsze napięciowo w niektórych generacjach).
- Inne dostępne tanio na rynku wtórnym.

Każda kaseta powinna mieć ten sam interfejs mechaniczny i elektryczny – wymienność.

---

## 2. Power Pack (silnik + reduktor)

### Rekomendowany silnik na start (koszt + dostępność 2026 PL)
**Nissan Leaf EM57** (używany)
- Ceny rynkowe: często 1 400 – 4 500 PLN
- Wystarczający moment i moc do Caro Plus / Borewicz (przy dobrym przełożeniu)
- Dużo dokumentacji społeczności DIY
- Łatwiej znaleźć niż dobry Tesla SDU w rozsądnej cenie

Alternatywy:
- Inne jednostki z Leaf / e-NV200
- Tesla SDU (jeśli uda się tanio)
- Silnik przemysłowy + własny reduktor (więcej pracy)

### Rama / adapter
- Spawana konstrukcja z kątownika / profilu prostokątnego dopasowana do:
  - punktów mocowania silnika Leaf (lub innego)
  - oryginalnych łap silnika Poloneza lub nowych punktów na podłużnicach
- 3D printed: dystanse, osłony, uchwyty złączy, jigs do precyzyjnego spawania i wiercenia.

### Reduktor
- Najprościej: zachować oryginalną skrzynię Poloneza jako reduktor (adapter silnik → sprzęgło/wał skrzyni) – maksymalny reuse.
- Albo prosty jednostopniowy reduktor spawany / z używanych elementów przemysłowych.

### Dock
Jedno miejsce podłączenia:
- HV power
- Cooling in/out
- Sygnały / enkoder / temperatura
Mechaniczne prowadzenie (kołki + 3D printed tuleje) + solidne śruby.

---

## Następne konkrety do rozwinięcia

1. Wymiary przykładowej kasety pod konkretny moduł (Tesla lub Leaf) + pliki STL koncepcyjne prowadnic.
2. Szkic ramy power packu pod EM57 + punkty mocowania Poloneza.
3. Lista dokładnych źródeł części (Allegro / Otomoto / złomy / grupy DIY).
4. Szacunek masy i środka ciężkości przy kasetowym układzie.

To jest kierunek, w którym idziemy: metal tam gdzie siła i bezpieczeństwo, druk i upcycling wszędzie indziej.
