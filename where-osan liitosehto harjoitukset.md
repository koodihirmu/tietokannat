# where-osan liitosehto harjoitukset

### Tehtävä 1
select country.name as "country name", airport.name as "airport name"
from airport, country
where airport.iso_country = country.iso_country
and country.name = "Iceland";
![ruudunkaappaus](resources/04_tehtävä_1.png)

### Tehtävä 2
select airport.name as "airport name"
from airport, country
where airport.iso_country = country.iso_country
and country.name = "France"
and type = "large_airport";
![ruudunkaappaus](resources/04_tehtävä_2.png)

### Tehtävä 3
select country.name as "country_name", airport.name as "airport_name"
from country, airport
where airport.iso_country = country.iso_country 
and airport.continent = "AN";
![ruudunkaappaus](resources/04_tehtävä_3.png)

### Tehtävä 4
select airport.elevation_ft from game, airport
where game.location = airport.ident
and screen_name = "Heini";
![ruudunkaappaus](resources/04_tehtävä_4.png)

### Tehtävä 5
select airport.elevation_ft * 0.3048 as elevation_m from game, airport
where game.location = airport.ident
and screen_name = "Heini";
![ruudunkaappaus](resources/04_tehtävä_5.png)

### Tehtävä 6
select airport.name from game, airport
where game.location = airport.ident
and screen_name = "Ilkka";
![ruudunkaappaus](resources/04_tehtävä_6.png)

### Tehtävä 7
select country.name from game, country, airport
where game.location = airport.ident
and airport.iso_country = country.iso_country
and screen_name = "Ilkka";
![ruudunkaappaus](resources/04_tehtävä_7.png)

### Tehtävä 8
select goal.name from game, goal_reached, goal
where game_id = game.id
and goal_id = goal.id
and screen_name = "Heini";
![ruudunkaappaus](resources/04_tehtävä_8.png)

### Tehtävä 9
select airport.name from game, goal_reached, goal, airport
where game_id = game.id
and goal_id = goal.id
and location = ident
and screen_name = "Ilkka"
and goal.name like "%CLOUDS%";
![ruudunkaappaus](resources/04_tehtävä_9.png)

### Tehtävä 10
select country.name from game, goal_reached, goal, airport, country
where game_id = game.id
and goal_id = goal.id
and location = ident
and screen_name = "Ilkka"
and airport.iso_country = country.iso_country
and goal.name like "%CLOUDS%";
![ruudunkaappaus](resources/04_tehtävä_10.png)