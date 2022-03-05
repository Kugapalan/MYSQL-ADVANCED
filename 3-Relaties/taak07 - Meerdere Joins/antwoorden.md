# Antwoorden

1. Copy paste je gemaakte SQL query hieronder

127.0.0.1/mod-mysql-advanced-videogames-full/		http://localhost/phpmyadmin/index.php?route=/database/sql&db=mod-mysql-advanced-videogames-full

   Weergave van records 0 - 24 (35 totaal, Query duurde 0,0054 seconden.)


SELECT game.name, platform.platform, genre.genre FROM game
LEFT JOIN platform ON game.platform_id = platform.id
LEFT JOIN genre ON game.genre_id = genre.id
WHERE game.name LIKE "b%";


name	platform	genre	
Brain Age: Train Your Brain in Minutes a Day	DS	Misc	
Brain Age 2: More Training in Minutes a Day	DS	Puzzle	
Battlefield 3	X360	Shooter	
Battlefield 3	PS3	Shooter	
Big Brain Academy	DS	Misc	
Batman: Arkham City	PS3	Action	
Batman: Arkham City	X360	Action	
Batman: Arkham Asylum	PS3	Action	
Battlefield 1	PS4	Shooter	
Batman: Arkham Knight	PS4	Action	
Big Brain Academy: Wii Degree	Wii	Misc	
Banjo-Kazooie	N64	Platform	
Battlefield 4	PS4	Shooter	
Battlefield 4	PS3	Shooter	
Batman: Arkham Asylum	X360	Action	
Battlefield 4	X360	Shooter	
Battlefield: Bad Company 2	X360	Shooter	
Borderlands	X360	Shooter	
Baseball	NES	Sports	
Borderlands 2	X360	Shooter	
Battlefield: Bad Company 2	PS3	Shooter	
BioShock	X360	Shooter	
Battlefield 3	PC	Shooter	
Burnout 3: Takedown	PS2	Racing	
Bloodborne	PS4	Action	


   
2. Copy paste je gemaakte SQL query hieronder

127.0.0.1/mod-mysql-advanced-videogames-full/		http://localhost/phpmyadmin/index.php?route=/database/sql&db=mod-mysql-advanced-videogames-full

   Weergave van records 0 - 24 (29100 totaal, Query duurde 0,0006 seconden.)


SELECT game.name, platform.platform , publisher.publisher , game.year FROM game
LEFT JOIN platform ON game.platform_id = platform.id
LEFT JOIN genre ON game.genre_id = genre.id
LEFT JOIN publisher ON publisher.id = publisher.id
WHERE game.year = "2013";


name	platform	publisher	year	
Grand Theft Auto V	PS3	Nintendo	2013	
Grand Theft Auto V	X360	Nintendo	2013	
Pokemon X/Pokemon Y	3DS	Nintendo	2013	
Call of Duty: Ghosts	X360	Nintendo	2013	
Call of Duty: Ghosts	PS3	Nintendo	2013	
Minecraft	X360	Nintendo	2013	
FIFA 14	PS3	Nintendo	2013	
The Last of Us	PS3	Nintendo	2013	
Tomodachi Life	3DS	Nintendo	2013	
Luigi's Mansion: Dark Moon	3DS	Nintendo	2013	
Super Mario 3D World	WiiU	Nintendo	2013	
FIFA 14	X360	Nintendo	2013	
Call of Duty: Ghosts	PS4	Nintendo	2013	
Assassin's Creed IV: Black Flag	PS3	Nintendo	2013	
Battlefield 4	PS4	Nintendo	2013	
Just Dance 2014	Wii	Nintendo	2013	
Battlefield 4	PS3	Nintendo	2013	
Battlefield 4	X360	Nintendo	2013	
Monster Hunter 4	3DS	Nintendo	2013	
Assassin's Creed IV: Black Flag	X360	Nintendo	2013	
Gran Turismo 6	PS3	Nintendo	2013	
The Legend of Zelda: A Link Between Worlds	3DS	Nintendo	2013	
FIFA 14	PS4	Nintendo	2013	
Call of Duty: Ghosts	XOne	Nintendo	2013	
Assassin's Creed IV: Black Flag	PS4	Nintendo	2013	



3. Copy paste je gemaakte SQL query hieronder

127.0.0.1/mod-mysql-advanced-videogames-full/		http://localhost/phpmyadmin/index.php?route=/database/sql&db=mod-mysql-advanced-videogames-full

   Weergave van records 0 - 24 (440574 totaal, Query duurde 0,0007 seconden.)


SELECT game.name, genre.genre, game.year , game.global_sales FROM game
LEFT JOIN genre ON genre.id = genre.id
LEFT JOIN publisher ON publisher.id = publisher.id
WHERE genre.genre = "Puzzle"
AND game.year > 2000;


