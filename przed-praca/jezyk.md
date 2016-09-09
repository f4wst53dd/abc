# Główny język programowania, inne technologie

Jedną z najważniejszych decyzji która stanie przed tobą jest wybór języka/technologii którą masz zamiar opanować. Oczywiście, decyzja ta nie jest ostateczna. Jeśli po kilku miesiącach, latach stwierdzisz, że pora zająć się czymś innym najpewniej będziesz w stanie to zrobić. Jednak początkowy wybór jest ważny, ponieważ wejście w nieodpowiednią technologię może nam utrudnić zdobycie pracy, czy całkiem zniechęcić do nauki programowania.

Efektem podjęcia tej decyzja będzie nie tylko używanie danego języka/frameworka, ale często również zamknięcie się w bańce ekosystemu tego języka. Zatem należy zwrócić uwagę nie tylko na sam język, ale na ilość, dostępność i jakość dodatkowych modułów, bibliotek, narzędzi, programów dostępnych dla danej platformy, dajmy na to Javy.

Pierwsza decyzja dotyczy tego, czy chcesz programować po stronie serwera, klienta czy pośrodku (w obie strony). Programować/kodować po stronie klienta oznacza pisać kod wykonywany przez przeglądarkę internetową użytkownika strony. Osobę, która to robi nazywa się "front end developerem". Z kolei 'backend developer' skupia swoje działania na programowaniu po stronie serwera, czyli w wielkim uproszczeniu - oprogramowywuje większość logiki działania danej strony, łącznie z obsługą serwera, interakcjami z bazą danych, komunikacją  z aplikacjami działającymi na serwerze i zewnętrznymi. Istnieje również trzecia grupa programistów webowych, łącząca umiejętności z dwóch wcześniej wymienionych 'światów': 'Full stack developer'. Prawdopodobnie nie osiągnie tak szczegółowej znajomości technologii jak front- czy backend developerzy, z racji podwojenia ilości rzeczy do nauczenia się, ale jako jedyny będzie w stanie samemu stworzyć stronę od zera. To twierdzenie nieco upraszcza rzeczywistość, bo może dana osoba posiadać np. wiedzę z front-endu pozwalającą na stworzenie aplikacji, ale chcąca pracować i doskonalić się w backendzie.

Którą działkę wybrać? Prawdopodobnie najlepszym wyborem będzie rozpoczęcie nauki od poznania podstaw zarówno frontendu jak i backendu. Nawet jeśli mamy w głowie konkretny kierunek rozwoju (backend lub frontend) podstawy z obydwu dziedzin przydadzą nam się podczas pisania własnego projektu. Oczywiście możemy wykonać aplikację wyłącznie "przeglądarkową" (np. Single-Page Application), lub wyłącznie serwerową (np. API), ale wiedza nabyta przy obydwu na raz pozwoli nam zrozumieć lepiej działanie drugiego 'frontu'. Dodatkowo posiadanie nawet niewielkiego doświadczenia frontendowego może być atutem przy rekrutacji na stanowisko backendowego, i na odwrót.

Następną kwestią jest wybór konkretnych technologii jakimi będziemy się zajmowali.

## Technologie front-endowe:

Obowiązkowa jest klasyczna trójca: HTML5, CSS3, JavaScript (co najmniej w wersji ES5, docelowo również ES2015). W dużym skrócie te języki pozwalają na (w kolejności): opis semantyczny elementów (przycisk, lista, pole do wprowadzania tekstu itp.), wystylizowaniu elementów (kolor, marginesy, rozmiar itd.) oraz oskryptowanie strony (dodawanie/usuwanie znaczników HTML, ustawianie ciasteczek itp.). Dodatkowo za podstawową technologię można uznać bibliotekę języka JavaScript o nazwie JQuery, zatem jej również trzeba się nauczyć. Dzięki JQuery możemy pisać kod bardziej zwięzły niż w czystym (vanilla) JS, tworzyć efekty animacji, wygodnie manipulować elementami strony. Nie bez znaczenia jest również fakt iż istnieje bardzo dużo innych bibliotek opartych właśnie na JQuery.

