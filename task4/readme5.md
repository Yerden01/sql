select salesman_id, name, city, commission * 100 from salesman 

select 'For ', ord_date, ' there are ', count(ord_no), ' orders.' from orders group by ord_date

select *from orders order by ord_no

select *from orders order by ord_date desc

select *from orders order by ord_date, purch_amt desc

select *from customer order by customer_id

select salesman_id, ord_date, max(purch_amt) from orders group by salesman_id, ord_date order by salesman_id, ord_date

select *from customer order by grade desc

select customer_id, count(distinct ord_no), max(purch_amt) from orders group by customer_id order by 2 desc, 3 desc

select ord_date, sum(purch_amt), sum(purch_amt) * 0.15 from orders group by ord_date order by ord_date