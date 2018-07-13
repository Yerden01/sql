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

select * from nobel_win where subject = 'Chemistry' and year>=1965 and year<=1975;

select * from nobel_win where year > 1972 and category = 'Prime Minister'

select * from nobel_win where winner like 'Louis%'

select * from nobel_win where subject='Physics' and year = 1970 union select * from nobel_win where subject='Economics' and year = 1971

select * from nobel_win where subject not in ('Physiology', 'Economics') and year = 1970

select * from nobel_win where subject = 'Physiology' and year < 1971 union select * from nobel_win where subject = 'Peace' and year >= 1974

select * from nobel_win where winner = 'Johannes Georg Bednorz'

select * from nobel_win where subject not like 'P%' order by year desc, winner

select * from nobel_win where year = 1970 order by case when subject in ('Economics', 'Chemistry') then 1 else 0 end asc, subject, winner

select * from item_mast where pro_price between 200 and 600

select avg(pro_price) from item_mast where pro_com = 16

select pro_name as "Item name", pro_price as "Price in Rs." from item_mast

select pro_name, pro_price from item_mast where pro_price>=250 order by pro_price desc, pro_name

select avg(pro_price), pro_com from item_mast group by pro_com

select pro_name, pro_price from item_mast where pro_price=(select min(pro_price) from item_mast)

select distinct emp_lname from emp_details

select *from emp_details where emp_lname = 'Snares'

select *from emp_details where emp_dept = 57