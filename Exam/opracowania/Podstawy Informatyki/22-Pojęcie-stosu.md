# **Pojęcie Stosu**

**Pojęcie stosu, przykłady zastosowań**

Stos jest to struktura danych w informatyce, która działa na zasadzie LIFO (Last In First Out), czyli ostatni element dodany jest pierwszym do wyjęcia. Jest to podstawowa struktura używana w programowaniu do przechowywania danych i zarządzania wywoływanymi funkcji w pamięci komutera.

## **Jak działa Stos?**

Stos operuje na dwóch głównych oepracjach:

-   **Push** - Dodaje nowy element na wierzch stosu.
-   **Pop** - Usuwa element znajdujący się na wierzchu stosu.

Elementy na stosie są umieszczone jeden na drugim, a operacja push dodaje nowy element na górę stosu, przesuwając wcześniejsze elemety w dół. Operacja pop usuwa element z wierzchu stosu, pozwalając na dostęp do poprzednio umieszczonych danych.

## **Zastosowanie losu**

1. **Wywołania funkcji (Call Stack)** - Gdy funkcja jest wywoływna, informacje o jej stanie (takie jest lokalne zmienne, adres powrotu) są umieszczane na stosie. Gdy funkcja się kończy (return), jee stan jest usuwany ze stosu, a program wraca do miejsca, z którego funkcja została wywołana.

2. **Algorytmyy rekurencyjen** - Rekurencyjne funkcje wywołują same siebie. Stos jest wykorzystywany do przechowywania stanów wywołań rekurencyjnych, a pop przy zakończeniu wywołania usuwa te stany.

3. **Wyrażenia postfix (odwrotna notacja polska)** - W tej notacji operacje umieszczane są po operandach. Obliczenia są wykonywane z użyciem stosu, który przechowuje operandy i wykonywane są na nich odpowiednie operacje.

4. **Algorytmy przeszukiwania (np. DFS - Depth-First Search)** - Stos może być wykorzystywany w algorytmach przeszukiwania grafów (takich jak DFS), aby przechowywać wierzchołki do odwiedzenia lub do cofania się do poprzednich wierzchłków w grafie.

Stos jest wszechstronną strukturą danych używają w programowaniu do przechowywania danych w organizacji LIFO. Jego elastyczniość sprawia, że jedt używany w różnych kontekstach do zarządzania funkcjami, poprzez algorytmy rekurencyjne, po przeszukiwanie grafów.
