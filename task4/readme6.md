select customer.cust_name, salesman.name, salesman.city from salesman, customer where salesman.city = customer.city

select customer.cust_name as "Customer", salesman.name as "Salesman" from customer, salesman where customer.salesman_id = salesman.salesman_id and customer.city = salesman.city

select ord_no, cust_name, orders.customer_id, orders.salesman_id from salesman, customer, orders where customer.city <> salesman.city and orders.customer_id = customer.customer_id and orders.salesman_id = salesman.salesman_id

select ord_no, cust_name from orders, customer where customer.customer_id = orders.customer_id

select customer.cust_name as "Customer", customer.grade as "Grade" from customer, orders, salesman where orders.customer_id = customer.customer_idand orders.salesman_id = salesman.salesman_id and salesman.city is not null and customer.grade is not null

select customer.cust_name as "Customer", customer.city as "City", salesman.name as "Salesman", salesman.commission as "commission" from customer, salesman where salesman.commission between 0.12 and 0.14 and salesman.salesman_id = customer.salesman_id

select orders.ord_no, customer.cust_name, salesman.commission, orders.purch_amt * salesman.commission from customer, salesman, orders where customer.grade >= 200 and orders.customer_id = customer.customer_id and orders.salesman_id = salesman.salesman_id