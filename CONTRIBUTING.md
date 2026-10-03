# Współpraca przy projektach KC SSPW

Dzięki za chęć pomocy. Ten dokument opisuje domyślny sposób pracy w repozytoriach Komisji Cyfryzacji SSPW. Konkretne repozytorium może mieć dodatkowe zasady.

## Dwa tryby repozytoriów

W organizacji utrzymujemy zarówno **projekty Komisji**, jak i **repozytoria szkoleniowe**. Nie wymagają one identycznego procesu.

### Projekty Komisji

Dla aplikacji, narzędzi i innych repozytoriów, które mają być dalej utrzymywane:

- pracujemy przez Issues i Pull Requesty,
- ważniejsze zmiany przechodzą review,
- dokumentujemy sposób uruchomienia i utrzymania,
- unikamy bezpośrednich zmian na `main`, jeśli repozytorium jest współdzielone.

### Repozytoria szkoleniowe

Repozytoria tworzone przez uczestników podczas szkoleń służą przede wszystkim nauce i eksperymentowaniu.

W takich repozytoriach:

- Pull Requesty i code review **nie są obowiązkowe**,
- uczestnik może pracować bezpośrednio na własnym repozytorium,
- kod może być nieukończony lub eksperymentalny,
- najważniejsze jest, aby repozytorium było czytelnie oznaczone jako materiał szkoleniowy,
- nie należy przechowywać prawdziwych haseł, tokenów, kluczy API ani innych sekretów.

Prowadzący może wprowadzić dodatkowe zasady dla konkretnego szkolenia.

## Zanim zaczniesz pracę nad projektem Komisji

1. Sprawdź README projektu.
2. Poszukaj istniejącego Issue dotyczącego zadania.
3. Jeśli temat jest większy lub zmienia kierunek projektu, najpierw opisz propozycję w Issue.
4. Nie umieszczaj w repozytorium haseł, tokenów, kluczy API ani innych sekretów.

## Branch i Pull Request

Dla zmian w utrzymywanych projektach używaj osobnego brancha, np.:

- `feat/nazwa-funkcji`
- `fix/opis-bledu`
- `docs/opis-zmiany`
- `chore/opis-zmiany`

Pull Request powinien być możliwie mały i dotyczyć jednego logicznego tematu.

W opisie PR podaj:

- co zostało zmienione,
- dlaczego zmiana jest potrzebna,
- jak ją sprawdzić,
- powiązane Issue, jeśli istnieje.

## Commity

Preferujemy krótkie, opisowe komunikaty, np.:

- `feat: add event registration form`
- `fix: handle expired session`
- `docs: update local setup`

Nie jest wymagane idealne stosowanie Conventional Commits, ale komunikat powinien jasno mówić, co zmienia commit.

## Review

W utrzymywanych projektach autor PR nie powinien zatwierdzać własnej zmiany jako jedyny reviewer. W ważniejszych repozytoriach wymagamy co najmniej jednej akceptacji przed merge.

Review służy poprawie rozwiązania i przekazywaniu wiedzy — komentarze powinny być konkretne i merytoryczne.

Ta zasada nie dotyczy domyślnie repozytoriów tworzonych przez uczestników podczas szkoleń.

## Dokumentacja

Jeśli zmiana wpływa na sposób uruchamiania, konfigurację, API albo zachowanie utrzymywanego projektu, zaktualizuj odpowiednią dokumentację w tym samym PR.

## Bezpieczeństwo

Podejrzenia dotyczące podatności zgłaszaj zgodnie z plikiem [SECURITY.md](SECURITY.md), a nie w publicznym Issue.
