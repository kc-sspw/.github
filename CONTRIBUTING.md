# Współpraca przy projektach KC SSPW

Dzięki za chęć pomocy. Ten dokument opisuje domyślny sposób pracy w repozytoriach Komisji Cyfryzacji SSPW. Konkretne repozytorium może mieć dodatkowe zasady.

## Zanim zaczniesz

1. Sprawdź README projektu.
2. Poszukaj istniejącego Issue dotyczącego zadania.
3. Jeśli temat jest większy lub zmienia kierunek projektu, najpierw opisz propozycję w Issue.
4. Nie umieszczaj w repozytorium haseł, tokenów, kluczy API ani innych sekretów.

## Branch i Pull Request

Dla zmian używaj osobnego brancha, np.:

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

Autor PR nie powinien zatwierdzać własnej zmiany jako jedyny reviewer. W ważniejszych repozytoriach wymagamy co najmniej jednej akceptacji przed merge.

Review służy poprawie rozwiązania i przekazywaniu wiedzy — komentarze powinny być konkretne i merytoryczne.

## Dokumentacja

Jeśli zmiana wpływa na sposób uruchamiania, konfigurację, API albo zachowanie projektu, zaktualizuj odpowiednią dokumentację w tym samym PR.

## Bezpieczeństwo

Podejrzenia dotyczące podatności zgłaszaj zgodnie z plikiem [SECURITY.md](SECURITY.md), a nie w publicznym Issue.
