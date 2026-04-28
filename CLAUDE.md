# GeoQuiz Europa — zasady pracy

## Projekt

Interaktywny quiz geograficzny o krajach i stolicach Europy. Aplikacja działa jako **pojedynczy plik `index.html`** (HTML + CSS + JS, zero zależności zewnętrznych). Użytkownik otwiera link do strony — nie instaluje niczego.

**Docelowy użytkownik:** dziecko korzystające z aplikacji przez przeglądarkę na telefonie lub tablecie.

## Technologia

- Tylko `index.html` — bez frameworków, bundlerów, node_modules, CDN
- Każda zmiana musi działać offline i bez instalacji po stronie użytkownika
- Nie dodawać zewnętrznych zależności (biblioteki JS, fonty z CDN itp.)

## Tryby gry i liczba pytań

| Tryb | Liczba pytań |
|---|---|
| Stolice | 12 |
| Państwa | 12 |
| Wskaż na mapie | 8 |

## Sposób pracy

### Przy niejednoznacznych zmianach

Zawsze zaproponuj **kilka opcji rozwiązania** i zapytaj o cel produktowy / biznesowy zanim zaczniesz kodować. Przykład: jeśli prośba dotyczy UX, zapytaj czy chodzi o doświadczenie dziecka czy rodzica, o czytelność czy o gamifikację.

### Po akceptacji rozwiązania

1. Wprowadź zmiany w kodzie
2. Zrób commit z sensownym opisem po polsku
3. Wypchnij (`git push origin main`) — automatycznie, bez pytania

### Commit i push

- Commit message po polsku, zwięzły, opisuje "dlaczego" a nie "co"
- Zawsze `git push origin main` zaraz po commicie
