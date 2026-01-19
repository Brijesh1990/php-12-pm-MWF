what is sql ? 
sql is stands for structured query language 
sql is a case-insenstive 
examples : Insert , INSERT , insert 
sql is used to create database and tables structured

sql create some commands .....

types of sql commands ...
a) DDL (data definition language)
b) DML (data manupulation language)
c) DQL (data query language)
c) TCL (transactional control language)  

DDL : stands for data definition language 
it is used to create database and tables structures 
DDL query are ...

1) create 2) alter 3) rename 4) change 5) drop  6) truncate

1) How to create a database in sql ...

query : create database database name;
examples :  create database flipkart_db;   
create database amazon;


what is database ? 
database is used to stored an information about users i.e called database. 

list out 5 database name ...
1) mySQL
2) sqlLite 
3) mongoDB 
4) sqlServer 
5) oracle 

Note : mysql database open source database.
mysql is case-sensitive 
examples : mysql     


2) how to create a table in database 
table : table is used to created and stored data in form of column and row i.e called tables.

users 

uid  name   age  pin     salary  address    

1    abc      32 36005   15600    rjt


chart ....

column name     datatype          size
id               int              default size (11)
name             char, varchar    (0-255)   
date             date , varchar   (0-255) 
datetime         datetime 
comments         text             
message          text 
price            int, float
mobile           bigInteger        default size (20)
image            blob, varchar     (0-255)


syntax : create table tablename
(
columnname datatype(size)  auto_increment primary key,
columnname datatype(size)  
.
.
.

)  

examples :
create table users 
(
user_id int AUTO_INCREMENT primary key,
name varchar(255),
email varchar(255),
password varchar(255),
address text,
mobile bigInt,
salary float  

)


create table country 
(
country_id int AUTO_INCREMENT primary key,
name varchar(255)
)


create table feedback 
(
feedback_id int AUTO_INCREMENT primary key,
name varchar(255),
email varchar(255),
ranking int,
phone bigint,
comment text      
)

3) alter :  alter is used to add | modify | update new column name after create tables. 

  syntax :
  a) add photo at the end of column name 
  alter table users add photo varchar(255);

 b) add photo after name column name 
   alter table users add photo varchar(255) after name;  

 c) update any column name via alter   

    alter table users change mobile phone bigint;
  
4) rename :  rename is used to rename any tables 

          rename table feedback to tbl_feedback

5) change :  change any column name 

    alter table users change mobile phone bigint;

6) truncate : truncate is used to remove or empty all data from tables 

    truncate table tbl_country;

    Note : after truncate we can not rollback data             

7) drop : drop is used to delete database and tables structures 

          a) drop database flipkart_db;
          b) drop table tbl_country; 
  
    
    
           
            
       