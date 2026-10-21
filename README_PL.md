# Better Me — wersja prywatna

## Co zawiera
- Dzisiaj: wynik dnia, lista zadań, szybki zapis kroków i masy ciała.
- Nawyki: edytowalna lista codziennych zachowań.
- Fizyczność: kroki wpisywane ręcznie, aktywności, masa ciała, obwód pasa, praca fizyczna i dodatkowy przychód.
- Rozwój: czytanie, medytacja, gitara, deep work i plan na jutro.
- Finanse: szacowane oszczędności i ręczne dodatkowe przychody.
- Raporty: tygodniowe i miesięczne podsumowania oraz wykresy.
- Historia: możliwość wybrania wcześniejszej daty i edycji.
- Dane: eksport i import JSON, zmiana aktywnego dnia i usuwanie danych.
- PWA/offline: podstawowy cache statycznych plików.

## Publikacja
W repozytorium GitHub `Betterme` umieść `index.html`, `manifest.json`, `sw.js`, `README_PL.md` oraz folder `assets` w katalogu głównym. W Settings → Pages wybierz `Deploy from a branch`, branch `main`, folder `/(root)`.

## Dodanie do ekranu iPhone'a
Otwórz opublikowaną stronę w Safari → przycisk Udostępnij → Dodaj do ekranu początkowego.

## Ważne ograniczenia
- To prywatna aplikacja webowa/PWA, nie natywna aplikacja iOS.
- Nie ma integracji z Apple Health ani powiadomień push.
- Dane są przechowywane w localStorage na tym urządzeniu/przeglądarce. Eksportuj kopię zapasową regularnie. Wyczyszczenie danych Safari może usunąć dane aplikacji.
- Nie przechowuj tu haseł ani danych wrażliwych.
- Wynik dnia jest umownym wskaźnikiem motywacyjnym, nie diagnozą zdrowotną.
- Wskaźnik zachowań nie mierzy poziomu dopaminy.
- To kompletna wersja osobista do testów, ale przed uznaniem jej za stabilną należy przetestować ją na urządzeniu i sprawdzić wszystkie przepływy.

## Zasady punktacji
Fizyczność: poniżej 10 000 kroków = 20 pkt; 10 000–13 999 = 30 pkt; 14 000+ = 40 pkt. Jedna aktywność daje 60 pkt plus punkty krokowe (maks. 100); dwa różne typy aktywności = 100 pkt. Praca fizyczna jest jednym typem aktywności niezależnie od liczby jednostek; 1 jednostka = 150 zł dodatkowego przychodu, maksymalnie 3 jednostki dziennie. Spadek masy o każde pełne 0,5 kg względem poprzedniego pomiaru to +30 pkt bonusu; wzrost masy nie odejmuje punktów. Bonus wagowy nie jest w tej wersji dodawany do wyniku dnia.
