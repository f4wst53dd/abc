# Słowniczek

- __senior (senior developer)__ - programista, który wyróżnia się umiejętnościami, stażem pracy, doświadczeniem od reszty developerów; zob. developer, junior developer. Jest on odpowiedzialny za pieczę nad projektem (wieloma projektami). Zwykle od niego zależą najważniejsze decyzje, typu modyfikacja architektury aplikacji, wprowadzenie do niej kolejnej technologii/framweorka. Często mentor, do którego szeregowi programiści, juniorzy a nawet inni seniorzy zwracają się z problemem, albo o poradę. Osoba, która również może wykonywać

- __junior__ - programista, który ma zerowe lub b. małe doświadczenie. Może nie znać niektórych prostych technik, pojęć. Jakość pisanego przez niego kodu zwykle jest gorsza, a zadania wykonuje wolniej niż zwykły developer. Zwykle nie jest samodzielny, tzn. musi korzystać z pomocy innych developerów. Prawdopodobnie w ciągu kilku miesięcy nabierze doświadczenia, i płynnie może być nazywany developerem.

- __developer__ - programista, który ma więcej doświadczenia niż junior, ale mniej niż senior. Umowna grupa, w której znajduje się najwięcej developerów. Ma przynajmniej kilka miesięcy doświadczenia. Jest samodzielny, tzn. może samemu stworzyć dany ficzer, ew. raz na jakiś czas zasięgając rady seniora.

- __produkcja (serwer produkcyjny)__ - środowisko, przeznaczone dla odbiorców końcowych (klientów, użytkowników). Zob. dev, stage, UAT

- __stage (staging) server, lub UAT (User Acceptancy Test, spolszcz. łat)__ - środowisko (serwer), wykorzystywany przez wyznaczone osoby (tester, klient, sam developer) od testowania zmian. Jest on bardzo zbliżony do produkcji, ale zamiast prawdziwych użytkowników korzystają z niego wspomniani wcześniej ludzie. Na stage możemy upewnienie się czy dane zmiany są poprawne, i działają w środowisku produkcyjnym. Czasem bowiem zmiany mogą działać bezproblemowo w środowisku developerskim (dev), a na produkcyjnym już nie.

- __dev (development) server__ - środowisko w który programista przygotowuje zmiany. Zob. stage, uat, produkcja

- __web__ - wersja strony dla komputerów, dostępna przez zwykłą przeglądarkę. 'Zobaczyć coś na webie' - otworzyć stronę aplikacji w przeglądarce.

- __product manager, PM__ - osoba zajmująca się projektem od strony zarządzania nim. Komunikuje się z zespołem programistów, kładąc nacisk tworzenie najpilniejszych/najpotrzebniejszych ficzerów. Jest pośrednikiem między klientem a programistami, dzięki czemu developerzy mogą zajmować się programowaniem. Zajmuje się ustaleniem tego, co będzie robione w najbliższej przyszłości, zgodnie z potrzebami klienta a jednocześnie uwzględniając w pewnym stopniu preferencje developerów (np. może wynegocjować odsunięcie taska, którego wykonanie byłoby bardzo trudne i poza kompetencjami developera).

- __HR (kadry, ejdż-ar, ang. Human Resources)__ - sekcja w firmie (i osoby w niej pracujące), które zajmują się wyszukiwaniem i pozyskiwaniem nowych pracowników dla firmy. Przeglądają nadesłane CV, wybierają odpowiednie osoby. Zwykle przeprowadzają część nietechniczną rozmowy rekrutacyjnej.

- __tracker, bugtracker, bug tracking system__ - aplikacja (może być webowa), która służy do zarządzania taskami (błędami, ficzerami itp.). Zwykle klient chcący mieć wykonane jakieś zadanie umieszcza go w tym systemie. Developer oznacza ten task jako rozpoczęty, zakończony lub jako wrzucony na staging. Klient wtedy widzi postęp prac, i może np. skomentować task, jeśli jest już on na stage, a nie spełnia do końca jego oczekiwań.

