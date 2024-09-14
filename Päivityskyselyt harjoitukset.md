# Päivityskyselyt harjoitukset

### Tehtävä 1
update game
set location =
(
    select ident
    from airport
    where name = "Nottingham Airport"
),
    co2_consumed = co2_consumed + 500
where screen_name = "vesa";

![ruudunkaappaus](resources/08_tehtävä_1.png)

### Tehtävä 2
a

![ruudunkaappaus](resources/08_tehtävä_2.png)

### Tehtävä 3
delete from goal_reached;

![ruudunkaappaus](resources/08_tehtävä_3.png)

### Tehtävä 4
delete from game;

![ruudunkaappaus](resources/08_tehtävä_4.png)