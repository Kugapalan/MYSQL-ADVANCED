# Antwoorden Eindopdracht
1. Copy paste je gemaakte SQL query hieronder





SELECT races.name as Race, circuits.name as Circuit 
FROM races 
JOIN circuits ON circuits.circuitId = races.raceId;





2. Copy paste je gemaakte SQL query hieronder




SELECT races.name as name, drivers.surname,driver_standing.points 
FROM races 
JOIN driver_standing ON races.raceId = driver_standing.raceId 
JOIN drivers ON driver_standing.driverId = drivers.driverId 
WHERE races.year = 2017 AND driver_standing.points = 10;




3. Copy paste je gemaakte SQL query hieronder




SELECT drivers.forename,drivers.surname,pitstops.time 
FROM drivers 
LEFT JOIN pitstops ON drivers.driverId = pitstops.driverId 
WHERE pitstops.duration < 25;




4. Copy paste je gemaakte SQL query hieronder




SELECT constructors.name as constructor, races.name AS GrandPrix 
FROM constructors 
LEFT JOIN constructor_standing ON constructors.constructorId = constructor_standing.constructorId 
LEFT JOIN races ON constructor_standing.raceId = races.raceId
WHERE constructors.name = 'Mclaren' AND year = 2010;




5. Copy paste je gemaakte SQL query hieronder




SELECT circuits.name AS circuit, circuits.country AS country, races.name AS GrandPrix, drivers.surname AS surname 
FROM drivers 
RIGHT JOIN driver_standing ON  driver_standing.driverId = drivers.driverId 
RIGHT JOIN races ON  races.raceId = driver_standing.raceId 
RIGHT JOIN circuits ON  circuits.circuitId = races.circuitId 
WHERE drivers.surname LIKE 'F%' AND races.year = 1950;


