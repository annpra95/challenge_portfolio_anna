# Wyświetl tabelę actors w kolejności alfabetycznej sortując po kolumnie surname.
* SELECT * FROM `actors` ORDER BY `surname` ASC

# Wyświetl film, który powstał w 2019 roku.
* SELECT * FROM `movies` WHERE year_of_production=2019;

# Wyświetl wszystkie filmy, które powstały między 1900, a 1999 rokiem.
* SELECT * FROM `movies` WHERE year_of_production>1900 and year_of_production<1999;

# Wyświetl JEDYNIE tytuł i cenę filmów, które kosztują poniżej 7$
* SELECT title, price FROM `movies` WHERE price<7;

# Użyj operatora logicznego AND, aby wyświetlić aktorów o actor_id pomiędzy 4-7 (4 i 7 powinny się wyświetlać). NIE UŻYWAJ operatora BETWEEN.
* SELECT * FROM `actors` WHERE actor_id>3 and actor_id<8

# Wyświetl klientów o id 2,4,6 wykorzystaj do tego warunek logiczny.
* SELECT * FROM `customers` WHERE customer_id in ('2','4','6');

# Wyświetl klientów o id 1,3,5 wykorzystaj do tego operator IN.
* SELECT * FROM `customers` WHERE customer_id in ('1','3','5');

# Wyświetl dane wszystkich osób z tabeli ‘actors’, których imię zaczyna się od ciągu “An”.
* SELECT * FROM `actors` WHERE name LIKE 'An%';

# Wyświetl dane klienta, który nie ma podanego adresu email.
* SELECT * FROM `customers` WHERE email is NULL;

# Wyświetl wszystkie filmy, których cena wynosi powyżej 9$ oraz ich ID mieści się pomiędzy 2 i 8 movie_id.
* SELECT * FROM `movies` WHERE price>9 AND movie_id BETWEEN 2 and 8;

# Popełniłam błąd wpisując nazwisko Ani Miler – wpisałam Muler. Znajdź i zastosuj funkcję, która poprawi mój karkołomny błąd 🙈


# Pobrałam za dużo pieniędzy od klienta, który kupił w ostatnim czasie film o id 4. Korzystając z funkcji join sprawdź, jak ma na imię klient i jakiego ma maila. W celu napisania mu wiadomości o pomyłce fantastycznej szefowej.


# Na pewno zauważył_ś, że sprzedawca zapomniał wpisać emaila klientce Patrycji. Uzupełnij ten brak wpisując: pati@mail.com


# Dla każdego zakupu wyświetl, imię i nazwisko klienta, który dokonał wypożyczenia oraz tytuł wypożyczonego filmu. (wykorzystaj do tego funkcję inner join, zastanów się wcześniej, które tabele Ci się przydadzą do wykonania ćwiczenia).


# W celu anonimizacji danych, chcesz stworzyć pseudonimy swoich klientów. - Dodaj kolumnę o nazwie ‘pseudonym’ do tabeli customer,- Wypełnij kolumnę w taki sposób, aby pseudonim stworzył się z dwóch pierwszych liter imienia i ostatniej litery nazwiska. Np. Natalie Pilling → Nag


# Wyświetl tytuły filmów, które zostały zakupione, wyświetl tabelę w taki sposób, aby tytuły się nie powtarzały.


# Wyświetl wspólną listę imion wszystkich aktorów i klientów, a wynik uporządkuj alfabetycznie. (Wykorzystaj do tego funkcji UNION)
SELECT name from actors union name from customers

# Polskę opanowała inflacja i nasz sklepik z filmami również dotknął ten problem. Podnieś cenę wszystkich filmów wyprodukowanych po 2000 roku o 2,5 $ (Pamiętaj, że dolar to domyślna jednostka- nie używaj jej nigdzie).


# Wyświetl imię i nazwisko aktora o id 4 i tytuł filmu, w którym zagrał


# A gdzie nasza HONIA!? Dodaj do tabeli customers nową krotkę, gdzie customer_id = 7, name = Honia, surname = Stuczka-Kucharska, email = honia@mail.com oraz pseudonym = Hoa
* INSERT INTO customers (customer_id, name, surname, email) VALUES ("7", "Honia", "Stuczka-Kucharska", "honia@mail.com");
