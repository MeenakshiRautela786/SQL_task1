# SQL_task1
-- Creating a new table
Create table if not exists office(
	employee_id int not null,
	first_name varchar(50),
	last_name varchar(50),
	hire_data date,
	salary float,
	department_id Int,
	primary key (employee_id)
)

-- add a new column to a table
Alter table office
add email varchar(50)

-- inserting data into table
insert into office values 
	(1,'krishna','kaniya','2023-02-03',55000.21,102,'krishna@sdnf.com'),
    (2,'radha','Rani','2022-11-13',2500.21,103,'radhaa@sdnf.com'),
	(3,'shayam','sharma','2023-02-03',250.21,102,'kasdnf.com'),	
	(4,'Ram','lal','2013-04-23',25000.21,102,null),
	(5,'Seeta','devi','2021-01-01',1000.21,102,'kaniyadnf.com'),
	(6,'jesus','christ','2010-02-09',5000.21,102, null),
	(7,'shiv','verma','2011-05-03',5500.21,102,'raytela@sdnf.com')


-- showing data and table using select statement 
SELECT * FROM OFFICE

-- using select statement with where clause 
SELECT * FROM OFFICE WHERE first_name ='krishna'
	
-- removing an existing column in the 'office' table using DDL (alter)
Alter table office DROP EMAIL

-- after removing email
select * from office

