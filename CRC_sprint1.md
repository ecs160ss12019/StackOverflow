<table><tr align = 'center'><td colspan = '2'>MalwareInvader</td></tr><tr><td>Presents the main menu when player load into the game<br>When 'new game' in menu is selected, start a new game and create the basic structure of the main game including all entities ,scores,GUI <br>
Control the malware applications and supermalware to move or fire signal randomly <br>
Draws the game interface whenver states are updated <br>
Detect the collistion and call the corresponding exploision function of the exploded entity<br>
Increment the score when player shot the malware application <br>
Game is over when malware application reach the bottom of the screen or Phnoeix3000 run out of its lives</td>
<td>Phoneix3000<br>
MalwareApp<br>
FireWall<br>
SuperMalware<br>
GUI<br>
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
Initially has three lives and decrement one Whenever I get shot<br>
Move horizontally <br>
Use KeyStroke to update my position<br>
Has physical signals and fire signals<br>
Explode when it get shot from malware app<br>
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
Based on system controlled horizontal movements, update its postions in entities<br>
Show explosion effect when I get shot<br>
</td><td>Entities<br> MalwareInvader</td></tr></table>

<table><tr align = 'center'><td colspan = '2'>MalwareApp</td></tr><tr><td>
Based on system controlled horizontal or vertical movements, update its postions in entities <br>
Based on fire signal sent by MalwareInvader, fire the signal <br>
Show MalwareExplosion effect 
</td><td>Signal <br> Entities<br>MalwareInvader
</td></tr></table>

<table><tr align = 'center'><td colspan = '2'>Wall</td></tr><tr><td>
Store and update all the current block locations within the wall, sent it to MalwareInvader
</td><td>
List of blocks
</td></tr></table>>

<table><tr align = 'center'><td colspan = '2'>GUI of main game</td></tr><tr><td>set up the initial leth
left, right and fire button
</td><td></td></tr></table>>

