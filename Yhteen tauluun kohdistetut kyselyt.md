# Yhteen tauluun kohdistetut kyselyt

### Tehtävä 1
select * from goal;
![ruudunkaappaus](resources/03_tehtävä_1.png)

### Tehtävä 2
select name, type from airport 
where iso_country = "FI";
![ruudunkaappaus](resources/03_tehtävä_2.png)

### Tehtävä 3
select name from airport 
where iso_country = "FI" order by name asc;
![ruudunkaappaus](resources/03_tehtävä_3.png)

### Tehtävä 4
select name, type from airport 
where iso_country = "FI" order by type, name;
![ruudunkaappaus](resources/03_tehtävä_4.png)

### Tehtävä 5
select name from country 
where name like "F%";
![ruudunkaappaus](resources/03_tehtävä_5.png)

### Tehtävä 6
select name from country 
where name like "%F%";
![ruudunkaappaus](resources/03_tehtävä_6.png)

### Tehtävä 7
select location from game 
where screen_name = "Vesa";
![ruudunkaappaus](resources/03_tehtävä_7.png)

### Tehtävä 8
select co2_consumed from game 
where screen_name = "Ilkka";
![ruudunkaappaus](resources/03_tehtävä_8.png)

### Tehtävä 9
select co2_budget from game group by co2_budget;
![ruudunkaappaus](resources/03_tehtävä_9.png)