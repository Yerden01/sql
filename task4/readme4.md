select sum(purch_amt) from orders

select avg(purch_amt) from orders

select count(distinct salesman_id) from orders

select count(*) from orders

select count(all grade) from customer

select max(purch_amt) from orders

select min(purch_amt) from orders

select max(grade) from customer group by city

select max(purch_amt), customer_id from orders group by customer_id

select customer_id, ord_date, max(purch_amt) from orders group by customer_id, ord_date

select max(purch_amt), salesman_id from orders where ord_date = '2012-08-17' group by salesman_id

select max(purch_amt), customer_id, ord_date from orders where purch_amt > 2000 group by customer_id, ord_date

select max(purch_amt), customer_id, ord_date from orders where purch_amt between 2000 and 6000 group by customer_id, ord_date

select max(purch_amt), customer_id, ord_date from orders where purch_amt in (2000, 3000, 5760, 6000) group by customer_id, ord_date

select max(purch_amt), customer_id from orders where customer_id between 3002 and 3007 group by customer_id

select customer_id, max(purch_amt) from orders where (customer_id between 3002 and 3007) and purch_amt > 1000 group by customer_id

select max(purch_amt), salesman_id from orders where salesman_id between 5003 and 5008 group by salesman_id

select count(*) from orders where ord_date = '2012-08-17'

select count(*) from salesman where city is not null

select ord_date, salesman_id, count(*) from orders group by ord_date, salesman_id

select avg(pro_price) as "Average Price" from item_mast

select count(*) as "Number of products" from item_mast where pro_price >= 350

select avg(pro_price), pro_com from item_mast group by pro_com

select sum(dpt_allotment) from emp_department

select emp_dept, count(*) from emp_details group by emp_dept