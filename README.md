business_info table query

create table business_info (
business_id varchar(20), 
business_name varchar(200),
contact_person varchar(200),
Local_address varchar(200),
city varchar(50),
pincode varchar(20),
states varchar(50),
GST varchar(50)) ;


LOAD DATA INFILE 'F:\\Business_info1.csv'
INTO TABLE business_info
FIELDS TERMINATED BY ',' 
OPTIONALLY ENCLOSED BY '"'
LINES TERMINATED BY '\n'
IGNORE 1 ROWS;
