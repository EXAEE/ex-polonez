# 15. Power Pack pod Nissan Leaf EM57 – DIY low-cost

## Dlaczego EM57

- Cena używanego na rynku PL: często 1,4–4,5 tys. PLN
- Moment ~250–340 Nm (w zależności od generacji/inwertera)
- Dużo wiedzy społeczności DIY
- Względnie kompaktowy
- Chłodzony cieczą (ale można na początek rozważyć uproszczenia)

## Szkic ramy / adaptera

**Cel:** jeden blok, który da się wyjąć po odłączeniu docka.

**Konstrukcja:**
- Płyta główna lub rama z kątownika / profilu prostokątnego (stal ze złomu).
- Punkty mocowania do silnika EM57: wykorzystać istniejące gwintowane otwory w obudowie silnika (są gotowe zestawy płytek montażowych na rynku, ale można je odtworzyć samemu z blachy 6 mm).
- Punkty mocowania do nadwozia Poloneza: oryginalne łapy silnika + ewentualne dodatkowe wsporniki do podłużnic.
- Wysokość i pozycja wału tak dobrana, żeby możliwie prosto połączyć z oryginalną skrzynią lub mostem.

**3D print:**
- Dystanse precyzyjne
- Osłony
- Uchwyty złączy
- Jigs do wiercenia i spawania (duża oszczędność czasu i błędów)

## Redukcja kosztów / budowa od zera

1. **Maksymalny reuse skrzyni biegów Poloneza**  
   Silnik EM57 → adapter → sprzęgło / wał skrzyni. Skrzynia zostaje jako reduktor wielostopniowy. To jeden z najtańszych sposobów na sensowne przełożenie.

2. **Płyta montażowa silnika**  
   Zamiast kupować gotową – wyciąć z blachy 5–6 mm (laser lub nawet ręcznie + szlifierka) na podstawie szablonu 3D printed lub papierowego.

3. **Chłodzenie**  
   Na pierwszą wersję: uproszczone cieczowe z pompą z złomu / PC + chłodnica z auta, albo testowo powietrze jeśli silnik na to pozwoli przy ograniczonym obciążeniu.

4. **Inwerter**  
   Używać oryginalnego z Leafa + open-source kontroler (OpenInverter, rozwiązania społeczności) zamiast drogich uniwersalnych jednostek.

5. **Cały power pack jako „skrzynia”**  
   Można zamknąć silnik + inwerter w prostej spawanej skrzyni z blachy – łatwiejszy transport i ochrona.

---

Dokładne wymiary otworów EM57 trzeba potwierdzić na konkretnym egzemplarzu (lub z gotowych płytek montażowych jako wzorca).  
Najpierw warto kupić silnik, zmierzyć, dopiero potem finalizować ramę.