- __task, zadanie__ - zadanie, które jest pojedynczą jednostką 'czegoś do zrobienia' dla developera. Czasami zawiera kilka(naście) podtasków - podzadań. Rodzajem taska może być ficzer, bug, chore, research itp.

- __ficzer (ang. feature)__ - zadanie, które polega na stworzeniu nowej funkcjonalności, lub modyfikacji/usunięcia istniejącej. Przykład: trzeba wykonać system logowania aktywności użytkowników.

- __bug (spolszcz. bag)__ - błąd w działaniu aplikacji, objawiający się uzyskaniem niepożądanym spadkiem wydajności, zwracaniem niepoprawnych wyników, czy nawet zawieszeniem się (crashem) całej aplikacji.

- __chore (wym. 'czor')__ - proste zadanie, które nie jest ficzerem ani bugiem. Przykładem chora może być prośba klienta o wyciągnięcie z bazy wszystkich użytkowników, którzy są użytkownikami premium, i zapisanie ich danych w pliku Excela.

- __research__ - zadanie, które polega na wyszukaniu najlepiej nadających się narzędzi/biblioteki do implementacji danego zadania, albo stwierdzenie, czy dane zadanie w ogóle jest możliwe do wykonania. Przykład: klient prosi o research jakiego systemu powiadomień użyć na urządzeniach mobilnych.

- __crash__ - zatrzymanie się aplikacji, spowodowane błędem

- __QA - qualiy assurance__ (zapewnienie jakości), wym. 'kju-ej' - dział/zawód zajmujący się szeroko pojętym testowaniem aplikacji w celu minimalizacji ilości błędów jakich mogliby doświadczyć użytkownicy. Osoba QA pisze testy automatyczne (kod testów), lub 'przeklikuje' stronę podobnie jak zwykły użytkownik, i stara się wyłapać wszelkie niedociągnięcia (graficzne, UXowe, w logice działania). Błędy raportowane są do developera, który powinien je poprawić.

- __CI (Continous Integration)__ - praktyka polegająca na ciągłym włączaniu zmian z własnego brancha do brancha głównego, często wielokrotnie w ciągu dnia. Dzięki temu unika się scenariusza: developer pracuje na własnym branchu przez dłuższy czas. W międzyczasie główny branch bardzo się zmienił, zatem ciężko jest włączyć zmiany z brancha developera do brancha głównego. Najczęściej serwer CI automatycznie uruchamia testy automatyczne aplikacji, dzięki czemu developer od razu dostaje informację gdy testy nie przechodzą (tj. wprowadzone zmiany powodują błędy).

- __UX, usability__ - pojęcia związane z wrażeniami, jakich doświadcza użytkownik korzystający ze strony/aplikacji. Dotyczy ergonomii, zapewnienie łatwego w obsłudze interfejsu, odpowiednio dobranej szaty graficznej, rozmiaru elementów na stronie itp. 'Zły UX' - gdy z jakiejś części aplikacji źle się korzysta, np. zamiast użyć paginacji jest b. długa lista elementów.

- __paginacja__ - metoda prezentacji dużej ilości danych polegająca na rozbiciu jednej, dużej listy elementów na podstrony. Klikając na dany numer strony użytkownik zobaczy właściwą porcję danych. Tak jak "infinite scrolling", metoda ta oszczędza zasoby serwera, bo nie wyświetlamy wszystkich danych na raz, tylko ich część.

- __infinite scroll(ing)__ - nieskończone przewijanie - technika prezentacji dużej ilości danych na stronie. Polega wyświetleniu wstępnej porcji elementów (np. 20 obrazków) wraz z doczytywaniem kolejnych na bieżąco. Użytkownik przewija (scrolluje) stronę w dół. Gdy zaczyna wyświetlać ostatni obrazek, strona doczytuje kolejną porcję danych (np. kolejne 20 obrazków), pozostawiając poprzednie na miejscu. Proces ten powtarza się dopóki użytkownik scrolluje w dół, i istnieją kolejne elementy do pokazania.