Wielu pracodawców wymaga lub preferuje również znajomość bibliotek takich jak Backbone.js, React lub frameworka AngularJS. Powinniśmy poznać podstawy najlepiej każdej z tych technologii, oraz przynajmniej jedną z nich poznać bardziej dogłębnie, zwłaszcza jeśli chcemy zostać frontendowcem. Backbone.js jest najstarszą biblioteką z tej trójki, umożliwia ustrukturyzowanie kodu JS. Jest wciąż wykorzystywany, ale jest najmniej popularny. AngularJS, stworzony przez firmę Google AngularJS jest najbardziej rozbudowany, najpopularniejszy i jednocześnie najtrudniejszy w nauce. Istnieje bardzo dużo bibliotek, pluginów napisanych specjalnie pod Angulara. Nie mniej jednak wiele osób wymienia jego wady, takie jak bardzo duże zmiany między wersjami 1.x a 2.x, skomplikowany model przepływu danych, duży rozmiar itp. Najmłodszą biblioteką jest Facebookowy React, który w odróżnieniu od pozostałej dwójki implementuje wyłącznie widok z modelu MVC (Model-View-Controller, Model-Widok-Kontroler). Jest stosunkowo prosty w nauce, i pozwala na łatwe tworzenie interfejsów dzięki prostemu jednokierunkowemu modelowi przepływu danych, możliwość podziału elementów strony na komponenty, elegancki sposób dodawania logiki dla elementów itp. React wciąż jest na etapie kształtowania się, ale mimo to zyskał bardzo dużą popularność.

W ciągu ostatnich lat ekosystem JavaScript rozrósł się do olbrzymich rozmiarów. Niegdyś popularne biblioteki i narzędzia dziś są już przestarzałe, a inne zyskały popularność. Spośród tych drugich na szczególną uwagę zasługują: Redux (do zarządzania stanem w aplikacji, np. w połączeniu z Reactem), TypeScript i Flow (możliwość definiowania typów zmiennych w kodzie JS), ESLint (linter JS), npm (system paczek dla JS), Webpack (system rozwiązywania zależności), BabelJS (umożliwia na korzystanie ze składni najnowszych standardów JS również na starszych przeglądarkach), Lodash (de facto bibliotek standardowa JS, zawierająca wiele przydatnych funkcji do pracy z tablicami, obiektami, liczbami itp.). Nie mniej jednak nawet w niedalekiej przyszłości ekosystem JavaScriptu może ulec zmianom, dlatego warto z jednej strony śledzić bieżące trendy, a z drugiej nie ulegać tymczasowej modzie.

Dodatkowym atutem, oraz w ofertach niektórych firm wymogiem będzie znajomość preprocesorów JavaScriptu (CoffeScript), CSS (SCSS, Sass), czy HTML (Jada, Haml). Preprocesory te umożliwiają pisanie bardziej zwięzłego, mniej podatnego na błędy kodu. Kod języków tych preprocesorów może różnić się bardzo od docelowej formy (np. Slim w porównaniu do HTML). Przeglądarki internetowe nie są w stanie tych języków zinterpretować, dlatego odbywa się konwersja do docelowego języka podczas deploymentu, albo konwersja ta przeprowadzana jest 'w locie', przez serwer aplikacji.

Istnieje również bardzo dużo frameworków HTML/CSS, które zawierają zestaw gotowych komponentów, kolorów, stylów, interakcji, layoutów itp. Najpopularniejszymi są m.in. Bootstrap, Foundation czy implementujący Material Design framework Materialize.

## Technologie backendowe

W praktyce dany język wykorzystuje się razem z frameworkiem, dlatego poniższa lista podaje ich przykłady:

- Java (Play, Spark, Akka HTTP)
- PHP (Laravel, Symfony, Zend)
- Python (Django, Flask)
- Ruby (Ruby on Rails, Sinatra)
- JavaScript/NodeJS (Express.js)
- Elixir (Phoenix)
- Go (Beego, Revel)
- C# (ASP.NET)
- Scala (Play, Spark, Akka HTTP)

Który język i jaki framework wybrać? Możemy podjąć decyzję biorąc pod uwagę kilka kryteriów:
a) popularność. Im więcej osób korzysta z danej technologii, tym łatwiej znaleźć materiały, książki, pomoc na forach itp. Nie mniej istotna jest ilość ofert pracy. Z wymienionych wyżej języków najmniej popularnymi są Go i Elixir, a najpopularniejszymi są Java i PHP.
b) składnia, łatwość tworzenia - każdy z języków posiada własną składnię, która może pewnym osobom nie odpowiadać. Przykładowo w Pythonie poziom wcięcia kodu określa bloki kodu, a niektórzy zapewne woleliby używając do tego celu klamerek: '{ blok_kodu }' jak w Javie, JS czy PHP lub słów kluczowych, np. 'do blok_kodu end' w Ruby. Warto samemu poczytać fragmenty kodu różnych języków, a najlepiej samemu napisać krótkie programy, żeby przekonać się, czy składnia nam odpowiada.

Myślę, że warto zwłaszcza zwrócić uwagę na Javę, Pythona (Django) i Ruby (Ruby on Rails).

Wśród technologii, których znajomość (użycie w projekcie) może być dobrze widziana są m.in.:
- Redis: prosta baza klucz-wartość, a także jako cache aplikacji
- Elasticrsearch; Solr - silniki wyszukiwania (np. wyrażeń tekstowych) w bazie danych
- RabbitMQ; ActiveMQ; Kafka - message brokery (systemy pozwalające na przesyłanie komunikatów między częściami aplikacji)
