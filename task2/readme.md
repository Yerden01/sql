//chapter 1
mysql --help //all commands 

//chapter 2
mysql -u root -p  //mysql -u 'login' -p 'password' but initially 'login'='root' 'password'=''

//chapter 3
select version(), current_date; //version and date only
select sin(PI()/4), (4 + 1) * 5; //mathematical calculations 
select version(); select now(); //version of mysql and date and time now
select user(), \c // \c is used for breaking

//chapter 4
show databases; //show all databases you have
use 'database_name' //to use database
//4.1
create database 'database_name' //creating database
//4.2
show tables; //show tables:)
create table pet (name VARCHAR(20), owner VARCHAR(20),
    -> species varchar(20), sex char(1), birth date, death date);//creating table varchar is
	//like array of chars '(20)' is length; 
describe 'table_name'; //describes table
//4.3
insert into pet //inserting information to table
    -> values ('Puffball', 'Diane', 'hamster', 'f', '2015-05-12', null);
//4.4.1
select * from pet // select * from 'table_name' used to select all
update pet set birth = '2016-05-12' where name = 'Puffball' // to update information in table
//4.4.2
select * from employers where Salary > 900; //selects all which birth is bigger or equal to your statement
select * from employers where position = 'specialist' and salary = '900'; //and operations
//4.4.3
select name, city from employers where salary = 900; //to show only 2 column name and city
select distinct salary from employers; // distinct used if it contains one element 2 or more it shows only one
//4.4.4
select name, salary from employers order by salary; //sorted by salary
select name, salary from employers order by salary desc; // sorted by descending order
