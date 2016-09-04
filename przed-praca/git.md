# Git

Jednym z najważniejszych, najbardziej podstawowym narzędziem które wykorzystuje w codziennej pracy każdy programista jest system kontroli wersji (VCS, Version Control System). Pozwala on na bardzo wygodne zarządzanie historią projektu. Developer zamiast wykonywać kopie zapasowe kodu całej aplikacji lub pojedynczych plików powinien użyć do tego celu system kontroli wersji.

Metoda backupowania staje się bardzo uciążliwa, zwłaszcza "badając teren", wypróbowując różne rozwiązania. Przykład: myślę, że przydałoby się dodać mechanizm cachowania. Na ok. 80% przewiduję, że jakiś będzie wdrożony. Są dwie popularne i polecane biblioteki, które oferują taki mechanizm, ale nie wiem, która z nich będzie lepsza. Może pierwsza z której skorzystamy będzie ok, i nie trzeba będzie przenosić się na drugą, ale nie jest to pewne. VCS oferuje doskonałe rozwiązanie dla tego problemu - użycie gałęzi (ang. 'branch').

Najpopularniejszym takim systemem jest Git.

Istnieje sporo systemów kontroli wersji. Git na tle konkurencji wyróżnia się popularnością i uniwersalnością. Jest wykorzystywany przy ogromnych projektach, takich jak wersjonowanie jądra (kernela) Linuxa, jak i średnich/małych. Również ten post jest utrzymywany w gicie, ponieważ system ten doskonale nadaje się do przechowywania zmian dowolnych plików tekstowych, nie tylko plików ze kodem źródłowym. Git radzi sobie też nie gorzej z dowolnym plikiem binarnym, zatem można w repozytorium można umieścić dowolny plik (obrazek, plik mp3 itp.), chociaż tego typu pliki zwykle powinny być umieszczane poza VCSem, np. na Amazon S3.

Git jest bardzo szybki. Praktycznie każda operacja, którą wykonujemy z jego użyciem jest wykonywana tak szybko, że jest to niemal niezauważalne. Posiada wygodne narzędzia (np. stash, bisect), możliwość wyszukiwania w historii i wprowadzenia w niej zmian (choćby zmiana nazwy dowolnego commita).

## Jak działa Git

W Gicie tymczasowe, próbne miejsca, w których możemy rozwijać kod w niezależnie od reszty są nazywane branchami (gałęziami), ponieważ przypominają one strukturę drzewa. Tak jak gałąź drzewa może posiadać n innych odgałęzień (które również mogą posiadać kolejne odgałęzienia od swojego przebiegu), tak i w Gicie można łatwo wyjść z dowolnego punktu historii, i działać (np. pisząc kod nowej funkcjonalności) na odrębnej od reszty "ścieżce". Jednym poleceniem możemy przełączyć się na dowolny inny branch (polecenie ‘git checkout’). Od nas zależy, co zrobimy ze zmianami na takim osobnym branchu. Czy zachowamy je, czy całkiem porzucimy, usuwając tą gałąź. W przypadku chęci zachowania możemy te zmiany dołączyć do ‘głównego’ (a nawet dowolnego innego) brancha (taka operacja nazywa się "merge"), albo zostawić je na tym branchu, w swoistym miejscu osamotnienia, przykładowo po to, aby kiedyś być może powrócić do rozwijania idei która przyświecała temu rozgałęzieniu.

Analogią do wspomnianego powyżej robienia ręcznych backupów (zipów) z poszczególnych etapów tworzenia aplikacji jest w Gicie robienie commitów. Jest to tworzenie 'migawek', czyli zapisanie porcyjki zmian w pojedynczej "skrzyneczce". Z automatu dopisywane są takie informacje jak dokładna data wykonania tego zapisu, oraz kto wykonał commit. Naszym zadaniem jest jedynie napisanie krótkiego komunikatu, który będzie dobrze opisywał co ta porcja zmian wprowadziła/zmieniła/usunęła. Na temat pisania dobrych komunikatów commitów można poczytać lub tu albo tu . Przykładami mogą być: 'Change color and size of login button’, lub ‘Add authentication via facebook'. Dobrze napisane komunikaty commitów pozwalają na bardzo szybkie przeglądanie historii i orientowanie się, kiedy dane zmiany zostały wprowadzone.