- __hamburger__ - menu strony www wykorzystywane głównie w wersji na urządzenia mobilne. W odróżnieniu od zwykłej, webowej wersji strony, mobilna ma ograniczone miejsce do wyświetlenia, zatem menu strony jest schowane pod ikonką hamburgera. Ikoną hamburgera są trzy krótkie poziome kreski jedna nad drugą, stąd nazwa.

- __sprite__ - pojedynczy plik graficzny, który składa się z 'posklejanych' wielu mniejszych obrazków. Używa się go po to, żeby zminimalizować ilość requestów (zob.) do serwera - mając 20 małych obrazków złączonych w 1 spricie nie wykonujemy 20 osobnych requestów do serwera (co wiąże się z dodatkowym narzutem czasowym dla użytkownika, jak i narzutem obsługi większej ilości żądań dla serwera), ale przesyłamy je do przeglądarki jako odpowiedź na pojedynczy request. W kodzie CSS podajemy możemy dokładne współrzędne na podstawie których wyciągamy tylko taki fragment sprita, który jest akurat potrzeby do wyświetlenia (np. obrazek przycisku). Użycie sprite jest sensowne, gdy mamy dużą ilość bardzo małych obrazków. Standardowym przykładem jest sprite z przyciskami, elementami obramowania.

- __maintanance, utrzymywanie__ - etap w cyklu życia aplikacji, w którym nie dodaje się aktywnie (regularnie, często) nowych ficzerów, jedynie dogląda się go. Monitorujemy czy aplikacja działa, poprawiamy okazjonalnie bugi, ewentualnie raz na jakiś czas wykonujemy drobne zadania dodające coś do funkcjonalności. Tak można określić działającą aplikację (korzystają z niej użytkownicy), która jest wykonana, i to na tyle dobrze, że zwykle działa poprawnie, a klient nie ma funduszy/potrzeby żeby ją dalej rozwijać.

- __minified__ - zmniejszony rozmiaru pliku. Zwykle wykonuje się tą operację dla plików CSS i JS. W obu przypadkach usuwany niepotrzebne znaki białe (spacje, tabulatory, znaki nowej linii. JavaScript dodatkowo nazwy zmiennych, funkcji itp. zamieniane są na jak najkrótsze. Dzięki temu skrypt wciąż będzie działał dokładnie tak jak w pierwotnej formie, ale będzie zajmował mniej miejsca, zatem szybciej zostanie przesłany przez sieć.

- __preprocesor__ - w przypadku technologii webowych jest to program, który zamienia jeden język na drugi. Źródłowym językiem jest zwykle język, który oferuje prostszą składnię, bardziej zwięzłą i inne usprawnienia. Językiem docelowy jest z kolei tak, który będzie zrozumiany przez np. przeglądarkę. Przykładami preprocesorów są Jade (preprocesor HTML), i CoffeScript (preprocesor JavaScriptu).

- __linter__ - program, który analizuje kod aplikacji, i zgłasza potencjalne błędy składniowe, stylistyczne itp. Przykład: ESLint, popularny linter dla języka JavaScript.

- __request (żądanie)__ - odpytywanie zasobów, często dostając odpowiedź, która zawiera informację nt. pomyślności wykonania tego requestu. Przykładowo, wchodząc na jakąś stronę przeglądarka wykonywuje zwykle wiele requestów. Pobranie zawartości strony internetowej wiąże się z wykonywaniem osobnych requestów do pobrania kodu HTML, plików stylów CSS, plików JavaScriptu, obrazków). W celu zmniejszenia ilości requestów dla środowiska produkcyjnego, wykonuje się minifikację i konkatenację plików JS i CSS (nie HTML!) oraz sprite'y obrazków.

- __endpoint__ - adres URL, na który możemy wykonywać requesty. Np. dana strona może mieć kilka endpointów, 'http://example.com/songs' zwracający listę piosenek, 'http://example.com/books/xyz' - zwracający listę książek autora 'xyz'

