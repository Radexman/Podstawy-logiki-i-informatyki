## **Priorytety systemu przerwań**

**Priorytety systemu przerwań oraz ustawianie ich aktywności (blokowanie/odblokowanie. Przykładowo, czy po RESET mikroprocesora przerwania są zablokowane?)**

W systemach przerwań istnieje koncepcja priorytetów, które oklreślają, które przerwania maja pierwszeństwo obsługi w stosunku do innych w przypadku, gdy więcej niż jedno przerwanie wystąpiło jednoczeńsnie. Wyższy priorytet oznacza, że przerwanie zostanie obsłużone przed przerwaniami o niższym priorytecie.

## **Ustawianie aktywności przerwań**

1. **Blokowanie przerwań** - Blokowanie przerwań to mechanizm, który uniemożliwia lub zatrzymuje obsługę przerwań o niższym priorytecie niż obecnie wykonywanie. Jest to przydatne w sytuacjach, gdy chcemy uniknąć zakłóceń wrażliwych operacji (np. krytycznych sekcji kodu).

2. **Odblokowywanie przerwań** - Odblokowywanie przerwań to aktywacja obsługi pzerwań po ich wsześniejszym zablokowaniu. Pozwala to na ponowne uwzględnienie przerwań w systemie i kontynuowanie ich obsługi.

## **Po RESET mikroprocesora**

Po zresetowaniu mikroprocesora przerwania mogą mieć różne ustawienia. W niektórych architekturach mikroprocesorów przerwania mogą być domyślnie wyłączone (zablokowanie), podczas gdy w innych mogą być domyślnie włączone (odblokowane).

Jednakże, po resecie, konkretny stan przerwań (czy są zablokowane lub odblokowane) zależy od implementacji mikropeocesora oraz konfiguracji systemu. Często producenci mikroprocesorów ustawiają konktetne domyślne zachowanie przerwań w swoich dokumentacjach technicznych.

Ważne jest, aby zrozumieć to zachowanie, ponieważ zarządzenie przerwaniami po resecie może mieć istotne znaczenie w programowaniu mikrokontrolerów lub systemów wbudowanych.
