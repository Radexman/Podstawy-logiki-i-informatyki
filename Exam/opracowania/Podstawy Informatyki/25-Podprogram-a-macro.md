# **Podprogram a macro**

**Podprogram a macro - różnice (zalety oraz wady jednego i drugiego).**

Podprogramy (funkcje) i makra są oba mechanizmami używanymi w programowanu do wielokrotnego użycia kodu, ale różnią sie w kilku aspektachm takich jak składnia, zarządzanie zmiennymi, czas życia i sposób rozszerzania.

## **Podprogramy**

### **Składnia**

Podprogramy mają bardziej formalną składnię, zdefiniowaną w sekcji kodu porgramu. Moa przyjmować argumenty i zwracać wartość.

### **Zmiennośći**

Mają swoje własne przestrzenie nazw dla zmiennych (zasięg zmiennych), co oznacza, że zmienne zdefiniowane w funkcji są lokalne dla tej funkcji.
Funkcje mogą również korzystać ze zmeinnych globalnych, jeśli są zadelkarowane.

### **Rozszerzalność**

Mogą być wywoływane z dowolnego miejsca w programie. Mogą być rozbudowane on nowe funkcje i aktualizowane niezależnie od reszty kodu.

### **Zarządzanie pamięcią**

Funkcje mają swoje własne ramki stosu, co oznacza, że automatycznie zarządzają pamięcią.

## **Makra**

### **Składnie**

Makra to fragmenty kodu, które są zastępowane przez konkretne wyrażenia podaczas kompilacji. Składnia makr jest bardzo elaryczna, ale mniej formalna niż w przypadku funkcji.

### **Zmienność**

Makra nie mają swoich własnych przetrzeni nazw; są zastępowane w miejscu, gdzie są używane, co może prowadzić do konfliktów nazw.

### **Rozszerzalność**

Makra są rozszerzane w trakcie kompilacji, co oznacza, że ich rozwinięcie odbywa się przed wykonaniem programu. Nie mają możliwości tworzenia nowych funkcji w trakcie działania programu.

### **Zarządzaie pamięcią**

Makra same w sobie nie zarządzają pamięcią, ponieważ są tylko zastępowane przez konkretne wyrażenia w trakcie kompilacji.

## **Wady i Zalety**

### **Podprogramy**

**Zalety**

-   Bardziej czytelna i strukturalna składnia.
-   Możliwość przyjmowania argumentów i zwracania wartości, co czyni je bardziej elastycznymi.
-   Zarządzanie pamięcią jest automatyczne.

**Wady**

-   Wywołanie funkcji wiąże się z pewnym narzutem czasowym (przesyłanie argumentów, towrzenie ramki stosu).

### **Makra**

**Zalety**

-   Bardzo elastyczne, umzliwiają zastępownaie dowolnych fragmentów kodu.
-   Mogą być używane do definicji prostych, często używanych fragmentów kodu.

**Zalety**

-   Mniejsza czytelność z powodu bardziej swobodnej składi.
-   Mogą prowadzić do błędów związanych z konfiktami nazw.
-   Brak zarządzania pamięcią, co może prowadzić do nieoczekiwanych efektów ubocznych.

Wybór między podprogramem a makrami zależy od konkretnego przypadku użycia i preferencji programisty. W praktyce często korzysta się z funkcji do bardziej ogólnych zadań, a makra wykorzystuje się do prostych, powtarzalnych fragmentów kodu.
