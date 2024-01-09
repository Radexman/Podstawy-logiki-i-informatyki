# **Wykonanie podprogramu**

**Dokładna wiedza o wykonaniu podprogramu**

Wykonanie podprogramu (czyli funkcji w przypadku programowania) to sekwencja kroków, która ma miejsce, gdy dany fragment kodu jest wywoływany z innego fragmentu programu. Oto dokładny proces wykonania podprogramu.

## **Wywołanie podprogramu**

1. **Przygotowanie do wywołania**

-   Zbierane są argumenty lub parametry, jeśli podprogram ich wymaga.
-   Adres powrotu (adres, z którego został wywołany podprogram) jest zapamiętywany.
-   Rejestr instrukcji wskazuje na pierwszą instrukcję podprogramu.

2. **Przejście do podprogramu**

-   Wykonywanie kodu przechodzi do pierwszej instrukcji wewnątrz podprogramu.

3. **Wykonywanie kodu podprogramu**

-   Wykonywane są kolejne instrukcje zawarte w podprogramie.
-   Może następować manipulacja danymi, obliczenia, warukni, pętle itp.

4. **Zakńczenie podprogramu**

-   Jeśli podprogram ma zwrócić wartość, jest ona przygotowywana.
-   Rezultat ten zostaje przechowywany w stosie lub rejestrze.
-   Adres powrotu jest pobierany z pamięci i program wraca do miejsca, z którego został wywołany podprogram.
-   Wykonywanie podprogramu głównego wznawia się od miejsca, w którym zostało przerwane przez wywołanie podprogramu.

5. **Powrót do programu głównego**

-   Stan zmeinnej środowiskowej (m.in licznik instrukcji, rejestry), jest przyzwracany z momentu, w którym podprogram został wywołany.
-   Program główny wznawia swoje wykonywanie od miejsca, które było przerwane przez wywołanie podprogramu.

Proces wykonania podprogramu obejmuje przejście sterowania do podprogramu, jego wykonanie zgodnie z instrukcjami, ewentualne zwrócenie wartości oraz powrót do miejsca wywołania. Ten proces jest kluczowy w organizacji i wykonywaniu logiki programu, umożliwiając inzolowanie funkcjonalności i ich wielokrotne wykorzystanie.
