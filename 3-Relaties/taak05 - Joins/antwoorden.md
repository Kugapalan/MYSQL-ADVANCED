# Antwoorden

1. Copy paste je gemaakte SQL query hieronder

   127.0.0.1/mod-mysql-advanced-videogames/game/		http://localhost/phpmyadmin/index.php?route=/database/sql&db=mod-mysql-advanced-videogames

   Weergave van records 0 - -1 (0 totaal, Query duurde 0,0005 seconden.)


SELECT * FROM game JOIN platform ON platform.id = game.platform_id;



1	Wii Sports	1	1	Wii	
3	Mario Kart Wii	1	1	Wii	
4	Wii Sports Resort	1	1	Wii	
8	Wii Play	1	1	Wii	
9	New Super Mario Bros. Wii	1	1	Wii	
14	Wii Fit	1	1	Wii	
16	Wii Fit Plus	1	1	Wii	
40	Super Smash Bros. Brawl	1	1	Wii	
50	Super Mario Galaxy	1	1	Wii	
62	Just Dance 3	1	1	Wii	
69	Just Dance 2	1	1	Wii	
80	Wii Party	1	1	Wii	
81	Mario Party 8	1	1	Wii	
87	Mario & Sonic at the Olympic Games	1	1	Wii	
98	Super Mario Galaxy 2	1	1	Wii	
104	Just Dance	1	1	Wii	
108	The Legend of Zelda: Twilight Princess	1	1	Wii	
117	Just Dance 4	1	1	Wii	
120	Zumba Fitness	1	1	Wii	
129	Donkey Kong Country Returns	1	1	Wii	
156	LEGO Star Wars: The Complete Saga	1	1	Wii	
210	Link's Crossbow Training	1	1	Wii	
231	Animal Crossing: City Folk	1	1	Wii	
235	Guitar Hero III: Legends of Rock	1	1	Wii	
238	Mario & Sonic at the Olympic Winter Games	1	1	Wii	

2. Copy paste je gemaakte SQL query hieronder

127.0.0.1/mod-mysql-advanced-videogames/game/		http://localhost/phpmyadmin/index.php?route=/table/sql&db=mod-mysql-advanced-videogames&table=game

   Weergave van records 0 -  9 (10 totaal, Query duurde 0,0007 seconden.)


SELECT * FROM game JOIN platform ON platform.id = game.platform_id WHERE game.id < 11;


id	name	platform_id	id	platform	
1	Wii Sports	1	1	Wii	
2	Super Mario Bros.	2	2	NES	
3	Mario Kart Wii	1	1	Wii	
4	Wii Sports Resort	1	1	Wii	
5	Pokemon Red/Pokemon Blue	3	3	GB	
6	Tetris	3	3	GB	
7	New Super Mario Bros.	4	4	DS	
8	Wii Play	1	1	Wii	
9	New Super Mario Bros. Wii	1	1	Wii	
10	Duck Hunt	2	2	NES	


3. Copy paste je gemaakte SQL query hieronder

127.0.0.1/mod-mysql-advanced-videogames/game/		http://localhost/phpmyadmin/index.php?route=/table/sql&db=mod-mysql-advanced-videogames&table=game

   Weergave van records 0 -  3 (4 totaal, Query duurde 0,0017 seconden.)


SELECT game.name , platform.platform FROM game JOIN platform ON platform.id = game.platform_id WHERE game.name = "Call of Duty: Advanced Warfare";


name	platform	
Call of Duty: Advanced Warfare	X360	
Call of Duty: Advanced Warfare	PS3	
Call of Duty: Advanced Warfare	PS4	
Call of Duty: Advanced Warfare	XOne	


4. Copy paste je gemaakte SQL query hieronder
   
127.0.0.1/mod-mysql-advanced-videogames/game/		http://localhost/phpmyadmin/index.php?route=/table/sql&db=mod-mysql-advanced-videogames&table=game

   Weergave van records 0 - 24 (930 totaal, Query duurde 0,0003 seconden.)


SELECT   platform.platform , game.name FROM game join platform WHERE game.name LIKE "FIFA%";


platform	name	
Wii	FIFA 16	
NES	FIFA 16	
GB	FIFA 16	
DS	FIFA 16	
X360	FIFA 16	
PS3	FIFA 16	
PS2	FIFA 16	
SNES	FIFA 16	
GBA	FIFA 16	
PS4	FIFA 16	
3DS	FIFA 16	
N64	FIFA 16	
PS	FIFA 16	
XB	FIFA 16	
PC	FIFA 16	
2600	FIFA 16	
PSP	FIFA 16	
XOne	FIFA 16	
WiiU	FIFA 16	
GC	FIFA 16	
GEN	FIFA 16	
DC	FIFA 16	
PSV	FIFA 16	
SAT	FIFA 16	
SCD	FIFA 16	


