<table><tr align = 'center'><td colspan = '2'>MalwareInvader</td></tr><tr><td>
<!-- Presents the main menu when player load into the game<br> -->
When 'new game' in menu is selected, start a new game and create the basic structure of the main game including all entities ,scores,GUI <br>
Control the malware applications and supermalware to move or fire signal randomly <br>
Draws the game interface whenver states are updated
<!-- Detect the collistion and call the corresponding exploision function of the exploded entity<br> -->
Detect the collistion and disappear
<!-- Increment the score when player shot the malware application <br> -->
<!-- Game is over when malware application reach the bottom of the screen or Phnoeix3000 run out of its lives</td> -->
<td>Phoneix3000<br>
MalwareApp<br>
FireWall<br>
SuperMalware<br>
GamePage<br>
</td>
</tr>
</table>

<table><tr align = 'center'><td colspan = '2'>Entities</td></tr>
<tr><td>Know the entity's moves<br>
Know if the entity is destroyed<br>
Know the entitie's positions
</td>
<td></td></tr></table>

<table><tr align = 'center'><td colspan = '2'>Phoneix3000</td></tr><tr><td>
Has all the states as entity<br>
Initially has three lives and decrement one Whenever get shot<br>
Move horizontally <br>
Use KeyStroke to update position<br>
Has physical signals and fire signals<br>
Disappear when it get shot from malware app
<!-- Sprint2: Explode when it get shot from malware app<br> -->
</td><td>
Signal<br>
Entities<br>
KeyStroke<br>
</td></tr></table>

<table><tr align = 'center'><td colspan = '2'>Signal</td></tr><tr><td>
Move in direction that is specified <br>
Disappear when touches with block, SuperMalware, MalwareApp, Phoneix3000<br>
</td><td>
Phoneix3000 <br>
MalwareApp <br>
SuperMalware<br>
Block
</td></tr></table>

<table><tr align = 'center'><td colspan = '2'>SuperMalware</td></tr><tr><td>
Based on system controlled horizontal movements, update its postions in entities
<!-- Show explosion effect when I get shot<br> -->
Disappears when get shot<br>
</td><td>Entities<br> MalwareInvader</td></tr></table>

<table><tr align = 'center'><td colspan = '2'>MalwareApp</td></tr><tr><td>
Based on system controlled horizontal or vertical movements, update its postions in entities <br>
Based on fire signal sent by MalwareInvader, fire the signal
<!-- Show MalwareExplosion effect -->
Disappers when get shot<br>
</td><td>Signal <br> Entities<br>MalwareInvader
</td></tr></table>

<table><tr align = 'center'><td colspan = '2'>FireWall</td></tr><tr><td>
Stores and updates all the current block locations
within the wall, sent it to MalwareInvader<br>
</td><td>List of blocks
</td></tr></table>

<table><tr align = 'center'><td colspan = '2'>Block</td></tr><tr><td>
Stores four-corner coordinates<br>
</td><td></td></tr></table>

<table><tr align = 'center'><td colspan = '2'>Keystroke</td></tr><tr><td>
Stores and updates left, right and shoot variables based on user inputs<br>
</td><td></td></tr></table>

<table><tr align = 'center'><td colspan = '2'>MainPage</td></tr><tr><td>
Initialize the beginning page with options: "New Game", "Leaderboard" and "Sound On" <br>
With userInput "New Game" true, sent signal to MalwareInvader to set up the game page<br>
On NewGame page, When receives gameover signal from MalwareInvader, jumps to "Leaderboard" page<!-- With userInput "Leaderboard" true, draw the Leaderboard page, which contains a "back" button <br> --><!-- With userInput "Sound On" true, sound on <br> -->
<!-- On Leaderboard page, when "back" true, jumps to "New Game"  page <br> -->
</td><td>MalwareInvader</td></tr></table>

