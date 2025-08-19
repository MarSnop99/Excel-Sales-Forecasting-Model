#  Zaawansowany Model Prognostyczny w Excelu: Porównanie Metod Top-Down vs. Bottom-Up

## Cel Projektu
Celem tego projektu było przeprowadzenie kompleksowej analizy porównawczej dwóch popularnych metod prognozowania szeregów czasowych – zagregowanej (Top-Down) i hierarchicznej (Bottom-Up) – w celu znalezienia najdokładniejszego i najefektywniejszego modelu dla danych sprzedażowych firmy "Superstore".

##  Użyte Narzędzia i Metodologia
*   **Narzędzia:** Microsoft Excel, Power Query, Dodatek Solver
*   **Model Statystyczny:** Potrójne Wygładzanie Wykładnicze (Metoda Holta-Wintersa)
*   **Optymalizacja:** Minimalizacja błędu MAPE przy użyciu algorytmu GRG Nieliniowy w dodatku Solver dla każdego z czterech zbudowanych modeli (trzy dla kategorii, jeden zagregowany).
*   **Metodologia Porównawcza:** Skrupulatne zbudowanie i optymalizacja obu modeli, a następnie porównanie ich ostatecznej precyzji na tym samym, oczyszczonym okresie testowym.

## 💡 Kluczowe Odkrycie i Rekomendacja Biznesowa
Wbrew początkowej hipotezie, że bardziej złożony, hierarchiczny model Bottom-Up okaże się dokładniejszy, dogłębna analiza wykazała, że **oba podejścia, po precyzyjnej optymalizacji, zbiegły się do identycznego, najwyższego możliwego poziomu dokładności, osiągając błąd MAPE na poziomie 43%**.

**Rekomendacja Biznesowa:** W związku z faktem, że bardziej złożony i zasobożerny model Bottom-Up nie oferuje żadnej przewagi w precyzji nad prostszym modelem Top-Down, **rekomendacja biznesowa jest jednoznaczna: należy wdrożyć model Top-Down.** Pozwoli to osiągnąć ten sam, optymalny rezultat przy znacznie niższym nakładzie czasu i zasobów na jego budowę, utrzymanie i ewentualne modyfikacje. Odkrycie to podkreśla, że celem analizy jest znalezienie najefektywniejszej drogi do najlepszego wyniku.

##  Przegląd Pliku
Plik `Superstore Analysis.xlsx` w tym repozytorium zawiera kompletny, interaktywny model z następującymi arkuszami:
*   **README:** Strona startowa z nawigacją i opisem projektu.
*   **Conclusion & Comparison:** Główny arkusz wynikowy z finalnym porównaniem obu metod, wnioskami i wizualizacjami.
*   **Forecast_TopDown & Forecast_[Kategorie]:** Cztery arkusze zawierające w pełni działające, zoptymalizowane modele prognostyczne.
*   **Aggregated_Data:** Czyste dane źródłowe przygotowane za pomocą Power Query.

*Możesz pobrać plik, aby samodzielnie przetestować działanie modelu i Solvera.*
