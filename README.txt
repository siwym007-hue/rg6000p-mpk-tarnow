R&G 6000P SIMULATOR – WERSJA 0.8
MPK TARNÓW – pakiet przygotowany do publikacji przez HTTPS (GitHub Pages)

CO ZMIENIA WERSJA 0.8
- Dodano automatyczne zapowiedzi przystanku końcowego.
- Dodano możliwość tworzenia dowolnej liczby kierunków (minimum dwa) dla jednej linii.
- Dodano automatyczne przejście do następnego przystanku po opuszczeniu strefy bez zaliczenia.
- Zaliczenie nadal wymaga otwarcia drzwi i naciśnięcia przycisku „ZALICZ PRZYSTANEK”.
- Zachowano uruchamianie przez HTTPS i obsługę GPS.

JAK OPUBLIKOWAĆ APLIKACJĘ NA GITHUB PAGES
Potrzebne jest konto GitHub. Publikacja jest bezpłatna dla publicznego repozytorium.

1. Na komputerze rozpakuj ZIP. Wejdź do folderu rg6000p_v08.
2. Zaloguj się na https://github.com i utwórz nowe repozytorium (New repository).
3. Nazwij je np. rg6000p-mpk-tarnow. Wybierz Public i utwórz repozytorium.
4. W repozytorium wybierz Add file → Upload files.
5. Przeciągnij do okna pliki z folderu rg6000p_v08: index.html, manifest.webmanifest i README.txt. Ważne: index.html ma znajdować się bezpośrednio w głównym katalogu repozytorium, a nie w dodatkowym folderze.
6. Zatwierdź przyciskiem Commit changes.
7. Wejdź w Settings → Pages. W sekcji Build and deployment wybierz Deploy from a branch.
8. Jako Branch wybierz main, a folder /(root), następnie Save.
9. Poczekaj, aż GitHub opublikuje stronę. Adres będzie miał postać https://TWOJ_LOGIN.github.io/rg6000p-mpk-tarnow/ .
10. Otwórz ten adres w Chrome na telefonie. Wejdź w Ustawienia aplikacji → „Poproś o dostęp i sprawdź GPS” i zezwól na lokalizację.

WAŻNE – GPS NA ANDROIDZIE
- Włącz lokalizację w ustawieniach telefonu.
- W Chrome, dla opublikowanej strony, ustaw uprawnienie Lokalizacja na Zezwalaj.
- Przy pierwszym teście najlepiej stać na zewnątrz lub przy oknie i odczekać kilkanaście–kilkadziesiąt sekund.
- W ustawieniach Androida można sprawdzić: Aplikacje → Chrome → Uprawnienia → Lokalizacja.
- Jeśli strona była już wcześniej blokowana, otwórz informacje o witrynie przy pasku adresu Chrome i zmień Lokalizację na Zezwalaj.
- Nie uruchamiaj index.html z menedżera plików. Korzystaj z adresu https://...github.io/...

DANE I PRYWATNOŚĆ
Konfiguracja linii i przystanków jest zapisywana w pamięci przeglądarki na danym urządzeniu i w danym profilu Chrome. Po publikacji na HTTPS dane z poprzedniego uruchomienia przez content:// nie przeniosą się automatycznie – użyj eksportu/importu konfiguracji, jeśli masz przygotowaną bazę.
Repozytorium GitHub będzie publiczne, więc opublikowane w nim pliki aplikacji będą widoczne dla innych. Dane wpisywane podczas korzystania z aplikacji nie są automatycznie wysyłane do GitHub; pozostają w pamięci lokalnej przeglądarki. Nie umieszczaj w repozytorium prywatnych danych.

OGRANICZENIA
To nadal aplikacja przeglądarkowa, a nie natywny APK. HTTPS umożliwia przeglądarce poproszenie o lokalizację, ale nie gwarantuje działania GPS w tle po zablokowaniu ekranu. Do niezawodnego śledzenia w tle potrzebna będzie natywna aplikacja Android z usługą lokalizacji na pierwszym planie.


ZMIANY WERSJI 0.8
- Ostatni przystanek każdego kierunku jest automatycznie traktowany jako przystanek końcowy.
- Zapowiedź przed strefą: „Następny przystanek” → nazwa przystanku → (dla ostatniego przystanku) „Przystanek końcowy”.
- Po wjeździe w strefę końcową: nazwa przystanku → komunikat o opuszczeniu pojazdu i podziękowanie MPK Tarnów.
- Linia obsługuje dowolną liczbę kierunków (minimum dwa); w edycji linii dostępny jest przycisk „Dodaj kierunek”.
- Wyjazd ze strefy bez zaliczenia przystanku automatycznie przesuwa trasę na następny przystanek. Zaliczenie nadal wymaga otwarcia drzwi i naciśnięcia przycisku „ZALICZ PRZYSTANEK”.
