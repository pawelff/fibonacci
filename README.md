# Lab8

- Dockerfile.dev1 - wersja developerska bez montowania volumenów
- docker-compose-dev.yml - developerska wersja bazująca na Dockerfile.dev, montująca volumeny, zmiany w kodzie od razu widoczne w uruchomionym kontenerze
- docker-compose2.yml - developerska wersja bazująca na Dockerfile.dev, uruchamia 2 kontenery, jeden uruchamiający aplikację, drugi uruchamiający testy
- Dockerfile i docker-compose.yml - wersja produkcyjna, multistage build, aplikacja uruchomiona na nginx

##
- .travis.yml - konfiguracja dla Travis CI. Po wypchnięciu zmian i zrobieniu pull requesta travis odpala testy. Po mergu do mastera aplikacja jest wdrażana na AWS Elastic Beanstalk
[Wdrożona aplikacja](http://lab8fullstack-env.eba-hsn8hz3e.eu-central-1.elasticbeanstalk.com/)