Wyświetl tabelę actors w kolejności alfabetycznej sortując po kolumnie surname.
** SELECT * FROM `actors` ORDER BY `surname` ASC

Wyświetl film, który powstał w 2019 roku.
** SELECT * FROM `movies` WHERE year_of_production=2019;

Wyświetl wszystkie filmy, które powstały między 1900, a 1999 rokiem.
** SELECT * FROM `movies` WHERE year_of_production>1900 and year_of_production<1999;

Wyświetl JEDYNIE tytuł i cenę filmów, które kosztują poniżej 7$
** SELECT title, price FROM `movies` WHERE price<7;

Użyj operatora logicznego AND, aby wyświetlić aktorów o actor_id pomiędzy 4-7 (4 i 7 powinny się wyświetlać). NIE UŻYWAJ operatora BETWEEN.
** SELECT * FROM `actors` WHERE actor_id>3 and actor_id<8

Wyświetl klientów o id 2,4,6 wykorzystaj do tego warunek logiczny.
** SELECT * FROM `customers` WHERE customer_id in ('2','4','6');

Wyświetl klientów o id 1,3,5 wykorzystaj do tego operator IN.
** SELECT * FROM `customers` WHERE customer_id in ('1','3','5');

Wyświetl dane wszystkich osób z tabeli ‘actors’, których imię zaczyna się od ciągu “An”.
** SELECT * FROM `actors` WHERE name LIKE 'An%';

Wyświetl dane klienta, który nie ma podanego adresu email.
** SELECT * FROM `customers` WHERE email is NULL;

Wyświetl wszystkie filmy, których cena wynosi powyżej 9$ oraz ich ID mieści się pomiędzy 2 i 8 movie_id.
** SELECT * FROM `movies` WHERE price>9 AND movie_id BETWEEN 2 and 8;
