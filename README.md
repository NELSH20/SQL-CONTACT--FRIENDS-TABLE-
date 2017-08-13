# SQL-CONTACT--FRIENDS-TABLE-
/*Basic table testing my new acquire SQL skill in organizing a table */ 


CREATE TABLE friends (id INTEGER, name TEXT, birthday TEXT);
INSERT INTO friends (name, birthday) VALUES ('Jane Doe', 'May 19th, 1993');
/* INSERTANDO A LOS TRES AMIGOS AQUI */
INSERT INTO friends (name, birthday) VALUES ('Paul Erison', 'August 11th, 1995');
INSERT INTO friends (name, birthday) VALUES ('Eric Erison', 'September 8th 1999');
INSERT INTO friends (name, birthday ) VALUES ('Einstein Peterson', 'October 10 1981');
/*UPDATE OF Jane marriage*/
UPDATE friends Set name = 'Jane Smith' WHERE name = 'Jane Doe';
/*ALTER AND ADDING THE EMAILS*/
ALTER TABLE friends ADD email TEXT;
UPDATE friends SET email = 'jdoe@example.com' WHERE name = 'Jane Smith';
UPDATE friends SET email = 'jonas@brother.com' WHERE name = 'Paul Erison';
UPDATE friends SET email = 'Eric@eric.com' WHERE name = 'Eric Erison';
UPDATE friends SET email = 'Ein@hotmail.com'
WHERE name = 'Einstein Peterson';
/*DISPLAYING THE TABLE*/
SELECT * FROM friends;
/*REMOVE JANE */
DELETE FROM friends WHERE name = 'Jane Doe';
