# Bazy danych

Wiedza z zakresu baz danych jest bardzo istotna w web developmencie. I o ile frontend developer nie musi jej posiadać, to w przypadku backend-, czy full-stack developera jest to konieczność. Jest to tematyka na tyle rozległa, że istnieją specjalizacje w tym kierunku (administrator baz danych). W przypadku web developera nie musimy mieć bardzo szerokiej wiedzy z baz. Zwykle wystarczy znać podstawy projektowania baz danych, zapytań i optymalizacji.

## Jaką bazę danych wybrać?

Po pierwsze musisz zdecydować jaki typ bazy będziesz używał. Najpowszechniejsze są bazy relacyjne, a istnieją one już od wielu lat. Charakteryzują się one ustaloną strukturą, w przybliżeniu odpowiadającą tabeli (w kolumnami są atrybuty, np. 'nazwisko' i 'wiek', a w wierszach wartości atrybutów, np. 'Nowak', 23). Ostatnimi laty coraz większą popularnością cieszą się bazy nierelacyjne (NoSQL). Wśród nich wyróżnia się bazy przechowujące dane w dokumentach, w parach klucz-wartość, w postaci grafu i inne. Przykładami bazy NoSQL są MongoDB, Redis czy Neo4j. Posiadanie wiedzy z baz NoSQL może być dużym plusem, jednak poznanie modelu relacyjnego baz danych jest niemal koniecznością, dlatego właśnie na nim warto skupić uwagę na początku nauki web developmentu.

Którą spośród baz relacyjnych warto opanować? Dużymi graczami na rynku tego typu baz są m.in.: Oracle Database, MySQL, Microsoft SQL Server czy PostgreSQL. Oracle i Microsoft oferują darmowe wersje baz, ale są one bardzo mocno ograniczone, np. ilością danych na jedną instancję bazy. PostgreSQL oferuje więcej funkcjonalności niż MySQL, oraz jest tworzona całkowicie w duchu Open Source. MySQL został przejęty przez firmę Oracle, wprowadzając dodatkowe płatne wersje. Podsumowując: biorąc pod uwagę popularność, darmowość i możliwości bazy danych najlepszym wyborem jest prawdopodobnie PostgreSQL, a w drugiej kolejności MySQL (lub jego całkowicie otwarty fork o nazwie MariaDB).

Istnieje wiele bibliotek ORM (mapowanie obiektowo-relacyjnego). Pozwalają one 'ukryć' zapytania SQL wykorzystując obiekty języka programowania w jakim dany ORM został napisany. W zamyśle ORMy miały ułatwić pisanie zapytań do bazy, jednak istnieje szereg problemów z nimi związanymi. Przykładem tych niedogodności może być wolniejsze działanie (spowodowane przykładowo tworzeniem obiektów przy każdym zapytaniu), trudność (a czasem całkowita niemożność) napisania bardziej skomplikowanych zapytań w ORM, np. joinów wielu tabel, procedur składowych itp. Biorąc pod uwagę te czynniki błędem jest myślenie, że wystarczy opanować jakiś ORM, całkowicie ignorując SQL.

## Umiejętności z baz danych

- tworzenie, usuwanie tabel (CREATE TABLE, DROP TABLE)
- typy danych (INTEGER, TEXT, SERIAL itp.)
- wartość domyślna (DEFAULT), constraints (NOT NULL, UNIQE)
- klucz główny (PRIMARY KEY), klucz obcy (FOREIGN KEY, REFERENCES)
- modyfikacja tabel (ALTER TABLE): usuwanie, usuwanie kolumn (ADD COLUMN, DROP COLUMN); więzy spójności danych (ADD CHECK, ADD CONSTRAINT, DROP CONSTRAINT); zmiana wartości domyślnej kolumny (ALTER COLUMN .. SET DEFAULT, DROP DEFAULT); zmiana nazwy tabeli, kolumny (RENAME TO)
- praca ze schemami (CREATE/DROP/SHOW SCHEMA, SET search_path TO)
- wybieranie wartości z tabeli z opcjonalnymi warunkami (SELECT .. FROM .. WHERE)
- wybieranie wartości z wielu tabel (SELECT .. FROM .. JOIN .. ON .. WHERE);
- agregacje (zliczanie rekordów COUNT, suma SUM, wartość maksymalna/minimalna MAX/MIN, średnia AVG); agregacje b. często wykorzystują konstrukcję GROUP BY
- zapytania zagnieżdżone (jeden SELECT wewnątrz drugiego)
- aktualizacja rekordów (UPDATE .. SET)
- usuwanie rekordów (DELETE FROM)
- dodawnie rekordów (INSERT INTO .. VALUES)
- używanie indeksów (CREATE INDEX .. ON, DROP INDEX); wiedza kiedy stosować indeksy, i jaki ich rodzaj
- podstawy projektowania baz danych (podział danych na tabele, podział na kolumny tabel i wybór ich typów, tworzenie kluczów głównych, tworzenie kluczów obcych czyli relacji między tabelami, normalizacja bazy)
- transakcje, widoki
- programowanie bazy (triggery, funkcje, stored procedures)
