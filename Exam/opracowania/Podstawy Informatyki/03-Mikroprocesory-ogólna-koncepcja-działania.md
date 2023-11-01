# **Mikroprocesory - ogólna koncepcja działania**

**Mikroprocesory (jedno i wielordzeniowe) - ogólna koncepcja działania - sposób wykonywania kodu**

## **Budowa typowego mikroprocesora**

W prawie każdym mikroprocesorze możemy wyróżnić następujące bloki:

-   ALU - jednostka arytmetyczno-logiczna (ang. _Arithmetic Logic Unit_), wykonuje ona operacje logiczne na dostarczonych jej danych, podstawowy zestaw to: dodawanie, podstawowe operacje logiczne (AND, XOR, OR, NOT), oraz przesunięcia bitowe w lewo i prawo. W bardziej złożonych mikroprocesorach zestaw ten jest znacznie bogatszy,

-   CU - układ sterowania (ang. _Control Unit_), zwany również dekoderem rozkazów. Odpowiedzialny jest on za dekodowanie dostarczonych mikroprocesorowi instrukcji i odpowiednie sterowanie pozostałymi jego blokami (na przykład jeśli zdekodowaną instrukcją będzie dodawanie, CU odpowiednio ustawi sygnały sterujące, by ALU wykonała tę właśnie operację),

-   Rejestry - umieszczone wewnątrz mikroprocesora komórki pamięci o niewielkich rozmiarach (najczęściej 4/8/16/32/64/128 bitów) służące do przechowywania tymczasowych wyników obliczeń (rejestry danych) oraz adresów lokacji w pamięci operacyjnej (rejestry adresowe). Proste mikroprocesory mają tylko jeden rejestr danych zwany akumulatorem. Oprócz rejestrów danych i rejestrów adresowych występuje też pewna liczba rejestrów o specjalnym przeznaczeniu:

    -   PC - licznik rozkazów (ang. _Program Counter_) - zawiera on adres komórki pamięci zawierającej następny rozkaz do wykonania,
    -   IR - rejestr instrukcji (ang. _Instruction Register_) - zawiera on kod aktualnie wykonywanej przez procesor instrukcji,
    -   SP - wskaźnik stosu (ang. _Stack Pointer_) - zawiera adres wierzchołka stosu,

Mikroprocesor komunikuje się z otoczeniem za pomocą szyny danych i szyny adresowej.

## **Sposób Działania**

1. **Pobieranie instrukcji** - mikroprocesor odczytuje kolejne instrukcje z pamięci operacyjnej RAM lub z pamięci cache.

2. **Dekodowanie instrukcji** - mikroprocesor rozumie instrukcje, które odczytał, interpretując je na poziomie elektronicznym.

3. **Wtkonywanie operacji** - mikroprocesor wykonuje operacje zgodnie z zrozumiałymi instrukcjami. Operacje mogą objemować dodawanie, odejmowanie, mnożenie, dzielenie, porównywanie itp.

4. **Zarządzanie danymi** - mikroprocesor przechowuje dane w rejestrach (małe, szybkie obszary pamięci wewnętrznej). Operacje są wykonywane na danych przechowywanych w tych rejestracj.

5. **Kontrola przepływu programu** - mikroprocesor decyduje, który zestaw instrukcjii ma zostać wykonany na podstawie wyników poprzednich operacji lub innych warunków logicznych.

6. **Obsługa przerwań** - mikroprocesor może przerwać aktualnie wykonywany program, aby obsłużyć priorytetowe zadania lub zdarzenia, takie jak wejście/wyjście lub inne sytuacje awaryjne.

7. **Komunikacja z pamięcią** - mikroprocesor może odczytywać i zapisywać dane w pamięci, aby przetwarzać je lub przechowywać wyniki obliczeń.

8. **Komunikacja z urządzeniami wejścia/wyjścia (I/O)** - mikroprocesor może komunikować się z różnymi urządzeniami, takimi jak klawiatura, monitor, dyski twarde itp. za pomocą portów I/O.

9. **Wykonywanie skoków (branching)** - mikroprocesor może zmieniać bieg programu, wykonując instrukcje skoku (np. warunkowe skoki, pętle, itp.) w zależności od wyników operacji.

10. **Cykl zegara** - mikroprocesor operuje w cyklach zegara, gdzie każdy cykl reprezentuje jedną jednostkę czasu, w której wykonywane są konkretne operacje.

11. **Reagowanie na sygnały sterujące** - mikroprocesor reaguje na sygnały sterujące pochodzące z układów zewnętrznych, takich jak kontrolery pamięci, karty graficzne, itp.

12. **Obsługa błędów i wyjątków** - mikroprocesor może wykrywać błędy i obsługiwać wyjątkowe sytuacje, takie jak dzielenie przez zero, odwołania do niepoprawnej pamięci itp.

Ogólnie rzecz biorąc, mikroprocesor jest mózgiem komputera, który przetwarza dane i instrukcje w sposób sekwencyjny, umożliwiający wykonywanie różnych zadań i programów. Jego działanie jest wspomagane przez inne komponenty komputera, takie jak pamięć, karty rozszerzeń, kontrolery itp.

## **Dodatkowe Informacje**

**Klasyfikacja Mikroprocesorów**

Generalnie każdy bardziej skomplikowany mikroprocesor można zaklasyfikować do jednej z trzech architektur:

-   CISC (ang. _Complex Instruction Set Computing_)
-   RISC (ang. _Reduced Instruction Set Computing_)
-   VLIW (ang. _Very Long Instruction Word_)

---

-   Mikroprocesory i Mikrokontrolery - https://www.youtube.com/watch?v=Wiv4k4ku-Qc&t=386s
