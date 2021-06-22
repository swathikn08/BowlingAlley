# BowlingAlley
BowlingAlley
Bowling Alley
Assumptions:
1.	The game is started assuming there are 3 players in the lane.
2.	Once the lanes are assigned, no new players can be added.

API Details:
HTTP Method	API	Description
Get	/players	To get the details of all the Players
Get	layers/player-details/{player_id}	Get each player Details like name , allocated lane, Game ID
Get	players/{player_id}/scoreBoard	Get Player Score Board Details like , Current Score , Strikes, Spares
Post	players/addPlayer	Adds New Player, accepts a list of players and generates Game ID.
Put	players/update-player/{player_id}	Updates a Player
Delete	/players/delete-player/{player_id}	Deletes a player
Get	/players/assignLane	Assigns lane to the players, max 3players per lane
Get	/players/lanes	Returns the players for each lane
Get	/startGame/{gameid}	Starts the game

Functionality
1.	Add the Players.
2.	Assign lane to the players
3.	Start the Game
4.	Get the Score Board for each Player.

Sample Add player Request:
[
		{
			"name": "John"
		},
		 {
			"name": "James"
		},
		{
			"name": "Jack"
		},
		{
			"name": "Bob"
		},
		 {
			"name": "Jeff"
		}

	]
