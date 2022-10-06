KÄYTTÖ:
myapi
npm start
käynnistä Qt sovellus




TIETOKANTA:

CREATE DATABASE netdb;
CREATE USER 'netuser'@'localhost' IDENTIFIED WITH mysql_native_password BY 'netpass';
GRANT ALL on netdb.* to 'netuser'@'localhost';

USE netdb;

CREATE TABLE book(
id_book INT primary key auto_increment,
name VARCHAR(255),
author VARCHAR(255),
isbn VARCHAR(20)
);

INSERT INTO book(name,author,isbn) VALUES('PHP Basic','Bob Jones','123-456-789-111-x');
INSERT INTO book(name,author,isbn) VALUES('Statistics','Lisa Smith','222-333-444-555-y');

CREATE TABLE car (
  id_car INT primary key auto_increment,
  brand varchar(255),
  model varchar(255) 
);

INSERT INTO car(brand,model) VALUES('Ford', 'Mustang');
INSERT INTO car(brand,model) VALUES('Delorean', 'DMC-12');
INSERT INTO car(brand,model) VALUES('Dodge', 'Charger');
INSERT INTO car(brand,model) VALUES('Ferrari', 'Testarossa');
INSERT INTO car(brand,model) VALUES('Toyota', 'Supra');
INSERT INTO car(brand,model) VALUES('Datsun', 'Cherry');
INSERT INTO car(brand,model) VALUES('Chevrolet', 'Caprice');