# GeoQuiz Europa — zasady pracy

## Projekt

Interaktywny quiz geograficzny o krajach i stolicach Europy. Aplikacja działa jako **pojedynczy plik `index.html`** (HTML + CSS + JS, zero zależności zewnętrznych). Użytkownik otwiera link do strony — nie instaluje niczego.

**Docelowy użytkownik:** dziecko korzystające z aplikacji przez przeglądarkę na **telefonie w orientacji pionowej**.

**Język:** polski — cały interfejs, komunikaty, treść pytań i odpowiedzi po polsku.

## Technologia

* Tylko `index.html` — bez frameworków, bundlerów, node_modules, CDN
* Każda zmiana musi działać offline i bez instalacji po stronie użytkownika
* Nie dodawać zewnętrznych zależności (biblioteki JS, fonty z CDN itp.)
* Layout responsywny zoptymalizowany pod ekran telefonu w pionie (~360-430px szerokości)

## Pliki w repo

* `index.html` — cała aplikacja
* `map.svg` — mapa Europy (DUŻY plik — nie wczytuj go do kontekstu, chyba że zmiana dotyczy bezpośrednio mapy)
* `icon.png`, `LICENSE`, `README.md` — nie ruszaj bez wyraźnej prośby

## Tryby gry i liczba pytań

| Tryb | Liczba pytań |
| --- | --- |
| Stolice | 12 |
| Państwa | 12 |
| Wskaż na mapie | 8 |

## Sposób pracy

### Na starcie sesji

Wykonaj `git pull origin main` na początku każdej rozmowy, żeby mieć aktualny stan repo (bo czasem edytuję pliki bezpośrednio na GitHubie).

### Przy niejednoznacznych zmianach

Jeśli zmiana dotyczy UX, mechaniki gry, struktury danych lub czegoś z więcej niż jednym sensownym rozwiązaniem — zaproponuj 2-3 opcje i zapytaj o wybór zanim zaczniesz kodować. Przy oczywistych poprawkach (literówka, kolor, drobny bugfix, jasno opisane zachowanie) — działaj od razu.

### Komunikacja

* Po zakończeniu zadania krótkie podsumowanie (1-2 zdania), bez powtarzania całego diffu czy listy zmian
* Nie tłumacz oczywistego — zakładaj, że rozumiem podstawy programowania
* Komunikuj się po polsku

### Kodowanie
Plik index.html jest w UTF-8 bez BOM. NIE wstawiaj escape'ów \uXXXX dla polskich znaków, emoji ani strzałek - używaj 
znaków bezpośrednio. Do edycji używaj natywnego tool'a edycyjnego, nie PowerShella.

### Po akceptacji rozwiązania

1. Wprowadź zmiany w kodzie
2. Zrób commit z sensownym opisem po polsku
3. Wypchnij na GitHub

### Commit i push

* Commit message po polsku, zwięzły, opisuje "dlaczego" a nie "co"
* Drobne zmiany (do ~30 linii, jasna intencja) — commit + `git push origin main` od razu, bez pytania
* Większe zmiany lub zmiany w kluczowej logice — pokaż diff i poczekaj na akceptację przed pushem
