# Antwoorden Eindopdracht

1. Copy paste je gemaakte SQL query hieronder
   
127.0.0.1/mod-mysql-advanced-formula1-7tables/races/		http://localhost/phpmyadmin/index.php?route=/database/sql&db=mod-mysql-advanced-formula1-7tables

   Weergave van records 0 - 24 (454125964 totaal, Query duurde 0,0047 seconden.)


SELECT races.name , drivers.surname , driver_standing.points FROM races  , drivers ,driver_standing
WHERE races.year = '2009';


name	surname	points	
Australian Grand Prix	Hamilton	10	
Australian Grand Prix	Heidfeld	10	
Australian Grand Prix	Rosberg	10	
Australian Grand Prix	Alonso	10	
Australian Grand Prix	Kovalainen	10	
Australian Grand Prix	Nakajima	10	
Australian Grand Prix	Bourdais	10	
Australian Grand Prix	RÌ_ikkÌ¦nen	10	
Australian Grand Prix	Kubica	10	
Australian Grand Prix	Glock	10	
Australian Grand Prix	Sato	10	
Australian Grand Prix	Piquet Jr.	10	
Australian Grand Prix	Massa	10	
Australian Grand Prix	Coulthard	10	
Australian Grand Prix	Trulli	10	
Australian Grand Prix	Sutil	10	
Australian Grand Prix	Webber	10	
Australian Grand Prix	Button	10	
Australian Grand Prix	Davidson	10	
Australian Grand Prix	Vettel	10	
Australian Grand Prix	Fisichella	10	
Australian Grand Prix	Barrichello	10	
Australian Grand Prix	Schumacher	10	
Australian Grand Prix	Liuzzi	10	
Australian Grand Prix	Wurz	10	


2. Copy paste je gemaakte SQL query hieronder

127.0.0.1/mod-mysql-advanced-formula1-7tables/		http://localhost/phpmyadmin/index.php?route=/database/sql&db=mod-mysql-advanced-formula1-7tables

   Weergave van records 0 - 24 (622035920 totaal, Query duurde 0,0131 seconden.)


SELECT races.name AS 'race' , circuits.name AS 'circuit', drivers.surname
FROM  races , circuits , driver_standing , drivers
WHERE races.year = '2017' 
AND driver_standing.points = 10;


race	circuit	surname	
Australian Grand Prix	Albert Park Grand Prix Circuit	Hamilton	
Australian Grand Prix	Sepang International Circuit	Hamilton	
Australian Grand Prix	Bahrain International Circuit	Hamilton	
Australian Grand Prix	Circuit de Barcelona-Catalunya	Hamilton	
Australian Grand Prix	Istanbul Park	Hamilton	
Australian Grand Prix	Circuit de Monaco	Hamilton	
Australian Grand Prix	Circuit Gilles Villeneuve	Hamilton	
Australian Grand Prix	Circuit de Nevers Magny-Cours	Hamilton	
Australian Grand Prix	Silverstone Circuit	Hamilton	
Australian Grand Prix	Hockenheimring	Hamilton	
Australian Grand Prix	Hungaroring	Hamilton	
Australian Grand Prix	Valencia Street Circuit	Hamilton	
Australian Grand Prix	Circuit de Spa-Francorchamps	Hamilton	
Australian Grand Prix	Autodromo Nazionale di Monza	Hamilton	
Australian Grand Prix	Marina Bay Street Circuit	Hamilton	
Australian Grand Prix	Fuji Speedway	Hamilton	
Australian Grand Prix	Shanghai International Circuit	Hamilton	
Australian Grand Prix	Aut?_dromo Jos̩ Carlos Pace	Hamilton	
Australian Grand Prix	Indianapolis Motor Speedway	Hamilton	
Australian Grand Prix	N?_rburgring	Hamilton	
Australian Grand Prix	Autodromo Enzo e Dino Ferrari	Hamilton	
Australian Grand Prix	Suzuka Circuit	Hamilton	
Australian Grand Prix	A1-Ring	Hamilton	
Australian Grand Prix	Yas Marina Circuit	Hamilton	
Australian Grand Prix	Aut?_dromo Juan y Oscar G??lvez	Hamilton	



3. Copy paste je gemaakte SQL query hieronder
   
   127.0.0.1/mod-mysql-advanced-formula1-7tables/		http://localhost/phpmyadmin/index.php?route=/database/sql&db=mod-mysql-advanced-formula1-7tables

   Weergave van records 0 - 24 (3779738 totaal, Query duurde 0,0020 seconden.)


SELECT  drivers.forename ,  drivers.surname , pitstops.duration
FROM   drivers , pitstops
WHERE pitstops.duration <= '25';


