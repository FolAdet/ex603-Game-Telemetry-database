Schemas: players. matches, match_participants, game_modes, match_modes


Attributes-

  players: 
  
    player_id int [primary key]
    name varchar
    jersey_number int
    joined_at date
    points int
    assit int
    
  matches:
  
    mactch_id  int [primary key]
    who_played varchar
    match_type varchar
    match_title varchar
    
  match_participants:
  
    match_participant_id int [primary key]
    player_id int
    match_id int
    player_name varchar
    player_number int
    played_time time
    occured_at date
    
  game_modes:
  
    game_modes_id int [primary key]
    game_type varchar
    length time
    number_of_players int
    
  match_modes:
  
    match_modes_id int 
    match_id int
    modes_id int
    game_type varchar
    length time
    number_of_players int
    
