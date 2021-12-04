# Lab8

- Dockerfile.dev1 - wersja developerska bez montowania volumenów
- docker-compose-dev.yml - developerska wersja bazująca na Dockerfile.dev, montująca volumeny, zmiany w kodzie od razu widoczne w uruchomionym kontenerze
- docker-compose2.yml - developerska wersja bazująca na Dockerfile.dev, uruchamia 2 kontenery, jeden uruchamiający aplikację, drugi uruchamiający testy
- Dockerfile i docker-compose.yml - wersja produkcyjna, multistage build, aplikacja uruchomiona na nginx