- __API__ - ściśle określony zestaw reguł według których aplikacje komunikują się ze sobą. W przypadku web developmentu strony często oferują API, za pomocą którego możemy pobrać interesujące nas dane (np. listę ulubionych piosenek z youtube.com) lub wykonać jakąś operację (dodać piosenkę do playlisty). Używając API nie wyświetlamy elementów interfejsu (stylów, kodu HTML, plików JS), tylko wysyłamy/otrzymujemy ustrukturyzowane dane, np. w formacie JSON czy XML. W innym znaczeniu: API jest listą wszystkich możliwych elementów interfejsu danej biblioteki, frameworka. Przykładem jest witryna https://api.jquery.com

- __wyjątek (ang. exception)__- mechanizm umożliwiający zgłoszenie wyjątkowego przypadku, np. błędu. Wyjątek może wywołać programista w kodzie (żeby potem go w innej części kodu obsłużyć), lub może być wywołany z biblioteki/języka programowania. Przykład: tworzymy duży plik ze statystkami. Jeśli zabraknie nam miejsca na dysku twardym do utworzenia go podnosimy wyjątek.

- __500 (Internal Server Error, pięćsetka)__ - kod odpowiedzi requestu HTTP HTTP oznaczający błąd wykonywania kodu po stronie serwera. Może pojawić się, gdy np. programista popełni błąd składniowy w kodzie
- __404 (not found)__ - kod odpowiedzi requestu HTTP
- __200 (OK)__- kod odpowiedzi requestu HTTP, który oznacza poprawne jego wykonanie

- __polyfill__ - kod implementujący daną rzecz, która nie jest wspierana przez przeglądarkę. Np. starsze wersje przeglądarek nie obsługują JavaScript ES2015. Projekt Babel implementuje te elementy przy użycie starszej wersji JS (ES5), która jest obsługiwana przez każdą przeglądarkę.

- __code review__ - ocena kodu. Proces polegający na przeglądnięciu zmian w kodzie wykonanych przez innego programistę. Wykonywany przez 1 lub więcej ludzi. W przypadku znalezienia błędu, możliwości lepszego zapisu kodu, znalezienia optymalizacji przeglądający kod może umieścić komentarz w kodzie (jeśli review przeprowadzony jest na pull requeście), lub rozmawiając z autorem zmian.

- __pull request, PR__ - przygotowany przez programistę zbiór zmian w kodzie, który dotyczy zwykle jednej funkcjonalności (typu implementacja logowania przez facebooka, poprawienie błędu czy usunięcie nieużywanych plików). Zawiera jeden lub wiele commitów. PR-a tworzymy nie w bezpośrednio w systemie kontroli wersji (lokalnie), ale na stronie hostingu kodu (np. github, bitbucket, gitlab). Pozwala na łatwe wyszukiwanie zmian w historii - wystarczy przejrzeć listę starych pull requestów.

- __commit__ - pojedyncza zmiana w kodzie, zapisana w systemie kontroli wersji. Może ona dotyczyć jednego lub wielu plików. Cała historia zmian w projekcie to zbiór commitów.

- __fork__ - projekt oparty na innym projekcie, rozwijany osobno, w innym kierunku; lub utworzenie kopii procesu systemowego

- __cache__ (wym. 'kasz') - pamięć podręczna. Miejsce w którym umieszczane są dane, do które chcemy mieć szybszy dostęp. Np. cache bazy danych umieszcza część danych w RAM, do którego jest szybszy dostęp w porównaniu do standardowego miejsca przechowywania danych bazy danych (dysk twardy).

- __flaga__ - zmienna w kodzie, na podstawie której wykonujemy (lub nie wykonujemy) jakąś część kodu. Najprostszym rodzajem flagi jest zmienna binarna (o wartości 'true' lub 'false'). Na przykład mamy w funkcji skomplikowaną logikę biznesową. Chcemy wykonać zapis do pliku pod koniec tej funkcji, po wystąpieniu konkretnych warunków. Możemy wtedy utworzyć flagę 'var saveToFile = false', w dalszym kodzie ustawiamy jej wartość na 'true' jeśli wystąpią wspomniany warunki. Pod koniec kodu funkcji sprawdzamy wartość flagi, i zapisujemy plik jeśli ma ona wartość 'true'.