Git spełnia również rolę backupową. Zazwyczaj programista posiada na swoim komputerze (lub na innym serwerze) lokalną kopię całego repozytorium. Wprowadza na nim zmiany na własnych branchach. Gdy uzna, że chce z tymi modyfikacjami podzielić się z innymi programistami (lub po prostu chce je wprowadzić do kodu) wysyła te zmiany na osobny serwer, gdzie przechowywane jest repozytorium. Odpowiada za to polecenie ‘git push’. Nie trzeba samemu stawiać takiego serwera gita, można wykorzystać darmowe konto na Githubie, Bitbuckecie i in. Przechowując kopię repozytorium na takim serwerze mamy wtedy klasyczny, wygodny backup danych projektu, umieszczonych poza urządzeniem, na którym pracujemy. Gdy padnie nam dysk twardy, ktoś nam ukradnie laptopa nie stracimy efektów miesięcy, a często lat pracy. Każdy z programistów pracujących przy projekcie ma własną kopię całości kodu (wraz z całą jego historią!) co składa się na solidny, wielokrotny backup.

## Jak nauczyć się Gita?

Dróg jest wiele, gdyż powstało sporo książek na temat Gita. Nie brakuje też wideo-kursów i artykułów na różnych stronach internetowych przedstawiających zarówno podstawy jak i bardziej zaawansowane zagadnienia. Bardzo dobrą pozycją jest książka 'Pro Git', która jest dostępna za darmo na stronie domowej Gita. Zawiera ona bardzo przystępnie opisane wszystkie najważniejsze aspekty tego systemu. Oprócz pokazywania jak korzystać za poszczególnych jego poleceń ta książka kładzie także nacisk na zrozumienie tego, jak Git działa, a to jest bardzo ważne, żeby swobodnie z nim pracować. Przeczytanie tej jednej pozycji wystarczy do wejścia w świat Gita.

Warto również założyć konto na Githubie lub Bitbuckecie. W drugim można utworzyć darmowe, prywatne repozytorium. Z kolei na Githubie repozytoria są darmowe, ale muszą być wtedy publicznie dostępne. Bardzo ułatwia życie wykorzystanie kluczy SSH do uwierzytelniania się, dzięki czemu nie będziemy musieli wpisywać za każdym razem hasła do swojego konta przy pobieraniu (fetchowaniu) bieżącej wersji kodu lub przy wysyłaniu zmian (pushowaniu).

Niezmiernie ważną rzeczą w nauce jakiejkolwiek technologii jest używanie jej w praktyce. Nie inaczej jest z Gitem. Używając gita przy własnym, indywidualnym projekcie nie natkniemy się na wiele ważnych zagadnień. Przykładowo, fetchowanie nie ma zbytnio sensu, skoro kodu nikt inny nie mógł zmodyfikować. Rozwiązywanie konfliktów mergowania - gdy pracujesz w pojedynkę i nie tworzysz jednocześnie kilku branchów to jest szansa, że nie będziesz miał z tego wiedzy praktycznej. Jak zapobiec takim sytuacjom? Musisz tworzyć przynajmniej 1 projekt z kimś jeszcze. Jeśli nie masz żadnego znajomego programisty znajdź na githubie jakiś projekt. Najlepiej taki, który przyda ci się kiedyś, oraz który jest pisany w języku który znasz. Przeglądnij listę issues/bugów i napraw któryś błąd. Możesz również dodać potrzebną funkcjonalność lub wykonać refactoring. Najlepiej byłoby jednak, gdybyś współpracował z innymi programistami w pracy.