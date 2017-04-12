
Answers

Find all the robots from The Hitchhiker's Guide to the Galaxy.
SELECT * FROM robots WHERE source LIKE '%Guide%';


#Find the robot with an "anxious" personality.
SELECT * FROM robots WHERE personality = 'anxious';


Find all recipes that are nut free.
SELECT * FROM recipes WHERE nut_free = 't';

Count the number of recipes that are gluten free but not vegetarian.
intro_to_sql=# SELECT COUNT(name) FROM recipes WHERE (gluten_free = 't') AND (vegetarian  = 'f');


Find the animal with the most legs.
intro_to_sql=# SELECT * FROM animals ORDER BY number_of_legs DESC;

Find the board game that takes the least amount of time to play.
intro_to_sql=# SELECT * FROM board_games ORDER BY mins_to_play ASC;

Find the recipe that takes the most time to prepare.
intro_to_sql=# SELECT * FROM recipes ORDER BY minutes_required;


Find all the robots whose name starts with the letter M.
intro_to_sql=# SELECT * FROM robots WHERE name LIKE 'M%';


Count the number of board games that can be played by 8 people.
intro_to_sql=# SELECT * FROM board_games WHERE max_players >= 8;

Find all animals that are swimming and egg-laying.
intro_to_sql=# SELECT * FROM animals WHERE (swimming = 't') AND (egg_laying = 't');

Find all animals that are swimming and egg-laying but not flying.
intro_to_sql=# SELECT * FROM animals WHERE (swimming = 't') AND (egg_laying = 't') AND (flying = 'f');


Find the board game that supports the largest number of people.
intro_to_sql=# SELECT MAX(max_players) FROM board_games;





