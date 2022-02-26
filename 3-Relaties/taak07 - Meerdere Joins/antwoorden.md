# Antwoorden

1. Copy paste je gemaakte SQL query hieronder


127.0.0.1/mod-mysql-advanced-videogames-full/		http://localhost/phpmyadmin/index.php?route=/database/sql&db=mod-mysql-advanced-videogames-full

   Weergave van records 0 - 24 (13020 totaal, Query duurde 0,0006 seconden.)


SELECT game.name ,platform.platform , genre.genre FROM game , genre , platform WHERE game.name LIKE 'b%';


name	platform	genre	
Brain Age: Train Your Brain in Minutes a Day	Wii	Sports	
Brain Age: Train Your Brain in Minutes a Day	Wii	Platform	
Brain Age: Train Your Brain in Minutes a Day	Wii	Racing	
Brain Age: Train Your Brain in Minutes a Day	Wii	Role-Playing	
Brain Age: Train Your Brain in Minutes a Day	Wii	Puzzle	
Brain Age: Train Your Brain in Minutes a Day	Wii	Misc	
Brain Age: Train Your Brain in Minutes a Day	Wii	Shooter	
Brain Age: Train Your Brain in Minutes a Day	Wii	Simulation	
Brain Age: Train Your Brain in Minutes a Day	Wii	Action	
Brain Age: Train Your Brain in Minutes a Day	Wii	Fighting	
Brain Age: Train Your Brain in Minutes a Day	Wii	Adventure	
Brain Age: Train Your Brain in Minutes a Day	Wii	Strategy	
Brain Age: Train Your Brain in Minutes a Day	NES	Sports	
Brain Age: Train Your Brain in Minutes a Day	NES	Platform	
Brain Age: Train Your Brain in Minutes a Day	NES	Racing	
Brain Age: Train Your Brain in Minutes a Day	NES	Role-Playing	
Brain Age: Train Your Brain in Minutes a Day	NES	Puzzle	
Brain Age: Train Your Brain in Minutes a Day	NES	Misc	
Brain Age: Train Your Brain in Minutes a Day	NES	Shooter	
Brain Age: Train Your Brain in Minutes a Day	NES	Simulation	
Brain Age: Train Your Brain in Minutes a Day	NES	Action	
Brain Age: Train Your Brain in Minutes a Day	NES	Fighting	
Brain Age: Train Your Brain in Minutes a Day	NES	Adventure	
Brain Age: Train Your Brain in Minutes a Day	NES	Strategy	
Brain Age: Train Your Brain in Minutes a Day	GB	Sports	

   
2. Copy paste je gemaakte SQL query hieronder

127.0.0.1/mod-mysql-advanced-videogames-full/		http://localhost/phpmyadmin/index.php?route=/database/sql&db=mod-mysql-advanced-videogames-full

   Weergave van records 0 - 24 (10825200 totaal, Query duurde 0,0024 seconden.)


SELECT game.name ,platform.platform , publisher.publisher , game.year FROM game , genre , platform , publisher WHERE game.year = '2013';


name	platform	publisher	year	
Grand Theft Auto V	Wii	Nintendo	2013	
Grand Theft Auto V	Wii	Nintendo	2013	
Grand Theft Auto V	Wii	Nintendo	2013	
Grand Theft Auto V	Wii	Nintendo	2013	
Grand Theft Auto V	Wii	Nintendo	2013	
Grand Theft Auto V	Wii	Nintendo	2013	
Grand Theft Auto V	Wii	Nintendo	2013	
Grand Theft Auto V	Wii	Nintendo	2013	
Grand Theft Auto V	Wii	Nintendo	2013	
Grand Theft Auto V	Wii	Nintendo	2013	
Grand Theft Auto V	Wii	Nintendo	2013	
Grand Theft Auto V	Wii	Nintendo	2013	
Grand Theft Auto V	NES	Nintendo	2013	
Grand Theft Auto V	NES	Nintendo	2013	
Grand Theft Auto V	NES	Nintendo	2013	
Grand Theft Auto V	NES	Nintendo	2013	
Grand Theft Auto V	NES	Nintendo	2013	
Grand Theft Auto V	NES	Nintendo	2013	
Grand Theft Auto V	NES	Nintendo	2013	
Grand Theft Auto V	NES	Nintendo	2013	
Grand Theft Auto V	NES	Nintendo	2013	
Grand Theft Auto V	NES	Nintendo	2013	
Grand Theft Auto V	NES	Nintendo	2013	
Grand Theft Auto V	NES	Nintendo	2013	
Grand Theft Auto V	GB	Nintendo	2013	


