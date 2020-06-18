# Dim-Date-Project

create table dim_day (
 day_key int not null auto_increment,   -- primay key.
 date datetime ,     -- date: 2008-08-18 00:00:00
 date_num int(8),    -- numeric value, in YYYYMMDD, 20080818
 day_num int (2),    -- numeric value, 18
 day_of_year int(4), -- the day of the year 
 day_of_week int(2), -- the day of the week
 day_of_week_name varchar(20), -- day of week name (Monday, Tuesday,etc)
 week_num int (2), --  week of the year 
 week_begin_date date,  -- week begin date
 week_end_date date, -- week end date
 last_week_begin_date date,  -- priore week begin date
 last_week_end_date date,   priore week end date
 last_2_week_begin_date  date,   -- priore two week begin date
 last_2_week_end_date date,  -- priore two ween end date
 month_num int (2) ,  -- month in number, ie. 12
 month_name varchar(20),  -- month in name, ie. December
 YEARMONTH_NUM int(6),  -- year and month in number, ie. 201212
 last_month_num int (2), -- priore month in number, ie. 11
 last_month_name varchar(20), -- priore month in name, November
 last_month_year int(4),  -- priore month in year, 2012
 last_yearmonth_num int(6), -- priore year and month in  number, ie, 2o1211
 quarter_num int (2),  -- quarter in number, ie 4
 year_num int (4), -- year in number, ie, 2012
 created_date timestamp not null  ,  -- date record was created
 updated_date timestamp not null , -- date record was updated
 primary key (day_key)
 );