forename	surname	duration	
Lewis	Hamilton	23.426	
Nick	Heidfeld	23.426	
Nico	Rosberg	23.426	
Fernando	Alonso	23.426	
Heikki	Kovalainen	23.426	
Kazuki	Nakajima	23.426	
SÌ©bastien	Bourdais	23.426	
Kimi	RÌ_ikkÌ¦nen	23.426	
Robert	Kubica	23.426	
Timo	Glock	23.426	
Takuma	Sato	23.426	
Nelson	Piquet Jr.	23.426	
Felipe	Massa	23.426	
David	Coulthard	23.426	
Jarno	Trulli	23.426	
Adrian	Sutil	23.426	
Mark	Webber	23.426	
Jenson	Button	23.426	
Anthony	Davidson	23.426	
Sebastian	Vettel	23.426	
Giancarlo	Fisichella	23.426	
Rubens	Barrichello	23.426	
Ralf	Schumacher	23.426	
Vitantonio	Liuzzi	23.426	
Alexander	Wurz	23.426	



4. Copy paste je gemaakte SQL query hieronder
   
127.0.0.1/mod-mysql-advanced-formula1-7tables/		http://localhost/phpmyadmin/index.php?route=/database/sql&db=mod-mysql-advanced-formula1-7tables

   Weergave van records 0 - 18 (19 totaal, Query duurde 0,0023 seconden.)


SELECT constructors.name , races.name AS 'GrandPrix'
FROM   constructors , races
WHERE constructors.name = 'McLaren'
AND races.year = '2010';


name	GrandPrix	
McLaren	Bahrain Grand Prix	
McLaren	Australian Grand Prix	
McLaren	Malaysian Grand Prix	
McLaren	Chinese Grand Prix	
McLaren	Spanish Grand Prix	
McLaren	Monaco Grand Prix	
McLaren	Turkish Grand Prix	
McLaren	Canadian Grand Prix	
McLaren	European Grand Prix	
McLaren	British Grand Prix	
McLaren	German Grand Prix	
McLaren	Hungarian Grand Prix	
McLaren	Belgian Grand Prix	
McLaren	Italian Grand Prix	
McLaren	Singapore Grand Prix	
McLaren	Japanese Grand Prix	
McLaren	Korean Grand Prix	
McLaren	Brazilian Grand Prix	
McLaren	Abu Dhabi Grand Prix	


   
5. Copy paste je gemaakte SQL query hieronder
   
127.0.0.1/mod-mysql-advanced-formula1-7tables/		http://localhost/phpmyadmin/index.php?route=/database/sql&db=mod-mysql-advanced-formula1-7tables

   Weergave van records 0 - 24 (20440 totaal, Query duurde 0,0031 seconden.)


SELECT circuits.name , circuits.country , races.name AS 'GrandPrix', drivers.surname
FROM   circuits , races , drivers
WHERE races.year = '1950'
AND drivers.surname LIKE 'F%';


name	country	GrandPrix	surname	
Albert Park Grand Prix Circuit	Australia	British Grand Prix	Fisichella	
Sepang International Circuit	Malaysia	British Grand Prix	Fisichella	
Bahrain International Circuit	Bahrain	British Grand Prix	Fisichella	
Circuit de Barcelona-Catalunya	Spain	British Grand Prix	Fisichella	
Istanbul Park	Turkey	British Grand Prix	Fisichella	
Circuit de Monaco	Monaco	British Grand Prix	Fisichella	
Circuit Gilles Villeneuve	Canada	British Grand Prix	Fisichella	
Circuit de Nevers Magny-Cours	France	British Grand Prix	Fisichella	
Silverstone Circuit	UK	British Grand Prix	Fisichella	
Hockenheimring	Germany	British Grand Prix	Fisichella	
Hungaroring	Hungary	British Grand Prix	Fisichella	
Valencia Street Circuit	Spain	British Grand Prix	Fisichella	
Circuit de Spa-Francorchamps	Belgium	British Grand Prix	Fisichella	
Autodromo Nazionale di Monza	Italy	British Grand Prix	Fisichella	
Marina Bay Street Circuit	Singapore	British Grand Prix	Fisichella	
Fuji Speedway	Japan	British Grand Prix	Fisichella	
Shanghai International Circuit	China	British Grand Prix	Fisichella	
Aut?_dromo Jos̩ Carlos Pace	Brazil	British Grand Prix	Fisichella	
Indianapolis Motor Speedway	USA	British Grand Prix	Fisichella	
N?_rburgring	Germany	British Grand Prix	Fisichella	
Autodromo Enzo e Dino Ferrari	Italy	British Grand Prix	Fisichella	
Suzuka Circuit	Japan	British Grand Prix	Fisichella	
A1-Ring	Austria	British Grand Prix	Fisichella	
Yas Marina Circuit	UAE	British Grand Prix	Fisichella	
Aut?_dromo Juan y Oscar G??lvez	Argentina	British Grand Prix	Fisichella	
