# Umiejętności programistyczne

Web development jest dosyć szeroką dziedziną. Rozmowa techniczna będzie miała za zadanie stwierdzenie, czy twój stan wiedzy jest wystarczająco dobry z głównych technologii oraz na ile szeroką wiedzę posiadasz z pozostałych elementów. Zatem rekrutując się na junior developera prawdopodobnie firma będzie od ciebie wymagać co najmniej dobrej znajomości języka lub/i frameworka (np. Java + Spring) oraz co najmniej podstaw z innych technologii, zagadnień.

Część zagadnień została poruszona także w sekcji [studia](przed-praca/studia.md).

1. Główny język, framework i środowisko
  - warto skupić się przede wszystkim właśnie na tych kluczowych technologiach
  - opanowanie składni języka - swobodne czytanie kodu, umiejętność tworzenia klas, dziedziczenia itp.
  - opanowanie frameworka języka - często frameworki są bardzo rozbudowane, i nawet doświadczeni programiści nie znają na pamięć wszystkich metod, funkcji. Nie mniej jednak tworząc aplikację w tym frameworku powinniśmy zaznajomić się z najczęściej używanymi składnikami
  - znajomość systemu paczek/bibliotek: instalowanie, usuwanie paczek i ich aktualizacja
  - rozumienie logów serwera/aplikacji: interpretacja komunikatów błędów, logów aktywności serwera
  - debugging - podstawowe, prymitywne debugowanie kodu (wyświetlanie wartości zmiennych np. w logach; wywoływanie wyjątków, żeby sprawdzić w jakie części kodu są uruchamiane). Bardziej zaawansowane, przy użyciu debuggera - programu który zatrzyma wykonywanie kodu, pozwala na poruszanie się po kodzie krok po kroku, umożliwia wyświetlenie zmiennych, wykonywanie na nich operacji itp.
  - używanie CLI/REPL, czyli konsoli aplikacji
  - szablony HTML - w jaki sposób generować statyczną treść HTML wraz z dynamicznie dodawaną zawartością (kod framweworka)

2. Przeglądarka internetowa
  - interpretacja komunikatów ostrzeżeń, błędów JavaScriptu
  - poruszanie się po drzewie elementów DOM; usuwanie, dodawanie znaczników, atrybutów itp. bezpośrednio z panelu narzędzi developerskich przeglądarki (np. w Chrome zakładka 'Elements')
  - przeładowanie strony bez użycia cache przeglądarki (Ctrl+Shift+R), lub po uprzednim otwarciu panelu konsoli developerskiej przytrzymanie wciśniętego przycisku przeładowania strony (po lewej stronie paska adresu)
  - debugowanie kodu JS: przez użycie słowa 'debugger' w kodzie; za pomocą ustawiania breakpointów
  - analiza requestów sieciowych podczas działania aplikacji (w Chrome zakładka: Network)
  - analiza profilingu (w Chrome zakładka timeline)

3. Stack sieciowy
  - znajomość podstaw działania i używania serwera aplikacji (np. [Tomcat](http://tomcat.apache.org/), [Phusion Passenger](https://www.phusionpassenger.com/)); dodatkowo np. [Nginx](http://nginx.org/) (w roli reverse proxy)
  - znajomość protokołu HTTP (metody GET, POST itp., jak wygląda request HTTP, odpowiedź HTTP ). Co nowego wprowadza HTTP/2 w porównaniu do HTTP 1.1? Model OSI; protokół TCP i model TCP/IP, co to jest DNS. Kody odpowiedzi HTTP, znajmość [najpopularniejszych kodów](https://www.smartlabsoftware.com/ref/http-status-codes.htm), lub przynajmniej grup (1xx - informacyjne, 2xx - powodzenia, 3xx - przekierowania, 4xx - błędu klienta, 5xx - błędu serwera).
  - [REST](https://en.wikipedia.org/wiki/Representational_state_transfer), metody HTTP (GET, POST itp.)
  - ciasteczka (cookies)
  - URL - z jakich elementów składa się

4. Narzędzia (programy)
  - [cURL](https://curl.haxx.se/): umiejętność wykonywania żądań do serwera (GET, POST); dodawanie parametrów do requestu, ustawianie nagłówków

5. Bezpieczeństwo
  - znajomość popularnych zagrożeń (lista [OWASP Top 10](https://www.owasp.org/index.php/Top10#OWASP_Top_10_for_2013) oraz wiedza jak się przed nimi zabezpieczać
  - podstawy wiedzy nt. SSL, SSH, kryptografii symetrycznej/asymetrycznej

6. Frontend
  - HTML5, CSS3, Sass
  - znajmomość JavaScript (przynajmniej w wersji ES5, docelowo również nowszą - ES2015)
  - JQuery

7. Baza danych
  - znajomość PostgreSQL/MySQL. Obsługa bazy za pomocą GUI (np. PgAdmin dla PostgreSQL), jak i za pomocą interfejsu konsolowego
  - język SQL - znajomość podstawowych poleceń (tworzenie/edycja/usuwanie baz, tabel, rekordów; wyciąganie danych poleceniem SELECT)
  - zagadnienia optymalizacyjne: indeksy, N+1 query problem, sharding

8. Deployment
  - deployment na zewnętrznym 'czystym' serwerze VPS. Dodatkowo opcjonalnie na serwerze PaaS, np. Heroku
  - narzędzia/skrypty deploymentu, np. [Capistrano](http://capistranorb.com/)

9. Patterny
  - [zasada SOLID](https://en.wikipedia.org/wiki/SOLID_(object-oriented_design))

Czy trzeba mieć certyfikaty programistyczne (z kursów, szkoleń itp.)? Generalnie nie. Mogą być one dodatkowym atutem, miłym ozdobnikiem CV, ale nie należy im poświęcać dużej uwagi. Liczą się przede wszystkim umiejętności i wiedza którą posiadasz w momencie rekrutacji. Jeśli np. podczas studiów masz okazję zrobić jakiś certyfikat, za darmo lub okazjonalną cenę to warto co najmniej rozważyć wzięcie udziału w takim szkoleniu. Jednak nie wolno certyfikatów traktować jako kluczy, które magicznie otworzą nam drzwi dowolnego pracodawcy.