3. Copy paste je gemaakte SQL query hieronder

127.0.0.1/mod-mysql-advanced-videogames-full/game/		http://localhost/phpmyadmin/index.php?route=/database/sql&db=mod-mysql-advanced-videogames-full

   Weergave van records 0 - 24 (17987874 totaal, Query duurde 0,0031 seconden.)


SELECT game.name ,genre.genre, game.global_sales , game.year FROM game JOIN genre , platform , publisher WHERE genre.genre = 'Puzzle';


name	genre	global_sales	year	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	
Wii Sports	Puzzle	8253	2006	


4. Copy paste je gemaakte SQL query hieronder

127.0.0.1/mod-mysql-advanced-videogames-full/game/		http://localhost/phpmyadmin/index.php?route=/database/sql&db=mod-mysql-advanced-videogames-full

   Weergave van records 0 - 24 (6711624 totaal, Query duurde 0,0030 seconden.)


SELECT platform.platform , game.year , genre.genre , publisher.publisher,  game.jp_sales FROM game JOIN genre , platform , publisher WHERE game.name LIKE 'Mario%';


platform	year	genre	publisher	jp_sales	
Wii	2008	Sports	Nintendo	379	
Wii	2008	Platform	Nintendo	379	
Wii	2008	Racing	Nintendo	379	
Wii	2008	Role-Playing	Nintendo	379	
Wii	2008	Puzzle	Nintendo	379	
Wii	2008	Misc	Nintendo	379	
Wii	2008	Shooter	Nintendo	379	
Wii	2008	Simulation	Nintendo	379	
Wii	2008	Action	Nintendo	379	
Wii	2008	Fighting	Nintendo	379	
Wii	2008	Adventure	Nintendo	379	
Wii	2008	Strategy	Nintendo	379	
NES	2008	Sports	Nintendo	379	
NES	2008	Platform	Nintendo	379	
NES	2008	Racing	Nintendo	379	
NES	2008	Role-Playing	Nintendo	379	
NES	2008	Puzzle	Nintendo	379	
NES	2008	Misc	Nintendo	379	
NES	2008	Shooter	Nintendo	379	
NES	2008	Simulation	Nintendo	379	
NES	2008	Action	Nintendo	379	
NES	2008	Fighting	Nintendo	379	
NES	2008	Adventure	Nintendo	379	
NES	2008	Strategy	Nintendo	379	
GB	2008	Sports	Nintendo	379	


5. Copy paste je gemaakte SQL query hieronder
   
127.0.0.1/mod-mysql-advanced-videogames-full/game/		http://localhost/phpmyadmin/index.php?route=/database/sql&db=mod-mysql-advanced-videogames-full

   Weergave van records 0 - 24 (6963048 totaal, Query duurde 0,0036 seconden.)


SELECT game.name ,genre.genre , publisher.publisher,  game.year FROM game JOIN genre , platform , publisher WHERE platform.platform = 'PC';


name	genre	publisher	year	
Wii Sports	Sports	Nintendo	2006	
Wii Sports	Platform	Nintendo	2006	
Wii Sports	Racing	Nintendo	2006	
Wii Sports	Role-Playing	Nintendo	2006	
Wii Sports	Puzzle	Nintendo	2006	
Wii Sports	Misc	Nintendo	2006	
Wii Sports	Shooter	Nintendo	2006	
Wii Sports	Simulation	Nintendo	2006	
Wii Sports	Action	Nintendo	2006	
Wii Sports	Fighting	Nintendo	2006	
Wii Sports	Adventure	Nintendo	2006	
Wii Sports	Strategy	Nintendo	2006	
Wii Sports	Sports	Microsoft Game Studios	2006	
Wii Sports	Platform	Microsoft Game Studios	2006	
Wii Sports	Racing	Microsoft Game Studios	2006	
Wii Sports	Role-Playing	Microsoft Game Studios	2006	
Wii Sports	Puzzle	Microsoft Game Studios	2006	
Wii Sports	Misc	Microsoft Game Studios	2006	
Wii Sports	Shooter	Microsoft Game Studios	2006	
Wii Sports	Simulation	Microsoft Game Studios	2006	
Wii Sports	Action	Microsoft Game Studios	2006	
Wii Sports	Fighting	Microsoft Game Studios	2006	
Wii Sports	Adventure	Microsoft Game Studios	2006	
Wii Sports	Strategy	Microsoft Game Studios	2006	
Wii Sports	Sports	Take-Two Interactive	2006	

