select *from salesman where city = 'Rome' or city = 'Paris'

select *from salesman where city in ('Paris', 'Rome')

select *from salesman where city not in ('Paris', 'Rome')

select *from customer where customer_id in (3007, 3008, 3009)

select *from salesman where commission between 0.12 and 0.14

select *from orders where (purch_amt between 500 and 4000) and not purch_amt in (948.50, 1983.43)

select *from salesman where name between 'A' and 'K'

select *from salesman where name not between 'A' and 'L'

select *from customer where cust_name like 'B%'

select *from customer where cust_name like '%n'

select *from salesman where name like 'N__l%'

please explain this one about escape

and this one also

select *from testtable where col1 like '%/%' but in answer using escape please explain

select *from testtable where col1 not like '%/%'

select *from testtable where col1 like '%/_//%' escape '/'

select *from testtable where col1 not like '%/_//%' escape '/'

select *from testtable where col1 like '%/%%' escape '/' 

select *from testtable where col1 not like '%/%%' escape '/' 

select *from customer where grade is null

select *from customer where grade is not null

select *from emp_details where emp_lname like 'D%'