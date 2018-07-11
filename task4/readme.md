select * from salesman;
select 'This is SQL Exercise, Practice and Solution';
select 1, 2, 3;
select 2 + 2;
select 2 + 2 * 2;
select name, commision from salesman;
select ord_date, salesman_id, ord_no, purch_amt from orders;
select distinct salesman_id from orders;
select name, city from salesman where city = 'Paris'
select *from customers where grade=200;
select ord_no, ord_date, purch_amt from orders where salesman_id=5001
select * from nobel_win where year=1970
select * from nobel_win where year=1971 and subject='Literature'
select year, subject from nobel_win where winner='Dennis Gabor'
select winner from nobel_win where year >= 1950 and subject='Physics'
