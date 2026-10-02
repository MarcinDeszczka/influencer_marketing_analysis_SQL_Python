# Analiza efektywności influencer marketingu

**Projekt portfolio — SQL + Python**

## O projekcie

Celem projektu jest analiza efektywności kampanii influencer marketingowych w branży modowej. Analiza koncentruje się m.in. na efektywności influencerów, wynikach kampanii, ROI, przychodach oraz wpływie kategorii produktów na rezultaty kampanii.

Do analizy wykorzystałem syntetyczny zbiór **Influencer Marketing Campaign Analysis** dostępny na Kaggle. Zbiór został zaprojektowany jako realistyczna symulacja danych dotyczących kampanii influencer marketingowych i obejmuje relacje pomiędzy influencerami, kampaniami, produktami, zamówieniami oraz klientami.

[Dataset na Kaggle](https://www.kaggle.com/datasets/divyamehulmak/influencer-marketing-campaign-analysis-power-bi/)

## Zakres danych

Baza obejmuje:

* **20 influencerów** — platforma, tier, liczba obserwujących, zaangażowanie i dane dotyczące audytorium,
* **10 kampanii** — budżet, czas trwania, platforma, kategoria produktu i cel kampanii,
* **25 produktów** — kategorie, podkategorie, ceny, sezonowość i daty premiery,
* **ponad 100 tys. zamówień** — klienci, produkty, influencerzy, kampanie, kody rabatowe i wartości transakcji,
* **ponad 90 tys. klientów** — dane demograficzne, lokalizacja, dochód, preferowany styl oraz Customer Lifetime Value (CLV).

Dane są syntetyczne i służą wyłącznie celom demonstracyjnym. W związku z tym niektóre wyniki finansowe, w szczególności wartości ROI, mogą być nierealistyczne. Nie wpływa to na zastosowaną metodologię analizy. Walutą przyjętą w zbiorze jest USD.

## Przygotowanie danych

Dane wykorzystane w części SQL i Python pochodzą z tego samego źródła, ale zostały przygotowane niezależnie.

**SQL**

Oryginalny plik `.xlsx` został przekonwertowany do `.csv`, a następnie zaimportowany do bazy SQLite `.db` skonfigurowanej w DB Browser for SQLite. Podczas przygotowania danych przeprowadziłem ręczną weryfikację typów danych i poprawiłem wykryte niezgodności.

**Python**

Dane zostały wczytane bezpośrednio z plików `.xlsx`. Dodatkowo za pomocą Pythona skorygowałem separatory dziesiętne, które zostały nieprawidłowo zmienione podczas wcześniejszej konwersji danych do `.csv`.

## Technologie

* **SQL / SQLite**
* **Python**
* **Jupyter Notebook**
* `pandas`
* `numpy`
* `seaborn`
* `matplotlib`
* `plotly`
* `openpyxl`
* `IPython.display`
* `re`

SQL jest wykonywany w notebooku za pomocą `%%sql`.

W trakcie pracy korzystałem również ze wsparcia AI przy rozwiązywaniu problemów technicznych. **Kod SQL został napisany przeze mnie i nie był generowany przez AI.**

## Analiza SQL

### Zadanie 1 — Segmentacja influencerów

Audyt zgodności segmentacji influencerów z danymi znajdującymi się w bazie.

### Zadanie 2 — Agregacja kampanii

Agregacja najważniejszych danych dotyczących kampanii.

### Zadanie 3 — Kompleksowy profil efektywności influencerów

Analiza wyników influencerów z wykorzystaniem wielu wskaźników efektywności.

### Zadanie 4 — Selekcja twórców powyżej średniej

Identyfikacja influencerów osiągających wyniki powyżej wartości średnich.

### Zadanie 5 — Benchmark ROI względem platformy

Porównanie ROI influencerów z benchmarkiem właściwym dla danej platformy.

### Zadanie 6 — Trend przychodu miesiąc do miesiąca

Analiza zmian przychodu w ujęciu Month-over-Month (MoM).

## Analiza Python

### Wczytanie i weryfikacja jakości danych

Import danych oraz podstawowa kontrola ich jakości i struktury.

### Zadanie 7 — Wpływ kategorii produktu na skuteczność kampanii

Analiza zależności pomiędzy kategorią produktu a wynikami kampanii.

### Zadanie 8 — Wizualizacja przepływów przychodu

Wizualizacja przepływu przychodu pomiędzy poszczególnymi elementami analizy za pomocą diagramu Sankeya.

## Struktura projektu

```text
Python_SQL/
│
├── README.md
├── README_PL.md
│
├── influencer_marketing_analysis_EN.ipynb
├── influencer_marketing_analysis_PL.ipynb
│
│
└── ...


## Notebook

Pełna analiza wraz z kodem SQL, Pythonem, wynikami zapytań, wizualizacjami i komentarzami znajduje się w notebooku **Notebook Całość.ipynb**.
