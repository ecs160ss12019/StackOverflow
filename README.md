# StackOverflow
We plan to create the game 'Malware Invaders'.

## Game Objective
You are the antivirus program and you've been asked to protect the system from malware applications designed by Dr. Posnett and use physical signal to terminate those applications.

## The Team
- Karan Gupta: Cognitive Science with Computational Development, Junior.
- Zhiwei Zhang: Computer Science and Engineering, Junior.
- WaiYu Lam: Computer Science, Junior.
- Wenda Xu: Computer Science and Engineering, Junior.

## How Class Connect Each Other
  - First, when the game starts, the MIAPP application class calls the activity MainActivity.
  - MainActivity's onClick has two choices, either go to ActivityBoard or ActivitySetting
  - MainActivity initalize the Myservice class, which inialize the mediaplayer
  - In ActivityBoard, the onClick home button can go back to MainActivity
  - In ActivitySetting, sends the difficulty signal to MalwareInvaderAcitivity and calls it
  - In MalwareInvaderActivity, it initialize the MalwareInvader class, which initialize its sub-object classes(Phoenix3000, MalwareAppGroup, Firewall, Signal, SuperMalware, etc.) and the game thread, also it intialzie the SoundManager class
  - Many of the Object class are extends from anstract class Entities, since they share most of the same properties.
  - The MalwareInvader class initialize the onSingleTapListner, which helps detecting multi-touch
  - In MalwareAppGroup class, it initialzie the MalwareApp class
  - The Firewall class is constructed by the Block class
  - In MalwareInvader thread, when certain circumstances is fulfilled(the game ends), it jumps back to its parent MalwareInvaderActivity
  - When the game end, the MalwareInvaderActivity calls the Activity GameOverPop
  - GameOverPop onClick can either go to ActivitySetting or ActivityBoard
  
## Our design choices for this game 
  Our overall design for this game is a observer pattern. We have classes for all game objects such as player class , enemies class and so on. The whole game engine class "MalwareInvader.java" will handle the game state and notify these game object to update on their own. All the game object class will inherit from the sprite/entities class which holds the common state such as game object positions, image and so on. <br />
  In order to indicate different scenarios on our game, we use different activity class such as input activity, main activity , game activity and so on. We also use several refactoring to simplify our methods and classes. For example, we have different types of Malware app enemies and types of ammo they have. Instead of using the whole large class as blueprint of enemies, we extract the sub classes and put those extrinsic state of these object from their parent class. Also we have a signal/ammo interface and then we can delegate some behaviors to sub classes. We also designed a class to store the collections of different types of enemies. This helps us solve the data clumps problem as sometimes different parts of the code contain identical groups of variables. We turn these clumps into its own class. Moreover, we extracting our update method and draw methods. We let all the game object class has their own update method and draw method. Every game object will be responsible singly and our class would be less coupling.

   

## Link to Project Repository
https://github.com/ecs160ss12019/StackOverflow

## Link to storing mapping 
https://github.com/ecs160ss12019/StackOverflow/blob/master/StoryMapping.md

## Link to CRC for week1
https://github.com/ecs160ss12019/StackOverflow/blob/master/CRC_sprint1.md

## Link to CRC for week2
https://github.com/ecs160ss12019/StackOverflow/blob/master/CRC_sprint2.md

## Link to CRC for week3
https://github.com/ecs160ss12019/StackOverflow/blob/master/CRC_sprint3.md

## Link to Acceptance Criteria
https://github.com/ecs160ss12019/StackOverflow/blob/master/AcceptanceCriteria.md

## Current States and Screenshot of game 
https://github.com/ecs160ss12019/StackOverflow/blob/master/screenshot.pdf

