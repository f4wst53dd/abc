# Linux

Jedną z ważniejszych umiejętności które według mnie powinien opanować każdy programista/web developer jest znajomość systemu Linux, co najmniej w stopniu przynajmniej podstawowym. Nawet jeśli swoje środowisko developerskie stworzyłeś pod kontrolą innego systemu, np. Windows, to istnieje duża szansa, że umiejętności podstaw obsługi systemu uniksopodobnego kiedyś przydadzą ci się. Przykładowo wersja stage lub produkcyjna aplikacji którą tworzysz w firmie będzie zdeployowana na maszynie z [Debianem](https://www.debian.org/), [Ubuntu](https://www.ubuntu.com/) czy [CentOS](https://www.centos.org/). Możesz zostać poproszony o wyciągnięcie logów aplikacji, zainstalowanie nowego narzędzia na tym serwerze itp. Wtedy nawet niezbyt zaawansowana wiedza nt. poruszania się w 'terminalowym' systemie linuksowym (bez środowiska graficznego) będzie na wagę złota.

Dodatkowo, możesz w firmie otrzymać komputer ze takim systemem, lub z [macOS](https://en.wikipedia.org/wiki/MacOS), który również jest oparty na jądrze Linuxa, i ma terminal, który ma taką powłokę jak linux (bash).

## Zalety używania Linuxa jako platformy do programowania

Linux uczy minimalizmu, prostoty. Filozofię architektury Linuxa można streścić tak: 'uniwesalny, wyizolowany, mały program do rozwiązywania danego problemu, a rezultat jego działania można bezpośrednio użyć jako wejście (input) do innego programu (potokowanie/piping)'. Takie podejście w większym lub mniejszym stopniu będzie bardzo wskazane przy pisaniu oprogramowania. Modularność, czyli rozbicie dużego programu na szereg mniejszych części (modułów), tak, aby zachować przejrzystość w kodzie, a raz napisany moduł móc wykorzystać w tej samej aplikacji, albo w innym projekcie jest powszechna, często przytaczana jako poprawna technika.

Oprócz 'administracyjnych' czynności (typu tworzenie katalogów, obserwowanie procesów etc.) konsola Linuxa stanowi często wygodniejsze, szybsze środowisko uruchomienia kluczowych przy developmencie programów. Doskonałym przykładem jest [git](https://git-scm.com/), rozproszony system kontroli wersji oprogramowania. Istnieją GUI (interfejsy graficzne) dla gita, jednak w znakomitej większości przypadków użycie gita z poziomu konsoli (CLI) będzie szybsze i wygodniejsze.

## Przykłady najważniejszych poleceń w konsoli

- wyświetlanie zawartości katalogów (ls), przemieszczanie się między nimi (cd)
- tworzenie, usuwanie, zmiana nazwy, przenoszenie, kopiowanie plików i katalogów (mkdir, rmdir, rm, mv, cp)
- zmiana uprawnień, grupy, właściciela plików i folderów (chmod, chgrp, chown)
- badanie czasu wykonania programu (time)
- zmiana daty ostatniej modyfikacji pliku/utworzenie nowego, pustego pliku (touch)
- wyszukiwanie plików (find)
- tworzenie dowiązań do plików (ln)
- wyświetlenie, dodawanie/usuwanie wpisów zmiennych środowiskowych (environment variables) np. $PATH (export, printenv)
- używanie potoków do przekazywania danych (operator: '|' )
- wyświetlenie wolnego miejsca na dysku (partycji) oraz ile danych zawiera dany katalog (df, du)
- wyświetlenie zawartości plików (cat, less, tail, tailf), grepowanie (grep)
- wyświetlenie statystyk użycia zasobów systemu przez poszczególne procesy (top, htop); ogólne statystyki użycia RAM (free)
- wyświetlenie listy procesów, ich ubijanie (ps, pgrep, kill, pkill, killall); przenoszenie ich w tło/na pierwszy plan (fg, bg)
- polecenia sieciowe (ping), wyświetlanie konfiguracji sieci (ifconfig, iwconfig)
- komunikacja z zewnętrznym serwerem (ssh, scp)
- montowanie systemu plików, sprawdzenie i naprawa jego błędów (mount, fsck)
- narzędzia pobierania danych (curl, wget)
- instalacja paczek oprogramowania, kompilacja programów (apt-get lub jego odpowiednik, make)
- skróty klawiaturowe, zwł. Ctrl+R (wyszukiwanie w historii konsoli), Ctrl+A, Ctrl+E (przeniesienie kursora na początek i koniec linii), Tab (autouzupełnienie nazw), Ctrl+C, Ctrl+Z (zamknięcie i zawieszenie bieżącego programu)

## Skąd czerpać wiedzę?

Gdzie szukać informacji na temat tych zagadnień? Jest dużo materiałów w Internecie, są też książki, często opasłe, kilkuset stronnicowe tomiska, opisujące szczegółowo praktycznie każde podstawowe polecenie, łącznie z ich licznymi opcjami i przełącznikami. Początkujących mogą one odstraszyć, ponieważ najważniejsze punkty giną w lawinie mało istotnych informacji. Lepiej zabrać się za krótszą, bardziej zwięzłą książkę, taką jak ['Introduction to the Command Line (Second Edition): The Fat Free Guide to Unix and Linux Commands' Nicolasa Marsha](https://www.amazon.com/Introduction-Command-Line-Second-Commands/dp/1450588301).

Dodatkowo, warto zapoznać się z poniższymi linkami, gdzie przytoczono sporo skrótów, sztuczek i technik, dzięki którym usprawnimy naszą pracę w linuxowym terminalu:

- [http://www.commandlinefu.com/commands/browse/sort-by-votes](http://www.commandlinefu.com/commands/browse/sort-by-votes)
- [http://stackoverflow.com/questions/68372/what-is-your-single-most-favorite-command-line-trick-using-bash](http://stackoverflow.com/questions/68372/what-is-your-single-most-favorite-command-line-trick-using-bash)
- [http://mylinuxbook.com/20-interesting-and-extremely-helpful-linux-command-line-tricks/](http://mylinuxbook.com/20-interesting-and-extremely-helpful-linux-command-line-tricks/)
- [https://github.com/jlevy/the-art-of-command-line](https://github.com/jlevy/the-art-of-command-line)

## Jak 'nauczyć się' Linuxa?

W jaki sposób przyswoić sobie powyższą wiedzę? Jest kilka sposobów. Możesz otworzyć książkę czy jakąś stronę w Internecie, poczytać, i na tym zakończyć edukację. Takie 'uczenie się' nie sprawdza się prawie nigdy, w przeciwieństwie do nauki przy wykorzystaniu wiedzy w praktyce. Dlatego lepszym pomysłem będzie instalacja tego systemu.

Zrozumiałe są opory i obawy przed instalacją Linuxa na moim komputerze, obok instancji Windows. Raz - że proces wyodrębnienia kolejnej partycji i instalacja na niej innego systemu nie jest prosta; dwa - istnieje szansa, że posypie się coś w sektorach rozruchowych, i padną obydwa systemy. Można oczywiście zapoznawać się z Linuxem bez jego instalacji (np. [Cygwin](https://www.cygwin.com/), wersja live CD, wirtualizacja [VirtualBoxem](https://www.virtualbox.org/)), jednak każdy z tych sposobów jest protezą. Jeśli chcesz wejść w Linuxa na serio - a tak zakładam, to powinieneś się w nim zanurzyć. Całkowite zanurzenie (total immersion) jest koncept znany z nauki języków obcych. Polega w największym skrócie na całkowitym otoczeniu się danym językiem (obóz językowy, czytanie gazet i słuchanie radia - nawet bez zrozumienia przekazu). Podobnie w przypadku chęci nauki tego systemu: powinieneś zainstalować go i używać jako główny, podstawowy OS.

Jeśli posiadasz umiejętności obsługi komputera powyżej przeciętnej powinieneś poradzić sobie z zainstalowaniem tego systemu. Jeśli wciąż masz wątpliwości, możesz obejrzeć proces instalacji na [youtube](https://www.youtube.com/). Możesz popytać wśród znajomych czy ktoś może instalował taki system, i poprosić o asystę.

## Jaką dystrybucję Linuksa zainstalować?

Istnieje bardzo dużo różnych dystrybucji Linuksa. Zakładając, że poszukujesz systemu dla początkujących to najlepszym wyborem może być [Ubuntu](https://www.ubuntu.com/), [Mint](https://www.linuxmint.com/), [Fedora](https://getfedora.org/) czy [CentOS](https://www.centos.org/). Jednocześnie dystrybucje takie jak [Arch Linux](https://www.archlinux.org/), [Gentoo](https://www.gentoo.org/) czy [Slackware](http://www.slackware.com/) są trudniejsze w instalacji, modyfikacji i często w codziennym użytkowaniu, dlatego początkujący powinni ich unikać.
