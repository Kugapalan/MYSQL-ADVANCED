# Antwoorden

1. Copy paste je gemaakte SQL query hieronder

127.0.0.1/mod-mysql-advanced-videogames-joins/		http://localhost/phpmyadmin/index.php?route=/database/sql&db=mod-mysql-advanced-videogames-joins

   Weergave van records 0 - 14 (15 totaal, Query duurde 0,0006 seconden.)


SELECT game.name , platform.platform FROM game LEFT JOIN platform ON  game.platform_id = platform.platform  WHERE game.name LIKE 'Grand Theft Auto%';


name	platform	
Grand Theft Auto V	
    NULL
	
Grand Theft Auto: San Andreas	
    NULL
	
Grand Theft Auto V	
    NULL
	
Grand Theft Auto: Vice City	
    NULL
	
Grand Theft Auto III	
    NULL
	
Grand Theft Auto V	
    NULL
	
Grand Theft Auto IV	
    NULL
	
Grand Theft Auto IV	
    NULL
	
Grand Theft Auto: Liberty City Stories	
    NULL
	
Grand Theft Auto V	
    NULL
	
Grand Theft Auto: Vice City Stories	
    NULL
	
Grand Theft Auto: Liberty City Stories	
    NULL
	
Grand Theft Auto 2	
    NULL
	
Grand Theft Auto	
    NULL
	
Grand Theft Auto: San Andreas	
    NULL
	


2. Copy paste je gemaakte SQL query hieronder
   
127.0.0.1/mod-mysql-advanced-videogames-joins/		http://localhost/phpmyadmin/index.php?route=/database/sql&db=mod-mysql-advanced-videogames-joins

   Weergave van records 0 -  0 (1 totaal, Query duurde 0,0003 seconden.)


SELECT game.name , platform.platform FROM game RIGHT JOIN platform ON  platform.platform = game.platform_id WHERE platform="SCD";




    NULL
	SCD	
