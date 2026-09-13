the player schema has a NN constraint on the date the player joins the team because it ensures that all players have a recorded time for when they joined the team
match_participants has NN for the player name, player number, and played time to ensure the inputted data cannot have a record of a player without having the stats of their presense in the match
match_modes has NN on match_id and mode_id because it does not have its own primary key and has a composite primary key from the foreign keys match_id and mode_id