- __logika biznesowa__ - implementacja wymaganych rzeczy w aplikacji, według wizji jej właściciela (klienta); według specyfikacji. Np. klient wymaga, żeby wyliczyć statystyki za pomocą wymyślonego przez niego wzoru. W przypadku wystąpienia danych okoliczności (np. użytkownik aplikacji opłacił konto premium, jest konkretna pora dnia itp.) możliwa jest zmiana sposoby wyliczania statystyk. Logika prowadząca do wykonania tego typu rzeczy jest właśnie logiką biznesową.

- __mockup__ - zarys, koncept aplikacji lub jej części. Może być zrobiony w programie graficznym lub programie specjalnie do tego celu wykonanym; odręczny rysunek, prezentacja PowerPoint itp. Zwykle jako dodatek do opisu słownego, pozwala na pokazaniu developerowi jaki wygląd powinien zostać osiągnięty. W przypadku web developmentu mockupem może być przygotowana przez frontendowca wstępna wersja strony www, zawierająca jedynie wygląd (obrazki, ostylowanie), z treścią wprowadzoną 'na sztywno'.

- __deployment__ - proces wysłania aplikacji na serwer produkcyjny lub stagingowy. W odróżnieniu od środowiska developerskiego, gdzie edytujemy kod bezpośrednio zmieniając zawartość plików i widzimy od razu zmiany na stronie po jej odświeżeniu w przeglądarce, tu proces jest bardziej skomplikowany. Zwykle deployment wykonywany jest przez przeznaczone do tego oprogramowania/skrypt. Przykładowe elementy procesu deploymentu: utworzenie kopii obecnie działającej wersji kodu; zaciągnięcie najnowszego kodu z zewnętrznego repozytorium, np. z githuba; uruchomienie testów Continous Integration; zainstalowanie nowo dodanych bibliotek, przeprowadzenie migracji bazy danych; restart serwera.

- __migracja bazy danych__ - proces zaaplikowania jednego lub kilku plików migracji. Pliki migracji zawierają wszystkie zmiany przeprowadzone w schemacie bazy danych (dodanie/usunięcie kolumny w tableli, dodanie/usunięcie tabeli, zmiana typu kolumny, zmiana wartości domyślnej kolumny itp.), a także niektóre inne modyfikacje (np. skrypt przeliczający wartości po zmianie struktury schematu bazy).

- __release__ - wypuszczenie kolejnej wersji oprogramowania na światło dzienne, na serwerze produkcyjnym. W zależności od przyjętej polityki releasowania dla danego projektu może być od przeprowadzony w dowolnym czasie, lub np. raz na 2 tygodnie, lub po zebraniu się wystarczająco dużej ilości zmian.

- __debugowanie__ - proces znalezienia przyczyny błędu w kodzie i miejsca jego wystąpienia. Istnieją wyspecjalizowane do tego celu programy, debuggery. Umożliwiają one ustawianie breakpointów, wykonywanie kodu linia po linii.

- __breakpoint__ - w procesie debuggingu jest to oznaczenie danej linii kodu po to, żeby debugger zatrzymał działanie aplikacji tuż przed wykonaniem tej linii. Dzięki breakpointowi możemy stwierdzić czy uruchamia się dany fragment kodu. Zwykle programista ma możliwość analizy wartości zmiennych podczas pauzy breakpointa, dzięki czemu może uniknąć on np. żmudnego wyświetlania każdej zmiennej.

- __feedback__ - informacja zwrotna. Przykładem feedbacku może być implementacja danej funkcjonalności, i wystawienie jej na serwerze stagingowym, po to, żeby klient mógł sprawdzić, czy jest wszystko w porządku. Klient, jeśli implementacja nie jest dokładnie zgodna z tym co oczekuje powie/napisze ci np. 'trzeba poprawić kolor belki na jaśniejszy; walidacja pola X ma być wykonywana tylko jeśli użytkownik zaznaczył checkboxa A. Poza tym wszystko jest OK.' Ten komentarz jest feedbackiem dla ciebie.

- __edge case__ (przypadek skrajny) - rzadki, bardzo odbiegający od zwykłych okoliczności przypadek, który np. powoduje nieprawidłowe działania aplikacji. Przykładem edge casa może być to, że użytkownik aplikacji posiada 110 obiektów edycji dokumentu, a interfejs naszej aplikacji potrafi wyświetlić ich tylko 100.

