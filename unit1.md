Modelling Justification
  A lot of the design decisions for the ERD were determined through the use of the information presented in the unit topics and descriptions 
  provided in the project setup document. To start, the schemas were determined from the themes provided and ordered accordingly. It was best
  to use the template provided and build from that frame of reference. The theme chosen was the Game Telemetry consisting of the schemas players,
  matches, match_participants, game_modes, match_modes, and score. With the schemas for the chosen theme selected, the next step was planning
  relevant attributes that makes sense for each schema based on personal experience playing sports, being on competitive sport teams, and 
  watching sport matches of different types. Personal experience gave the insight of players having attributes of name, player number, date they 
  were recruited, and information on their performance in terms of points and assists. The next schema is matches, when attributes of players who
  played in the match, the type of match it was, and the name for the match to identify it among others. Match_participants have attributes of 
  the players who attended the match. Most of its attributes pertains to the players as well as the time and date of the match. Game modes and match
  modes share common attributes due to their close similarity. The table describing the five roles was used to determine how the assign primary keys
  and foreign keys. Primary keys were assigned to players, matches, and game_modes using the provided information of what the actor, producer, and 
  catalog roles always have. This also assisted in giving the foreign keys to match_participants and match_modes. Understanding that match_modes serves
  as a junctions guided the decision to include the _id of match and mode as foreign keys. Every instance of an _id in each schema is set as an integer 
  because the key must be minimal and storing the data as an integer solidifies the data structure. Attributes on player name and match titles are set 
  as varchar because the stored information is better stored as string characters to keep the naming conventions consistent throughout the ERD. A few 
  attributes have not null constraints because its data stored without those information would prevent proper storage. The join date of players is set a 
  not null because it guarantees every player recorded are current members of the team. Other attributes with not null was done in preparation of the 
  relational algebra that will be incorporated later.

Reflection
  The platform used to create the ERD was https://dbdiagram.io/d. This site has similar syntax with examples provided in the unit topics but the set up 
  for referencing foreign key follow a different setup. Another decision that could likely differ from other designers is the choice in attributes for 
  the various schemas. A different designer would likely include less information on the players to focus on recording more details about the matches 
  in terms of the match location and attendance capacity of the stadiums used. Other designers could used another sport as a frame of reference for 
  determining their attributes. For instance, if the match was an ESPORTS event, there are varying characteristics that would make the ERD for the match 
  different from one made for futbol. The ERD made for this projects could potentially be useful for people who keep track of player performance in matches
  rather than wanting a general performance overview of the team during each match.
