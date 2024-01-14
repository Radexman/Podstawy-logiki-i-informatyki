# **Algebra Boole'a**

**Algebra Boole'a (ze szczególnym uwzględnieniem prawa sklejania i pochłaniania).**

Algebra Boole'a to amtematycza dziedzina, która obejmuje manipulacje logiczne przy użyciu zbioru opercaji i regół logicznych opracowanych przez Georga Boole'a. Jest szeroko stosowana w dziedzinie informatyki, elektroniki cyfrowej, systemów sterowania i innych obszarach, gdzie logika odgrywa kluczową rolę.

## **Operacje w algebrze Boole'a**

1. **Negacja NOT**

-   Oznaczana jako !A.
-   Neguje wartość logiczną, czyli zamienia prawdę na fałsz i odwrotne.

2. **Koniunkcja AND**

-   Oznaczana jako A \* B lub A v B.
-   Zwraca prawdę tylko wtedy, gdy obie wartości logiczne są prawdziwe.

3. **Alternatywa OR**

-   Oznacza jako A \* B lub A ^ B.
-   Zwraca prawdę, gdy co najmniej jedna z watrości logicznych jest prawdziwa.

## **Prawo Sklejania (Associate Law)**

Prawo sklejania mówi o tym, że przy wykonywaniu opeacji AND lub OR, kolejność, w jakiej są grupowane wyrażenia, nie ma zanczenia

**Dla operacji AND**
(A _ B) _ C = A _ (B _ C)

**Dla operacji OR**
(A + B) + C = A + (B + C)

Prawo sklejania pozwala na uproszczenie wyrażeń logicznych i ułatwia ich analizę.

## **Prawo Pochłaniania (Absorption Law)**

Prawo Pochłaniania mówi o tym, że można "pochłonąć" jedno z wyrażeń w przypadku, gdy jedno z wyrażeń jest AND-em (koniunkcja) z drugim, a drugie jest zawarte w pierwszym w sensie logicznym.

**Dla operacji AND**
A \* (A + B) = A

**Dla operacji OR**
A + (A \* B ) = A

Prawo Pochłaniania pozwala na uproszczenie wyrażeń logicznych poprzez eliminajcę niepotrzebnych składników.

Te prawa są fundamentem algebry Boole'a i są szeroko wykorzystywane w projektowaniu układów czyfrowych, programowaniu logicznymi i analizie logicznej. Pomagają one w uproszczeniu i analizie złożonych wyrażeń logicznych.
