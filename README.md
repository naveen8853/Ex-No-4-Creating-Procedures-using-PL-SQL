# Ex. No: 4 Creating Procedures using PL/SQL

## AIM: 
To create a procedure using PL/SQL.

## Steps:
1. Create employee table with following attributes (empid NUMBER, empname VARCHAR(10), dept VARCHAR(10),salary NUMBER);
2. Create a procedure named as insert_employee data.
3. Inside the procdure block, write the query for inserting the values into the employee table.
4. End the procedure.
5. Call the insert_employee data procedure to insert the values into the employee table.
6. Display the employee table

## Program:

## Program To Create Table:
```
create table EMPLOYEE3 (empid NUMBER, empname VARCHAR(20), dept VARCHAR(10),salary NUMBER);
```
## Program To Create Procedure:
```
 create or replace procedure insert_employee_data as
  2  begin
  3  insert into employee3 values(1,'Pavan Kalyan','HR',100000);
  4  insert into employee3 values(2,'Naveen','IT',80000);
  5  insert into employee3 values(3,'Roobesh','Finance',70000);
  6  COMMIT;
  7  END;
  8  /
```
## Program To Call The Procedure:
```
 BEGIN
  2  insert_employee_data;
  3  END;
  4  /
```
## Program To Display The Table:
```
select * from employee3;
```
## Output:
![](Ex1.12.png)
## Result:
  Hence procedure has been created using PL/SQL.
