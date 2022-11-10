# Primary Key Foreign Key

CREATE TABLE book(
	id SERIAL PRIMARY KEY,
	title VARCHAR(150) NOT NULL,
	pageNumber INTEGER NOT NULL,
	publicationYear DATE,
	author_id INTEGER REFERENCES author(id)
);
insert into author(firstName,lastName,email,birthday) VALUES('Billy','Gates','aaa@bbb.de','2002-02-02');
insert into author(firstName,lastName,email,birthday) VALUES('James','Booker','a2aa@bbb.de','2002-02-02');
insert into author(firstName,lastName,email,birthday) VALUES('Mike','Saler','aa3a@bbb.de','2002-02-02');
insert into author(firstName,lastName,email,birthday) VALUES('Hans','Gate','aa5a@bbb.de','2002-02-02');
insert into author(firstName,lastName,email,birthday) VALUES('Carlos','Dummy','a6aa@bbb.de','2002-02-02');


insert into book(title, pageNumber, publicationYear,author_id) VALUES ('Seven',123,'2003-01-01',1);
insert into book(title, pageNumber, publicationYear,author_id) VALUES ('Kriminalität',123,'2001-01-01',2);
insert into book(title, pageNumber, publicationYear,author_id) VALUES ('Black Rose',1123,'2003-01-01',3);
insert into book(title, pageNumber, publicationYear,author_id) VALUES ('Tom and Jerry',123,'2002-01-01',4);
insert into book(title, pageNumber, publicationYear,author_id) VALUES ('Red Kid',123,'2003-01-01',5);
insert into book(title, pageNumber, publicationYear,author_id) VALUES ('Billy the Kid',123,'2012-01-01',6);
insert into book(title, pageNumber, publicationYear,author_id) VALUES ('Social Media attackers',123,'2019-01-01',7);


select * from book;