1. Należy pobrać pliki app.py, index.html, hello.html, requirements.txt z Moodla 
2. Utwórz folder templates i umieść tam pliki index.html oraz hello.html. Zmiany wrzuć na swoje repozytorium na gicie
3. Utwórz plik Makefile w folderze głównym projektu. Dodaj do pliku dwie komendy: 

install:
	pip install -r requirements.txt

run:
	python -m flask run
    
Wrzuć zmiany na swoje repozytorium na gicie.

4. Uruchom plik Makefile. Jeśli nie możesz zaisntalować wymaganego środowiska, wykorzystaj do tego git bush. 
Pamiętaj, żeby być w głównym katalogu projektu.

make install

make run

5. Zainstaluj curly na swoim środowisku - pip install curly (jeśli korzystasz z git basha, tam również zainstaluj)
6. Uruchom kolejny terminal (może być git bash lub terminal w pycharmie) oraz wykonaj kolejne komendy:
curl http://127.0.0.1:5000/
curl http://127.0.0.1:5000/hello
curl http://127.0.0.1:5000/hello/<name>
*w miejsce <name> wpisz swoje lub przykładowe imię
    