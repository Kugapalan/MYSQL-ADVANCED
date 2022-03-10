# Antwoorden

1. Copy paste je gemaakte SQL query hieronder


SELECT game.name, platform.platform, genre.genre FROM game
LEFT JOIN platform ON game.platform_id = platform.id
LEFT JOIN genre ON game.genre_id = genre.id
WHERE game.name LIKE "b%";




   
2. Copy paste je gemaakte SQL query hieronder



SELECT game.name, platform.platform , publisher.publisher , game.year FROM game
LEFT JOIN platform ON game.platform_id = platform.id
LEFT JOIN genre ON game.genre_id = genre.id
LEFT JOIN publisher ON publisher.id = publisher.id
WHERE game.year = "2013";




3. Copy paste je gemaakte SQL query hieronder


SELECT game.name, genre.genre, game.year , game.global_sales FROM game
LEFT JOIN genre ON genre.id = genre.id
LEFT JOIN publisher ON publisher.id = publisher.id
WHERE genre.genre = "Puzzle"
AND game.year > 2000;




4. Copy paste je gemaakte SQL query hieronder


SELECT platform.platform , game.year , genre.genre , publisher.publisher , game.jp_sales FROM game
LEFT JOIN genre ON genre.id = genre.id
LEFT JOIN publisher ON publisher.id = publisher.id
LEFT JOIN platform ON platform.id = platform.id
WHERE game.name LIKE 'Mario%';



5. Copy paste je gemaakte SQL query hieronder
   


SELECT game.name , genre.genre , publisher.publisher , game.year FROM game
LEFT JOIN genre ON genre.id = genre.id
LEFT JOIN publisher ON publisher.id = publisher.id
LEFT JOIN platform ON platform.id = platform.id
WHERE platform.platform = 'PC';