name	genre	year	global_sales	
Wii Sports	Puzzle	2006	8253	
Mario Kart Wii	Puzzle	2008	3552	
Wii Sports Resort	Puzzle	2009	3277	
New Super Mario Bros.	Puzzle	2006	298	
Wii Play	Puzzle	2006	2892	
New Super Mario Bros. Wii	Puzzle	2009	2832	
Nintendogs	Puzzle	2005	2467	
Mario Kart DS	Puzzle	2005	2321	
Wii Fit	Puzzle	2007	227	
Kinect Adventures!	Puzzle	2010	2181	
Wii Fit Plus	Puzzle	2009	2179	
Grand Theft Auto V	Puzzle	2013	2104	
Grand Theft Auto: San Andreas	Puzzle	2004	2081	
Brain Age: Train Your Brain in Minutes a Day	Puzzle	2005	2015	
Pokemon Diamond/Pokemon Pearl	Puzzle	2006	1825	
Grand Theft Auto V	Puzzle	2013	1627	
Grand Theft Auto: Vice City	Puzzle	2002	1615	
Pokemon Ruby/Pokemon Sapphire	Puzzle	2002	1585	
Brain Age 2: More Training in Minutes a Day	Puzzle	2005	1529	
Pokemon Black/Pokemon White	Puzzle	2010	1514	
Gran Turismo 3: A-Spec	Puzzle	2001	1498	
Call of Duty: Modern Warfare 3	Puzzle	2011	1473	
Call of Duty: Black Ops 3	Puzzle	2015	1463	
Call of Duty: Black Ops	Puzzle	2010	1461	
Pokemon X/Pokemon Y	Puzzle	2013	146	




4. Copy paste je gemaakte SQL query hieronder

127.0.0.1/mod-mysql-advanced-videogames-full/		http://localhost/phpmyadmin/index.php?route=/database/sql&db=mod-mysql-advanced-videogames-full

   Weergave van records 0 - 24 (6711624 totaal, Query duurde 0,0025 seconden.)


SELECT platform.platform , game.year , genre.genre , publisher.publisher , game.jp_sales FROM game
LEFT JOIN genre ON genre.id = genre.id
LEFT JOIN publisher ON publisher.id = publisher.id
LEFT JOIN platform ON platform.id = platform.id
WHERE game.name LIKE 'Mario%';


platform	year	genre	publisher	jp_sales	
Wii	2008	Sports	Nintendo	379	
Wii	2005	Sports	Nintendo	413	
Wii	2011	Sports	Nintendo	269	
Wii	1996	Sports	Nintendo	223	
Wii	2007	Sports	Nintendo	198	
Wii	2007	Sports	Nintendo	158	
Wii	2007	Sports	Nintendo	66	
Wii	2014	Sports	Nintendo	128	
Wii	2003	Sports	Nintendo	87	
Wii	2001	Sports	Nintendo	99	
Wii	2008	Sports	Nintendo	44	
Wii	2009	Sports	Nintendo	22	
Wii	2009	Sports	Nintendo	81	
Wii	2011	Sports	Nintendo	27	
Wii	2009	Sports	Nintendo	27	
Wii	2012	Sports	Nintendo	76	
Wii	1992	Sports	Nintendo	71	
Wii	1998	Sports	Nintendo	87	
Wii	2010	Sports	Nintendo	35	
Wii	2007	Sports	Nintendo	24	
Wii	1999	Sports	Nintendo	108	
Wii	2002	Sports	Nintendo	92	
Wii	2000	Sports	Nintendo	106	
Wii	1983	Sports	Nintendo	163	
Wii	2003	Sports	Nintendo	47	


5. Copy paste je gemaakte SQL query hieronder
   
127.0.0.1/mod-mysql-advanced-videogames-full/		http://localhost/phpmyadmin/index.php?route=/database/sql&db=mod-mysql-advanced-videogames-full

   Weergave van records 0 - 24 (6963048 totaal, Query duurde 0,0031 seconden.)


SELECT game.name , genre.genre , publisher.publisher , game.year FROM game
LEFT JOIN genre ON genre.id = genre.id
LEFT JOIN publisher ON publisher.id = publisher.id
LEFT JOIN platform ON platform.id = platform.id
WHERE platform.platform = 'PC';


name	genre	publisher	year	
Wii Sports	Sports	Nintendo	2006	
Super Mario Bros.	Sports	Nintendo	1985	
Mario Kart Wii	Sports	Nintendo	2008	
Wii Sports Resort	Sports	Nintendo	2009	
Pokemon Red/Pokemon Blue	Sports	Nintendo	1996	
Tetris	Sports	Nintendo	1989	
New Super Mario Bros.	Sports	Nintendo	2006	
Wii Play	Sports	Nintendo	2006	
New Super Mario Bros. Wii	Sports	Nintendo	2009	
Duck Hunt	Sports	Nintendo	1984	
Nintendogs	Sports	Nintendo	2005	
Mario Kart DS	Sports	Nintendo	2005	
Pokemon Gold/Pokemon Silver	Sports	Nintendo	1999	
Wii Fit	Sports	Nintendo	2007	
Kinect Adventures!	Sports	Nintendo	2010	
Wii Fit Plus	Sports	Nintendo	2009	
Grand Theft Auto V	Sports	Nintendo	2013	
Grand Theft Auto: San Andreas	Sports	Nintendo	2004	
Super Mario World	Sports	Nintendo	1990	
Brain Age: Train Your Brain in Minutes a Day	Sports	Nintendo	2005	
Pokemon Diamond/Pokemon Pearl	Sports	Nintendo	2006	
Super Mario Land	Sports	Nintendo	1989	
Super Mario Bros. 3	Sports	Nintendo	1988	
Grand Theft Auto V	Sports	Nintendo	2013	
Grand Theft Auto: Vice City	Sports	Nintendo	2002	