5. Copy paste je gemaakte SQL query hieronder

127.0.0.1/mod-mysql-advanced-videogames/game/		http://localhost/phpmyadmin/index.php?route=/table/sql&db=mod-mysql-advanced-videogames&table=game

   Weergave van records 0 - 123 (124 totaal, Query duurde 0,0008 seconden.)


SELECT    game.name , platform.platform  FROM game join platform WHERE game.name = "Borderlands" OR game.name = "Borderlands 2";


name	platform	
Borderlands	Wii	
Borderlands	NES	
Borderlands	GB	
Borderlands	DS	
Borderlands	X360	
Borderlands	PS3	
Borderlands	PS2	
Borderlands	SNES	
Borderlands	GBA	
Borderlands	PS4	
Borderlands	3DS	
Borderlands	N64	
Borderlands	PS	
Borderlands	XB	
Borderlands	PC	
Borderlands	2600	
Borderlands	PSP	
Borderlands	XOne	
Borderlands	WiiU	
Borderlands	GC	
Borderlands	GEN	
Borderlands	DC	
Borderlands	PSV	
Borderlands	SAT	
Borderlands	SCD	
Borderlands	WS	
Borderlands	NG	
Borderlands	TG16	
Borderlands	3DO	
Borderlands	GG	
Borderlands	PCFX	
Borderlands 2	Wii	
Borderlands 2	NES	
Borderlands 2	GB	
Borderlands 2	DS	
Borderlands 2	X360	
Borderlands 2	PS3	
Borderlands 2	PS2	
Borderlands 2	SNES	
Borderlands 2	GBA	
Borderlands 2	PS4	
Borderlands 2	3DS	
Borderlands 2	N64	
Borderlands 2	PS	
Borderlands 2	XB	
Borderlands 2	PC	
Borderlands 2	2600	
Borderlands 2	PSP	
Borderlands 2	XOne	
Borderlands 2	WiiU	
Borderlands 2	GC	
Borderlands 2	GEN	
Borderlands 2	DC	
Borderlands 2	PSV	
Borderlands 2	SAT	
Borderlands 2	SCD	
Borderlands 2	WS	
Borderlands 2	NG	
Borderlands 2	TG16	
Borderlands 2	3DO	
Borderlands 2	GG	
Borderlands 2	PCFX	
Borderlands 2	Wii	
Borderlands 2	NES	
Borderlands 2	GB	
Borderlands 2	DS	
Borderlands 2	X360	
Borderlands 2	PS3	
Borderlands 2	PS2	
Borderlands 2	SNES	
Borderlands 2	GBA	
Borderlands 2	PS4	
Borderlands 2	3DS	
Borderlands 2	N64	
Borderlands 2	PS	
Borderlands 2	XB	
Borderlands 2	PC	
Borderlands 2	2600	
Borderlands 2	PSP	
Borderlands 2	XOne	
Borderlands 2	WiiU	
Borderlands 2	GC	
Borderlands 2	GEN	
Borderlands 2	DC	
Borderlands 2	PSV	
Borderlands 2	SAT	
Borderlands 2	SCD	
Borderlands 2	WS	
Borderlands 2	NG	
Borderlands 2	TG16	
Borderlands 2	3DO	
Borderlands 2	GG	
Borderlands 2	PCFX	
Borderlands	Wii	
Borderlands	NES	
Borderlands	GB	
Borderlands	DS	
Borderlands	X360	
Borderlands	PS3	
Borderlands	PS2	
Borderlands	SNES	
Borderlands	GBA	
Borderlands	PS4	
Borderlands	3DS	
Borderlands	N64	
Borderlands	PS	
Borderlands	XB	
Borderlands	PC	
Borderlands	2600	
Borderlands	PSP	
Borderlands	XOne	
Borderlands	WiiU	
Borderlands	GC	
Borderlands	GEN	
Borderlands	DC	
Borderlands	PSV	
Borderlands	SAT	
Borderlands	SCD	
Borderlands	WS	
Borderlands	NG	
Borderlands	TG16	
Borderlands	3DO	
Borderlands	GG	
Borderlands	PCFX	
