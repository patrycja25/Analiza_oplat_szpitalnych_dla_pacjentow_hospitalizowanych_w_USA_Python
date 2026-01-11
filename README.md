# Analiza_oplat_szpitalnych_dla_pacjentow_hospitalizowanych_w_USA_Python

## Projekt wykonany we współpracy z Emmą Panasiuk (https://github.com/emmapstudent)

## Skrypt w języku Python bada relacje między opłatami szpitalnymi, kwotami pokrywanymi przez Medicare a rzeczywistymi płatnościami w USA, w celu identyfikacji potencjalnych anomalii cenowych oraz struktury kosztów leczenia.
Zachęcam do zapoznania się z prezentacją w repozytorium.

# Źródło danych
https://www.kaggle.com/datasets/speedoheck/inpatient-hospital-charges/data 

# Wymagane biblioteki:
pandas (wczytywanie, czyszczenie i manipulacja danymi)

numpy (obliczenia numeryczne)

matplotlib (tworzenie wykresów i wizualizacja danych)

re (wyrażenia regularne do przetwarzania tekstów)

# Kluczowe zmienne:

DRG Definition (Definicja grupy diagnostycznej/choroby)

Provider State (Stan, w którym znajduje się dostawca usług)

Total Discharges (Liczba wypisów)

Average Covered Charges (Średnia kwota obciążenia wystawiona przez szpital)

Average Total Payments (Średnia kwota faktycznie zapłacona)

Average Medicare Payments (Średnia kwota pokryta przez Medicare)

# Analiza danych:

W procesie przygotowania danych do analizy wykonano następujące kroki:

### Czyszczenie danych: 

Usunięto znaki walutowe ($) z kolumn finansowych i przekonwertowano je na typy numeryczne (float), aby umożliwić operacje matematyczne.

### Utworzono nowe zmienne w celu zbadania struktury płatności:

Medicare Payments as Percentage: Procent kosztów pokrywanych przez Medicare.

Actual Payments as Percentage: Stosunek faktycznej zapłaty do kwoty zadeklarowanej przez szpital (wskaźnik potencjalnego "zawyżania" cen).

# Zwerfyfikowano następujące hipotezy badawcze:
- Czy dostawcy usług medycznych w USA dopuszczają się oszustw w wycenie usług medycznych? ​

- Z tytułu czego pacjenci są najczęściej przyjmowani? I ile jest tego typu osób?​

- Jakie są średnie koszty pokryte przez Medicare a przez pacjenta? ​
