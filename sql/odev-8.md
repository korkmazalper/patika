## SQL - Odev 8
1. test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
```sql
CREATE DATABASE TEST;
CREATE TABLE employee(
    ID SERIAL PRIMARY KEY,
    name VARCHAR(50),
    birthday DATE,
    email VARCHAR(100)
);
```


2. Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.
```sql
insert into employee (name, birthday, email) values ('Florinda', '1994-10-13', 'frichichi0@1688.com');
insert into employee (name, birthday, email) values ('Romola', '1982-02-28', 'rmixon1@goo.gl');
insert into employee (name, birthday, email) values ('Darcy', '1994-07-15', 'dmargeram2@youtu.be');
insert into employee (name, birthday, email) values ('Dot', '2000-09-17', 'dshilvock3@delicious.com');
insert into employee (name, birthday, email) values ('Ellissa', '1989-08-03', 'ehazeldine4@ihg.com');
insert into employee (name, birthday, email) values ('Charline', '1992-11-03', 'cclears5@yellowpages.com');
insert into employee (name, birthday, email) values ('Silvana', '2001-09-19', 'sjoburn6@newyorker.com');
insert into employee (name, birthday, email) values ('Suzanna', '1997-05-05', 'slatek7@msu.edu');
insert into employee (name, birthday, email) values ('Horatio', '2002-06-19', 'hkinrade8@google.co.uk');
insert into employee (name, birthday, email) values ('Veronika', '1998-12-31', 'vmandrey9@rediff.com');
insert into employee (name, birthday, email) values ('Allyn', '1985-09-22', 'alengthorna@jalbum.net');
insert into employee (name, birthday, email) values ('Adrianna', '1993-01-07', 'acrowcroftb@vistaprint.com');
insert into employee (name, birthday, email) values ('Nicholle', '2002-03-03', 'nbrymnerc@yahoo.co.jp');
insert into employee (name, birthday, email) values ('Germayne', '2001-10-18', 'gcoalesd@desdev.cn');
insert into employee (name, birthday, email) values ('Magdalen', '2004-03-24', 'mdrinkhille@deviantart.com');
insert into employee (name, birthday, email) values ('Pancho', '1985-08-24', 'pdawtreyf@slate.com');
insert into employee (name, birthday, email) values ('Camel', '2004-08-20', 'coakeshottg@themeforest.net');
insert into employee (name, birthday, email) values ('Alick', '2000-06-19', 'awormellh@mac.com');
insert into employee (name, birthday, email) values ('Franny', '2002-07-10', 'fmctrustami@biglobe.ne.jp');
insert into employee (name, birthday, email) values ('Boycie', '1991-09-09', 'bnorthwoodj@tripadvisor.com');
insert into employee (name, birthday, email) values ('Ring', '1997-05-13', 'rcotesk@independent.co.uk');
insert into employee (name, birthday, email) values ('Barbabra', '2001-03-16', 'beyrll@qq.com');
insert into employee (name, birthday, email) values ('Elene', '1997-05-01', 'ekohenm@wikimedia.org');
insert into employee (name, birthday, email) values ('Addie', '1983-11-08', 'aatweln@springer.com');
insert into employee (name, birthday, email) values ('Deirdre', '2004-08-02', 'dskurrayo@multiply.com');
insert into employee (name, birthday, email) values ('Harrie', '2003-02-05', 'hstillertp@cbc.ca');
insert into employee (name, birthday, email) values ('Packston', '2003-11-28', 'ppelchatq@4shared.com');
insert into employee (name, birthday, email) values ('Lise', '2003-08-26', 'lhyder@dion.ne.jp');
insert into employee (name, birthday, email) values ('Estella', '2002-11-30', 'ecartmels@dailymail.co.uk');
insert into employee (name, birthday, email) values ('Dory', '1983-05-31', 'dwickardtt@meetup.com');
insert into employee (name, birthday, email) values ('Bren', '1991-09-11', 'bburtonshawu@cpanel.net');
insert into employee (name, birthday, email) values ('Terrye', '1991-01-14', 'ttipplerv@github.com');
insert into employee (name, birthday, email) values ('Uriah', '1998-05-10', 'uchastenetw@economist.com');
insert into employee (name, birthday, email) values ('Dulciana', '1982-08-10', 'dnewittx@examiner.com');
insert into employee (name, birthday, email) values ('Lalo', '2000-12-19', 'lvonwellduny@canalblog.com');
insert into employee (name, birthday, email) values ('Lari', '1992-07-27', 'lelgyz@nature.com');
insert into employee (name, birthday, email) values ('Bonnibelle', '1985-08-08', 'bormston10@scribd.com');
insert into employee (name, birthday, email) values ('Jacques', '1995-06-04', 'jsatford11@lycos.com');
insert into employee (name, birthday, email) values ('Franny', '1992-05-20', 'fgeddes12@nifty.com');
insert into employee (name, birthday, email) values ('Tanhya', '2004-04-28', 'tparell13@freewebs.com');
insert into employee (name, birthday, email) values ('Feodor', '1992-11-27', 'fmcenery14@soundcloud.com');
insert into employee (name, birthday, email) values ('Deana', '1998-11-30', 'dsilburn15@topsy.com');
insert into employee (name, birthday, email) values ('Herminia', '1986-02-07', 'hspadazzi16@prlog.org');
insert into employee (name, birthday, email) values ('Zebadiah', '1989-08-06', 'zsmithson17@mtv.com');
insert into employee (name, birthday, email) values ('Crysta', '1996-06-20', 'cgreengrass18@blogspot.com');
insert into employee (name, birthday, email) values ('Cherie', '1989-10-22', 'chardwell19@chicagotribune.com');
insert into employee (name, birthday, email) values ('Allin', '2001-09-10', 'atrevor1a@nps.gov');
insert into employee (name, birthday, email) values ('Franklyn', '1987-07-25', 'fonolan1b@nsw.gov.au');
insert into employee (name, birthday, email) values ('Gonzalo', '1984-05-06', 'gjojic1c@state.tx.us');
insert into employee (name, birthday, email) values ('Valentia', '1986-11-03', 'vbeckmann1d@newyorker.com');
```
3. Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.
```sql
UPDATE employee
SET name='TEST-NAME'
WHERE id=10 
RETURNING *;
```
```sql
UPDATE employee
SET name='UPDATE-MULTIPLE',
    email= 'test@test-update.info'
WHERE id>30
RETURNING *;
```
```sql
UPDATE employee
SET name='DOWNDATE-MULTIPLE'
WHERE name='UPDATE-MULTIPLE'
RETURNING *;
```
```sql
UPDATE employee
SET birthday='1980-01-01',
	name = 'Overage'
WHERE email ILIKE 'TEST@%'
RETURNING *;
```
```sql
UPDATE employee
SET birthday='1981-01-01',
	name = 'UPDATED-AGAIN',
	email= 'updatedby@x.com'
WHERE email ILIKE '%ST@%'
RETURNING *;
```
4. Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.
```sql
DELETE FROM employee 
WHERE name ILIKE 'UPDA%'
RETURNING *;
```
```sql
DELETE FROM employee 
WHERE name ='TEST-NAME'
RETURNING *;
```
```sql
DELETE FROM employee 
WHERE birthday = '2022-11-03'
RETURNING *;
```
```sql
DELETe FROM employee
WHERE email ILIKE 'ehazel%'
RETURNING *;
```
```sql
DELETE FROM employee
WHERE id>10 AND id<20
RETURNING *;
```
