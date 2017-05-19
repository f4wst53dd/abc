## Jak znaleźć przyczynę błędu aplikacji?

Ogólne:

- czy nie zostały użyte słowa zarezerwowane (reserved words) języka programowania, biblioteki, bazy danych? Możemy znaleźć taką listę wyszukując w Internecie frazę '<technologia> reserved words'. Ostatecznie można spróbować użyć innej zazwy.
- czy nie naruszamy automatycznie wygenerowanych przez język metod/funkcji? Przykładowo definiując asocjację między modelami we frameworku Ruby on Rails automatycznie dostajamy sporo dodatkowych metod . Będąc nieuważnym możemy np. błędnie nadpisać te automatyczne metody. Rozwiązaniem problemu jest jak najszersza wiedza nt. jak działa i co robi dany język, framework, biblioteka. Doraźnie warto spróbować zmienić nazwy nowoutworzonych metod/funkcji, co potencjalnie pozwoli uniknąć konfliktu nazw.
- czy przypadkowo nie zostały wprowadzone do pliku z kodem niewłaściwe znaki, np. znak spacji niełamięcej (non-breaking space) zamiast zwykłej spacji. Metodą na sprawdzenie kodu pod tym kątem może być ręczne przepisanie problematycznej linii kodu (zamiast kopiowania jej z innego źródła) lub podgląd pliku kodu źródłowego w edytorze heksadecymalnym (wtedy wartość znaku będzie inna od tej oczekiwanej).

Po stronie przeglądarki

- błędy/ostrzeżenia w konsoli JavaScript przeglądarki (dostępna w zakładce 'Console' po otwarciu narzędzi programistycznych 'Developer Tools' - w Chrome/Firefox można otworzyć je skrótem CTRL+SHIFT+I lub F12). Trzeba pamiętać, że nie każdy błąd/ostrzeżenie powoduje błędne działanie aplikacji oraz to, że obecne błędy w konsoli mogły być obecne już od dłuższego czasu (jeśli nikt je nie usunął), i niekoniecznie mają one wpływ na buga którego staramy się poprawić.

- requesty w konsoli przeglądarki (zakładka 'Network'): czy oczekiwany request pojawił się na liście? Czy nagłówki i parametry żądania/odpowiedzi są prawidłowe; czy żądanie nadeszło z odpowiedniego URL; czy przeglądarka otrzymała odpowiedź na żądanie.
- debugowanie kodu JS
- analiza struktury HTML strony
- przeładowanie strony bez cache, tzw. 'hard reload' (skrót CTRL+SHIFT+R w Chrome/Firefox); jednoczesne wyczyszczenie cache i przeładowanie strony bez cache (po otwarciu narzędzi programistycznych - np. skrótem F12 - naciskamy prawym przyciskiem myszy ikonę odświeżenia strony i wybiermy opcję 'Empty Cache and Hard Reload'. Możemy też przytrzymać wciśnięty lewy przycisk myszy.). Pierwsza metoda wymusi ściągnięcie każdego zasobu (pliku CSS, JS, obrazka itp.) odwiedzanej strony; innymi słowy zignoruje przechowywane dane w cache przeglądarki. Druga zaś zamiast zignorować cache wyczyści go całkowicie, dzięki czemu będziemy pewni, że przeglądarka nie odczyta z cache zasobów które zostały pobrane po fazie ładowania strony.

- analiza zawartości ciasteczek przeglądarki (ang. 'cookies') i ich edycja (za pomocą wbudowanych narzędzi przeglądarki lub wtyczki do obsługi cookies). Jeśli kod aplikacji zapisuje i odczytuje pewne dane w ciasteczkach może wystąpić szereg błędów związanych z ich obsługą. Błąd w aplikacji może być spowodowany przez ustawianie/usuwanie ciastka w niewłaściwym miejscu (np. za wcześnie, za późno). Wartość przypisana do cookie może być nieprawidłowa. Mogą występować także problemy z przypisaną do nich wartością wygasania (ang. 'Expires'), czy też ich domeną (np. gdy zmieniliśmy adres aplikacji w środowisku developerskim to ciastka ustawione na poprzednim adresie nie będą wykorzystywane).

- czy wtyczki użyte w przeglądarce nie zablokowały jakichś elementów strony? Dotyczy to zwłasza rozszerzeń przeglądarek blokujących reklamy (np. uBlock Origin, Adblock Plus), wyłączające śledzenie (tracking) na stronach (np. Ghostery, Disconnect), wyłączające JS (np. NoScript). Dodatkowo wraz z zablokowanym elementem może pojawić się błąd w konsoli JavaScript przeglądarki, np.: 'Failed to load resource: net::ERR_BLOCKED_BY_CLIENT'.

- czy aplikacja działa pod inną przeglądarką? Czasami mogą wystąpić różnice w wyświetlaniu zawartości strony między różnymi przeglądarkami. Różnice te są spowodowane odmiennym interpretowaniem niektórych reguł arkuszy stylów (CSS) oraz elementów języka JavaScript. W przypadku współczesnych przeglądarek takie problemy są rzadsze niż było to dawniej, ale nie mniej jednak warto czasem sprawdzić, czy błąd występujący na stronie otwartej w np. Firefoksie jest obecny również w Chromie.

Po stronie serwera
- analiza logów - czy w logach serwera, frameworka lub innego wykorzystywanego przez nas programu nie ma informacji wskazujących na błąd (np. obecność fraz 'Error', 'Exception', 'Fatal' itp.)? Warto również zwrócić uwagę na ostrzeżenia ('Warning') - czasem aplikacja jedynie umieści w logu ostrzeżenie i będzie kontynuować działanie.
- https
-


front:

- zduplikowane id
- zagnieżdżone formularze
- self-closing tags
- wymagane atrybuty alt, ahref

emaile HTML:
- czy wykorzystujemy style inline (style dodawane do elementów HTML przez atrybut 'style')? Inne metody dodawania stylów, typu element 'link' czy umieszczenie stylów w sekcji 'head' są często niewspierane przez aplikacje pocztowe czy poczty www.
- czy używamy skomplikowanych stylów CSS/struktur HTML? Generalnie im prostszy kod emaila HTML tym jest mniejsza szansa na błędy. Warto wykorzystywać CSS 2.1 zamiast nowszego standardu CSS 3; również znaczniki HTML powinny być jak najprostsze. W przypadku wystąpienia błędów z CSS/HTML dobrym pomysłem jest rozpoczęcie od najprostszej struktury emaila i stopniowe dodawanie kolejnych elementów HTML/CSS i sprawdzanie czy email wyświetla się poprawnie.
- czy używamy ścieżek bezwzględnych? W odróżnieniu od zwykłej strony www nie możemy używać ścieżek względnych w odnośnikach do stron www, w atrybucie 'src' obrazków itp. Czyli zamiast '/subpage.html' trzeba użyć 'http://www.example.com/subpage.html'.
