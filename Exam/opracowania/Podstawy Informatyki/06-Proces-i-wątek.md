# **Proces i Wątek**

**Pojęcia: proces, wątek (wskazać na różnice).**

Proces i wątek są dwoma podstawowymi koncepcjami w systemach operacyjnych, które dotyczą sposobu, w jaki programy są wykonywane na komputerze.

## **Proces**

To jedno z najbardziej podstawowych pojęć w informatyce. Z definicji jest to po prostu egzemplarz wykonywanego programu. Należy odróżnić jednak proces od wątku - każdy proces posiada własną przestrzeń adresową, natomias wątki posiadają wspólną sekcję danych.

### **Chrakterystyka Procesu**

-   **Definicja** - proces jest instnacją programu, która jest uruchamiana na komputrze. Obejmuje ona kod programu, dane otwarte pliki i inne zasoby systemowe.

-   **Izolacja** - każdy proces ma swoją właną przestrzeń adresową, co oznacza, że nie możę bezpośrednio ingerować od siebie nazwajem, co zapobiega przypadkowym lub nieautoryzowanym interfejsom.

-   **Synchronizacja** - procesy komunikują się ze sobą lub z systemem operacyjmy za pomocą mechanizmów komunikacji, takich jak potoki, pliki, gniazda lub sygnały.

-   **Zarządzanie Zasobami** - procesy mogą wymagać zasobów systemowych, takich jak pamięć, czas procesora, pliki, urządzenia itp. System operacyjny zarządza dostępem do tych zasobów i przydziela je procesom w sposób sprawiedliwy i efektywny.

-   **Tworzenie i Zakończenie** - procesy mogą być tworzone i zakończone dynamicznie przez system operacyjny w odpowiedzi na akcje użytkownika lub wydarzenia w systemie.

## **Wątek (ang. _tread_)**

To jednostka wykonawcza w obrębie jednego procesu, będąca kolejnym ciągiem instrukcji wykonywanych w obrębie tych samych danych (w tej samej przestrzeni adresowej). Wątki tego samego procesu korzystają ze wspólnego kodu i danych, mają jednak oddzielne stosy.

### **Charakterystyka Wątku**

-   **Definicja** - wątek jest lżejszą jednostką wykonawczą, która działa w obrębie procesu. Oznacza to, że w obrębie jednego procesu można mieć wiele wątków, które dzielą tę samą przestrzeń adresową i zasoby procesu.

-   **Dzielenie przestrzeni adresowej** - wszystkie wątki w jednym procesie współdzielą ten sam obszar pamięci. Oznacza to, że wątki mogą bezpośrednio współpracować i komunikować się ze sobą przez udostępnioną pamięć.

-   **Synchronizacja i współdzielenie zasobów** - wątki w ramach tego samego procesu mogą bezpośrednio współdzielić dane i inne zasoby. Jednak równoczesny dostęp do tych zasobów musi być starannie synchronizowanym aby uniknąć konfliktów i zakleszczeń.

-   **Wykonanie współbieżne** - wątki w ramach tego samego procesu mogą być uruchamiane równolegle na wielu rdzeniach procesu, co pozwala na wydajniejsze wykorzystanie zasobów.

-   **Zakończenie** - zakończenie wątku nie powoduje zakończenia całego procesu, chyba że jest to ostatni wątek w procesie. Inne wątki w procesie mogą nadal działać.

-   **Kontekst wątku** - każdy wątek ma swój własny kontekst wykonawczy, obejmujący stan rejestru, stosu itp. Wątki współdzielną zasoby procesu, ale mają własne sterty i rejestry.

-   **Korzyści** - umożliwiają łatwe wykorzystanie wielu rdzeni procesora, co może znacznie przyspieszyć wykonanie programów, które mają wiele zadań wykonyanych jednocześnie.

Podsumowująć, procesy i wątki to dwie różne jednostki wykonawcze, które pozwalają programom działać na komputerze. Proces to kontener, który obejmuje kod programu, dane i zasoby, podczas gdy wątek to lżejsza jednostka wykonawcza, która działa w obrębie procesu i współdzieli z nimi zasoby. Wątki pozwalają na efektywne wykorzystanie wielu rdzeni procesora i wykonywanie wielu zadań równolegle.

## **Dodatkowe informacje**

W systemach wieloprocesowych, a także w systemach z wywłaszczeniem, wątki mogą być wykonywane równocześnie (współbieżnie). Równoczesny dostęp do wspólnych danych grozi utratą spójności danych, i w konsekwencji błędnem działania programu.
