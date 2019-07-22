<table><tr align = 'center'><td colspan = '2'>MalwareInvader</td></tr><tr><td>
Presents the main menu when player load into the game<br> 
Add the general background music and display the background image</td> 
<td>Phoenix3000<br>
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
Know the entities positions
</td>
<td></td></tr></table>

<table><tr align = 'center'><td colspan = '2'>Phoenix3000</td></tr><tr><td>
<!--Has all the states as entity<br>Initially has three lives and decrement one Whenever get shot<br>Move horizontally <br>Use KeyStroke to update position<br>Has physical signals and fire signals<br>Disappear when it get shot from malware app-->
Explosion effect and sound effects when it get shot from malware app<br>
Vibrate the phone when get shot<br>
sound effects when shooting the signal
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
<!--SuperMalware can decide when to appear randomly every 30 seconds. <br>SuperMalware tells MalwareInvader it's entity information. <br>Based on system controlled horizontal movements, update its positions in entities Show explosion effect when I get shot<br> -->
add Explosion effect, sound effect and vibrates the phone when get shot<br>
</td><td>Entities<br> MalwareInvader</td></tr></table>

<table><tr align = 'center'><td colspan = '2'>MalwareApp</td></tr><tr><td>
It can propose to MalwareInvader that it wants to fire. <br>
Based on confirmation signal sent by MalwareInvader, it fires the signal. <br>
Show MalwareExplosion effect, sound effect and vibrates the phone when get shot
</td><td>Signal <br> Entities<br>MalwareInvader
</td></tr></table>

<table><tr align = 'center'><td colspan = '2'>FireWall</td></tr><tr><td>
Stores and updates all the current block locations
within the wall, sent it to MalwareInvader<br>
</td><td>List of blocks
</td></tr></table>

<table><tr align = 'center'><td colspan = '2'>Block</td></tr><tr><td>
Explosion effect, sound effect and vibrates the phone when get hit<br>
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
