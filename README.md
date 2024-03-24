# FlaskBlog

Projekt `FlaskBlog` to prosty blog stworzony z wykorzystaniem mikroframeworka **Flask** w języku **Python**. Demonstruje podstawowe funkcje Flask, takie jak routing i renderowanie szablonów.

## Rozpoczęcie pracy

Te instrukcje pomogą Ci uruchomić kopię projektu na lokalnym komputerze do celów deweloperskich i testowych.

### Wymagania wstępne

Aby uruchomić ten projekt, potrzebujesz następujących narzędzi:
- **Python 3**
- **Flask**

### Instalacja

Aby skonfigurować środowisko deweloperskie, wykonaj poniższe kroki:

1. Sklonuj repozytorium na swój lokalny komputer:
- `git clone https://github.com/luczakhubert/cw_praca_z_kodem.git`
2. Przejdź do głównego katalogu projektu.
Zainstaluj wymagane zależności z pliku `requirements.txt`:
- `pip install -r requirements.txt`
Możesz to zrobić również za pomocą komendy `make install` z pliku `Makefile`.

### Uruchamianie

Aby uruchomić aplikację, wykonaj poniższe kroki:

1. Uruchom serwer Flask za pomocą polecenia:
- `python -m flask run`
Alternatywnie, możesz użyć komendy `make run` z pliku `Makefile`.
2. Otwórz przeglądarkę i przejdź do `http://127.0.0.1:5000/` aby zobaczyć stronę główną aplikacji.

#### Użycie Makefile

W projekcie zawarty jest plik `Makefile`, który ułatwia zarządzanie najczęstszymi akcjami, takimi jak instalacja zależności i uruchamianie serwera Flask. Zawiera on definicje trzech głównych komend:

- `make install` - instaluje wszystkie wymagane zależności zdefiniowane w pliku `requirements.txt`.
- `make run` - uruchamia serwer Flask, umożliwiając dostęp do aplikacji przez przeglądarkę internetową.
- `make test` - Uruchamia narzędzie `pylint` na pliku `app.py` w celu analizy kodu i zwrócenia informacji o potencjalnych błędach lub problemach ze stylem kodowania.


Aby zainstalować zależności, wykonaj w terminalu:
- `make install`

Następnie, aby uruchomić aplikację, użyj polecenia:
- `make run`
Po uruchomieniu, aplikacja będzie dostępna pod adresem `http://127.0.0.1:5000/`.

Aby przetestować jakość kodu za pomocą `pylint`, wykonaj:
- `make test`

### Testowanie

Projekt zawiera proste ścieżki, które możesz przetestować za pomocą `curl` lub innego narzędzia do testowania API:
- Strona główna: `curl http://127.0.0.1:5000/`
- Powitanie: `curl http://127.0.0.1:5000/hello/`
- Powitanie z imieniem (w miejsce `<name>` wpisz swoje imię): `curl http://127.0.0.1:5000/hello/<name>`

### Przykładowe zapytania `curl`

Aby przetestować funkcjonalność powitalną, użyj następujących komend:
- curl http://127.0.0.1:5000/hello
- curl http://127.0.0.1:5000/hello/Hubert

## Autor

- **Hubert Łuczak** - *Narzędzia do automatyzacji budowy oprogramowania - zadanie 2* - [MójGitHub](https://github.com/luczakhubert)

## Licencja

Ten projekt został stworzony jako część zadania akademickiego na uczelni WSB Merito. Nie zawiera on dedykowanego pliku `LICENSE.md`, co oznacza, że wszystkie prawa są zastrzeżone przez autora. Projekt jest udostępniony wyłącznie w celach edukacyjnych i nie może być używany, kopiowany ani modyfikowany bez wyraźnej zgody autora lub w ramach dozwolonego użytku edukacyjnego.