# **Podstawowe pojęcia działania programu**

**Podstawowe pojęcia działania programu na mikroprocesorze (inicjalizacja, program główny, podprogram, macro, przerwanie).**

1. **Inicjalizacja** - To proces uruchamiania mikroprocesora. W trakcie inicjalizacji mikroprocesor przechodzi przez szereg kroków, które mogę obejmować konfigurację pamięci, rejestrów, urządzeń wejścia-wyjścia i innych elementów systemowych. Inicjalizacja zapewnia, że mikroprocesor znajduje się w odpowiednim stanie do wykonywania programów.

2. **Program Główny** - Jest to główna część programu, która wykonuje konkretne zadania. To tutaj znajduje się logika, której celem jest realizacja funkcjonalności, które chcemy osiągnąć. Program główny może zawierać instrukcje warunkowe, pętle, operacje na danych, komunikację z urządzenia itp.

3. **Podprogram** - Podprogram to fragment kodu, który wykonuje określone zadanie i może być wywoływany z różnych miejsc w programie głównym lub innych podprogramach. Podprogramy pomagają w organizacji kodu, poprzez wydzielenie powtarzających się lub logicznie oddzielnych fragmentów. Mogą przyjmować argumenty (parametry) i zwracać wartość.

4. **Makra** - Makrodefinicje są wykorzystywane do zautomatyzowania powtarzających się fragmentów kodu. Definiują one skróty (makra), które są zastępowane przez konkretne fragmenty kodu podczas kompilacji. Mogą być używane do uproszczenia pisania kodu, poprawy czytelności lub uniknięcia duplikacji kodu.

5. **Przerwania** - Przerwanie to mechanizm, króry pozwala mikroprocesorowi na reagowanie na zdarzenia zewnętrzne lub wewnętrzne w sposób asynchroniczny. Gdy przerwanie występuje (np. od urządzenia wejścia-wyjścia), mikroprocesor przerywa bieżące wykonywanie programu, zapamiętuje swój stan, a następnie wykonuje specjalną procedurę obsługi przerwania. Po zakończeniu obsługi przerwania do poprzedniej pracy.

Te elementy są kluczowe podczas tworzenia programów dla mikroprocesorów, umożliwiając organizację kodu, reakcję na zdarzenia oraz zoptymalizowae wykonywanie zadań.
