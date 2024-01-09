# **Wykonanie przerwania**

**Dokładna wiedza o wykonaniu przerwania.**

Wykonanie przerwania jest procesem, w którym mikroprocesor przerywa aktualne wykonywanie programu głównego, aby obsłużyć zdarzenie lub żądanie występujące zewnętrznie. Przerwanie może przechodzić od urządzeń wejścia-wyjścia, zegara czasu rzeczywistego, błędów sprzętowych itp.

1. **Wywołanie przerwania**

-   Zdarzenie zewnętrzne lub wewnętrzne (np. od urządzenia) powoduje wygenerowanie sygnału przerwania.
-   Mikroprocesor odbiera ten sygnał i reaguje na niego.

2. **Zapisanie stanu bieżącego**

-   Mikroprocesor automatycznie zapisuje aktualny stan programu głównego, który obejmuje adres powrotu (z którego nastąpiło przerwanie), zawartość rejestrów, liczniki instrukcji itp.
-   Ten stan jest zapisywany na stosie lub w wyznaczonym obszarze pamięci.

3. **Przejście do procedury obsługi przerwania (ISR - Interrupt Service Routine)**

-   Mikroprocesor pobiera adres procedury obsługi przerwania (ISR) ze specjalnej tablicy przerwań (tzw. wektorów przerwań) lub określanego miejsca w pamięci.
-   Program przenosi wykonanie do tego adresu.
-   Wykonuje się kod procedury obsługi przerwania, który jest dedykowany do reakcji na to konkretne przerwanie.
-   W ramach tej procedury mogę być wykonywane operacje obsługi zdarzenia, komunikacja z urządzeniem, zmiany stanu systemu.

4. **Zakończenie procedury obsługi przerwania**

-   Po zakońzczeniu obsługi przerwania, mikroprocesor przywraca zapisany wcześniej stan programu głównego.
-   Odtwarzane są wartości rejestrów, adres powrotu i inne istotne elementy.
-   Mikroprocesor wraca do miejsca, z którego zostało przerwane wykonanie.
-   Kontynuuje się wykonywanie programu głównego do miejsca, w którym zostało przerwane.

Proces wykonania przerwania obejmuje przechwycenie bieżącegos stanu, przejście do procedury obsługi przerwania, wykonanie odpowiedzi działań, a następnie przywrócenie stanu programu głównego i jego kontynuację. To pozwala mikroprocesorowi reagować na zdarzenia zewnętrzne bez blokowania wykonywania programu głównego.
