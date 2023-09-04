# second-hand-car

Second hand car dataset

#Task no.01. Read Cars data  

SELECT * FROM Car_dekho;

#Task no.02.Total Cars: To get a count of total records

SELECT COUNT(name) as total_cars FROM car_dekho;

#Task no.03. The manager asked the employee How many cars will be available in
2023? 

SELECT COUNT(name) as 2023_car FROM car_dekho WHERE year = "2023";

#Task no.04. The manager asked the employee How many cars is available in 2020,2021,2022

SELECT year, COUNT(*) as 20_21_22_cars FROM car_dekho WHERE year in (2020,2021,2022) GROUP BY year;

#Task no.05. Clint asked me to print the total of all cars by year.

SELECT year, COUNT(*)  FROM car_dekho  GROUP BY year;

#Task no.06. Clint asked to car dealer agent How many diesel cars will there be in 2020?

SELECT count(*) as diesel_car FROM car_dekho where Year = "2020" and fuel = "diesel";

#Task no.07. Clint requested a car dealer agent How many petrol cars will there be in 2020?

SELECT COUNT(*) FROM car_dekho WHERE fuel = "petrol" and year ="2020";

#Task no.08. The manager told the employee to give a print All the fuel cars (petrol, diesel, and CNG) come by all year.

SELECT year, fuel, COUNT(*) as numbers FROM car_dekho GROUP BY 1,2 ; 

#Task no.09. Manager said there were more than 100 cars in a given year, which year had more than 100 cars?

SELECT year, COUNT(*) FROM car_dekho GROUP BY 1 GAVING COUNT(*) >=100 ;

#Task no.10. The manager said to the employee All cars count details between 2015 and 2023; we need a complete list.

SELECT COUNT(*) FROM car_dekho WHERE year Between 2015 and 2023;

#Task no.11. The manager said to the employee All cars details between 2015 to 2023 we need complete list

SELECT * FROM car_dekho WHERE year between 2015 and 2023;

 
