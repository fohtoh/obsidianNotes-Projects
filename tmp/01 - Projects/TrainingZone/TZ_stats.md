# Details
Building a webpage that will be able to hold the stats for tournaments played in the Training Zone.  
This will use a DynamoDB to hold the data.
Data entry and Data view will be handled through the NextJs app.


# Api
- /teams 
	- GET (gets a list of all the teams)
- /team
	- /{teamId}
		- GET (get a specific team)
		- PUT (update a team)
	- POST (add a new team)
- /players
	- GET (gets a list of all the players)
- /player
	- /{playerId}
		- GET (get a specific player)
		- PUT (update a player)
	- POST (add a new player)
- /teamMembers
	- GET (gets a list of all players on the given team)
- /games
	- GET (gets a list of all the games)
- /game
	- /{gameId}
		- GET (gets a specific game)
		- PUT (update a game)
	- POST (add a new game)

?Rename these to fit above?
deleteMember 
addMember

Fix API so that the stuff like TEAM# are not in the url.  Just do that in the database behind the scene
# Database design


# Stats to track
- **Points:** Total points scored by the player.
- **Field Goals:**
    - **Made/Attempted:** Tracks shooting efficiency.
    - **Percentage:** Calculated from the above.
- **Three-Pointers:**
    - **Made/Attempted:** Specific to shots beyond the arc.
    - **Percentage:** Reflects three-point shooting efficiency.
- **Free Throws:**
    - **Made/Attempted:** Indicates performance from the line.
    - **Percentage:** Free throw efficiency.
- **Rebounds:**
    - **Offensive Rebounds:** Securing the ball after a missed shot on offense.
    - **Defensive Rebounds:** Grabbing missed shots on defense.
- **Assists:** Passes that lead directly to a basket.
- **Steals:** Instances of taking the ball away from the opponent.
- **Blocks:** Shots deflected or stopped.
- **Turnovers:** Times the player loses possession.
- **Personal Fouls:** Number of fouls committed.
- **Minutes Played:** Time spent on the court, which can be used to normalize other stats.
- **Plus/Minus:** The point differential when the player is on the floor, giving insight into overall impact.
