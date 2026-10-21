# Better Me — Fizyczność (PWA na iPhone)

To jest osobny prototyp webowy Better Me. Nie wymaga zmian w repozytorium Habitflow.

## Zawartość
- `index.html` — aplikacja i interfejs
- `manifest.json` — konfiguracja instalacji na ekranie początkowym
- `sw.js` — cache/offline shell
- `assets/icon.svg` i `assets/apple-touch-icon.png` — ikony
- dane lokalne: `localStorage` w przeglądarce na tym urządzeniu

## Publikacja przez nowe repozytorium GitHub
1. Na GitHub utwórz **nowe, osobne repozytorium**, np. `BetterMe`.
2. Nie otwieraj ani nie edytuj repozytorium `Habitflow`.
3. W nowym repozytorium dodaj pliki i foldery z tego ZIP-a do katalogu głównego: `index.html`, `manifest.json`, `sw.js`, `README_PL.md`, `assets/`.
4. W repozytorium wybierz **Settings → Pages**.
5. Ustaw publikację z gałęzi `main`, katalog `/ (root)` i zapisz.
6. Po opublikowaniu otwórz podany adres `https://...github.io/BetterMe/` w Safari na iPhonie.
7. W Safari wybierz **Udostępnij → Dodaj do ekranu początkowego**.

## Zasady w prototypie
- Kroki: poniżej 10 000 = 20 pkt; 10 000–13 999 = 30 pkt; 14 000+ = 40 pkt.
- Jedna aktywność + kroki: 60 pkt za aktywność + punkty krokowe, maksymalnie 100.
- Dwie różne aktywności: 100%, niezależnie od kroków.
- Praca fizyczna to jedna aktywność niezależnie od liczby jednostek; 0–3 jednostki, każda daje 150 zł dodatkowego przychodu.
- Dzień zamykasz ręcznie i możesz edytować później.
- Ręcznie wpisane kroki nie są nadpisywane automatycznie.
- Ważenie można wpisać ręcznie; spadek o każde pełne 0,5 kg daje 30 punktów premii tygodniowej.
- Raporty tygodniowe i miesięczne bazują na danych zapisanych w tej przeglądarce.

## Ograniczenia, które trzeba znać przed użyciem
- To PWA, a nie natywna aplikacja iOS.
- Safari/PWA nie może bezpośrednio odczytać HealthKit / Apple Health. W tej wersji kroki wpisuje się ręcznie. Prawdziwa integracja HealthKit wymaga natywnej aplikacji iOS zbudowanej i podpisanej w środowisku macOS lub odpowiednim zdalnym środowisku budowania.
- Przypomnienie o ważeniu jest przypomnieniem wewnątrz aplikacji widocznym po otwarciu jej w niedzielę po 7:00. To **nie** jest systemowe powiadomienie push o 7:00. Prawdziwe powiadomienie push wymaga dodatkowej konfiguracji.
- Dane są przechowywane lokalnie w przeglądarce na tym urządzeniu. Eksportuj kopię JSON z zakładki Historia; wyczyszczenie danych Safari może usunąć dane aplikacji.
- Ten pakiet nie został jeszcze uruchomiony na Twoim iPhonie. Kod JavaScript został sprawdzony składniowo, ale wygląd i zachowanie trzeba potwierdzić po opublikowaniu w Safari.
