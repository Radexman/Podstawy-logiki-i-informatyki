# **Tryby pracy procesorów**

**Tryby pracy procesorów (np. tryb superwizora i użytkownika).**

Tryby pracy procesorów to różne poziomy uprawnień, jakie mogą mieć programy działające na komputrze. Są to mechanizmy zaprojektowane w celu ochrony systemu operacyjnego i innych programów przez nieautoryzowanymi lub potencjalnie niebezpiecznymi operacjami.

Istnieją główne tryby pracy procesora:

## **Tryb użytkownika (ang. _user mode_)**

-   Programy działające w tym trybie mają ograniczony dostęp do zasobów sprzętowych i innych funkcji systemowych.

-   Nie mogą wykonywać bezpośrednich operacji na wielu elementach sprzętowych, takich jak rejestry procesora czy pamięć systemowa.

-   Dostęp do systemowych zasobów odbywa się za pośrednictwem wywołań systemowych (system calls), które są kontrolowane przez system operacyjny.

## **Tryb superwizora (ang. _supervisor mode_, _kernel mode_)**

-   Programy działające w tym trybie mają pełen dostęp do zasobów sprzętowych i mogą wykonywać wszystkie instrukcje procesora.

-   Mają także możliwość zarządzania pamięcią, obsługiwania przerwań i wyjątków oraz kontrolowania innych funkcji sprzętowych.

-   System operacyjny działa głównie w trybie superwizora.