- __stack/stos (technologii)__ - lista głównych technologii użytych w danej aplikacji. Dotyczy języków programowania, frameworków, bibliotek itp.

- __vanilla__ (np. vanilla JS) - 'czysta' wersja kodu, napisana w danym języku, bez użycia dodatkowych bibliotek.

- __protokół__ - zbiór reguł dzięki którym dwa i więcej urządzeń/aplikacji/serwerów itp. może się komunikować, być w stanie wysłać informacje i zrozumieć otrzymane.

- __skalowalność__ - możność rozbudowy systemu, aplikacji. W przypadku web developmentu skalowalność oznacza zwiększenie ilości użytkowników, i w konsekwencji większe zużycie zasobów serwera.

- __brute force__ - metoda rozwiązania problemu która wykorzysta wszystkie możliwe przypadki i ich kombinacje. Często istnieje bardziej "eleganckie" rozwiązanie oprócz brute force, z wykorzystaniem jakiegoś algorytmu, czy analizując wstępnie dane. Zwykle też brute force jest najwolniejszy spośród istniejących rozwiązań problemu.

- __race condition__ - w przypadku kodu wykonywanego równolegle sytuacja, kiedy dwa wątki pracują na wspólnym zestawie danych, i w konsekwencji powodująca niespodziewane, losowe wyniki.

- __callback (wywołanie zwrotne)__ - mechanizm pozwalający na wykonanie danego kodu w nieokreślonej przeszłości, po zakończeniu działania innego kodu. Np. chcemy wykonać request do zewnętrznego serwisu, a po otrzymaniu odpowiedzi z tego serwera (musimy uzyskać tą odpowiedź) uaktualnić rekord użytkownika w bazie danych. Request może potrwać długo, ponieważ problemem może być wolne łącze internetowe, czy wolna odpowiedź zewnętrznego serwisu (lub jej brak). Żeby nie zatrzymywać przebiegu kodu, możemy dodać callback do akcji wysyłania requesta, który zawierać będzie kod aktualizacji rekordu bazy.

- __webhook__ - metoda powiadamiania innej aplikacji webowej za pomocą callbacku. Webhook zwykle jest zdefiniowany żeby zareagować na dane zdarzenie. Przykładowo chąc uruchomić testy na serwerze Continous Integration natychmiast po zpushowaniu nowego kodu np. na Githubie, definiujemy webhooka w Githubie. Webhook ten wyśle request do servera CI, na co serwer ten zareaguje uruchomieniem testów.

- __refaktoryzacja (ang. refactoring)__ - jest to przeprowadzenie takich zamian w kodzie, które ulepszają go, ale przy tym nie zmieniając wyniku jego działania. Ulepszeniem może być zebranie zduplikowanego kodu w funkcję, wyekstraktowanie części funkcjonalności do osobnych klas itp.

- __Test-driven development (TDD)__ - jest to technika tworzenia oprogramowania według której programista najpierw pisze kod testów automatycznych (czyli określa za ich pomocą jak aplikacja ma się zachowywać), a następnie pisze właściwy kod który sprawi, że testy napisane w kroku 1 będą przechodzić (zostanie napisana wymagana funkcjonalność). W 3 kroku opcjonalnie można dokonać refaktoryzacji kodu, tak aby testy wciąż przechodziły. Stąd TDD często określa się mottem 'red-green-refactor' (napisane testy nie przechodzą-testy przechodzą-refaktoryzacja).

- __zreprodokować (ang. reproduce) błąd__ - odtworzyć, potwórzyć błąd. Gdy zostanie zgłoszone błędne działanie aplikacji (np. przez testera/klienta/system przechwytujący wyjątki) i jesteśmy w stanie wykonać czynności (np. wybrać pozycję z menu i kliknąć przycisk), które spowodują wystąpienie błędu w naszym środowisku developerskim/na naszym koncie użytkownika na stage - mówimy że błąd da się zreprodukować.
