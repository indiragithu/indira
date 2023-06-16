# indira
back end assignment
//creating warehouse
create database warhouse;

//delete warehouse 
delete database warehouse

//creating a table
create table product(
productname varchar(255),
skunumber varchar(255),
quantity int,
);

//adding products to stock
insert into product values('pen','prod0001',50);
insert into product values('pencil','prod0002',40);
insert into product values('book','prod0003',70);
insert into product values('sketches','prod0004',50);
insert into product values('ball','prod0005',60);
insert into product values('bat','prod0006',30);
insert into product values('box','prod0007',20);
insert into product values('colors','prod0008',50);
insert into product values('mouse','prod0009',90);
insert into product values('kayboard','prod0010',10);

//unstock the specified product
delete from product where skunumber='prod0005';

//two ways of listing the products
select * from product;

select count(quantity)
from product
where productname='book';
