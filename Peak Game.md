Need: To improve hand eye coordination, reaction time, and fast input skills in people using a faced paced game that mixes a rhythm game and a platformer.

Problem Statement: Many people struggle with hand eye coordination, reaction time, and fast input skills, and my game will help improve those aspects. having to use multiple keys to manoeuvre around obstacles that are constantly moving and changing can help build skills and keep people entertained.

Skill Development: To develop the skills in Unity required to create the game, I would complete 2d platformer

Inputs: Movment keys (e.g WASD), jump key (space), dash key (shift). keybinds will likley be customisable

Processing: The program will check for collisions, or if the player has died, and will update the game accordingly, either updating player position or updating the game over screen. 

Outputs: The game will display the players position, or the game over screen

Transmission: The game will be single player with no need for online transmission

Storage: The game will store which levels the player has completed locally

User Interaction: Users will use keyboard inputs to control the character, being able to move around with WASD, jump with space, and dash with shift.

Core Gameplay: The player will be tasked with dodging attacks from enemys to the beat of a song, having to use the movement keys avalible to survive. If the player is hit to many times, they will die, and will have to restart from the beggining of the level.

Level Progression: The player will progress through levels, each one incresing in difficulty gardually as they go. There will also be boss levels, which will be a challenge for the player, combining the skills they have learnt throught the game into one difficult level.

Saving And Loading Data: The game will store what level the player has reached, so they dont have to restart the game every time they close it.

Performance Requirements: the game should be able to run at a stable 60fps on most windows devices and load in a short amount of time

Usabillity Requirments: All the menus should be easy to navigate, clearly showing what level the user is playing, although the gameplay will not be easy to follow, since unpredictability increases the difficulty, and trains the users reaction speed.

Compatibility Requirments: The game should be able to be played on any devie with a keyboard and mouse, and correct processing power.

Social and ethical stuff

Existing Idea
Plus
Minus
Implication
Just Shapes And Beats

The game is simple to follow, clearly indicating attacks, while also having simple controls. It has a clear progression and increase in difficulty, while still making it fun for the player.
The game is fairly short, and honestly, not too hard, only taking 10-25 attempts to beat even the hardest levels for your first time. It is also very simple in its art, with very little variation throughout the game.
In my game, i will have a good progression system, with clear difficulty progression and more levels for a longer game, yet my game will be much harder overall, while keeping the simple controls. It will also have a simple yet varying and unique artstyle to make each section feel new.

BEGIN Movement 
INPUT userInput 
IF 'A' pressed THEN 
Move player left 
ELSE IF 'D' pressed THEN 
Move player right 
ELSE IF 'Spacebar' or 'W' pressed THEN IF player touching ground THEN 
Move player 
END Movement

BEGIN Health
	Health = 3
	IF player hit by attack THEN
		Health - 1
	IF Health = 0 THEN
		Game over
END Health

BEGIN Level Progression
	WHEN player selects level THEN
		IF player doesn't have level unlocked THEN
			Don't enter level
		ELSE
			Enter level
			IF player touches endpoint THEN
				Save level as complete
				Unlock and move to next level
END Level Progression

BEGIN Data Saving And Loading
	WHEN level unlocked THEN
		Print data to save file
END Data Saving And Loading
