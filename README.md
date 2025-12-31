#  Zaawansowane Prognozowanie Popytu (Excel + Solver)

### [Pobierz Model Excel (.xlsx)](Superstore Analysis.xlsx)

Projekt analityczny porównujący skuteczność dwóch strategii prognozowania sprzedaży: **Top-Down** (ogół do szczegółu) vs **Bottom-Up** (szczegół do ogółu).
Celem było wyłonienie metody optymalnej kosztowo i jakościowo dla sieci handlowej "Superstore".


##  Problem Biznesowy
Firma potrzebowała wiarygodnej prognozy sprzedaży, aby zoptymalizować stany magazynowe.
Pytanie badawcze: *Czy warto inwestować czas w budowę skomplikowanych modeli dla każdej kategorii osobno (Bottom-Up), czy wystarczy jeden model zagregowany (Top-Down)?*

##  Metodologia i Narzędzia
*   **Silnik:** Excel (Holt-Winters Triple Exponential Smoothing).
*   **ETL:** Power Query (czyszczenie i agregacja surowych danych transakcyjnych).
*   **Optymalizacja:** **Excel Solver (GRG Nonlinear)** – automatyczne dobieranie parametrów Alfa, Beta, Gamma w celu minimalizacji błędu.
*   **Metryka sukcesu:** MAPE (Mean Absolute Percentage Error).

##  Kluczowe Wnioski (Business Insights)
1.  **Efektywność Kosztowa:** Analiza wykazała, że złożony model Bottom-Up (sumujący prognozy z 3 kategorii) **nie przyniósł przewagi w dokładności** nad prostszym modelem Top-Down (błąd MAPE dla obu wyniósł ok. 43%).
2.  **Rekomendacja:** Zalecane wdrożenie metody **Top-Down**. Pozwala ona osiągnąć ten sam wynik przy **3-krotnie niższym nakładzie pracy** analityka i mniejszym ryzyku błędu operacyjnego.
3.  **Wnioski dla IT:** Mniejsza złożoność modelu oznacza łatwiejsze utrzymanie i szybsze przeliczanie raportów.

##  Struktura Pliku
*   `Conclusion & Comparison` - Dashboard menedżerski z porównaniem metod.
*   `Forecast_TopDown` - Główny model zagregowany (zoptymalizowany Solverem).
*   `Aggregated_Data` - Dane po procesie ETL w Power Query.
