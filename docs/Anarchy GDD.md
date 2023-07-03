# Anarchy GDD

## **Game Overview**

### **Appearance**

The battle royal takes place on various cities of Earth in its season 1. With every season the game settings changes, for its 2nd season the battle royal is going to take place on 

### **Story Abstract**

**Anarchy: Battle for the Universe** is a sci-fi battle royale game thousands of years in the future where time travel has been invented. In the game, players take on the role of different clans(species) from space and time to establish the most superior being and gain control of the universe. The battle takes place on Earth. Inspired by PUBG, the gameplay is fast-paced and challenging, with players needing to strategize and outsmart their opponents to come out as the ultimate winner.

### **Development Platform**

The requirements for playing Anarchy on a phone depend on the specific phone and operating system being used. However, generally speaking, Anarchy Mobile requires at least 2GB of RAM and a stable internet connection to play. It is also recommended to have a phone with a powerful processor and a high-quality display for the best gaming experience. It is important to check the specific requirements for your device before downloading and playing PUBG Mobile.

## **Game Mechanics**

This section discusses the game mechanics of Anarchy

### **Overview**

Anarchy is a TPS-style game. The player will play the game from either the 3rd person perspective. Anarchy is developed using Unity(LTS vers). For more information on the unity Engine, please go to [Unity - Manual: Unity User Manual 2022.3 (LTS) (unity3d.com)](https://docs.unity3d.com/Manual/index.html)

### **User Interface Design**

The user embodies an clan member in this Third Person Shooter (TPS). The conventions used will be similar to other games in the TPS  genre which a player will be familiar with such as battle royal & death match gameplays.

### **World**

The player will have access to different world according to the season. For season one the battle ground is Earth. The battle will take place in different maps according the game mode and maps selected.

### **Movement**

The player can move about the world using standard TPS conventions (more details in section 2.6, In-Game Control Summary). The player’s movement is constrained by buildings and objects in the world. Architecture will be used as puzzles, creating unique way to move from area to area.

### **Weapons**

The user can employ two weapons, which are selectable one at a time by the user.

1. MP5 – The MP5 is a submachine gun that fires 9x19mm Parabellum rounds. It is commonly used by military and law enforcement worldwide. The player gets 30 bullets with full bullet capacity of 1000.
2. M416 – M416 is a versatile assault rifle used in military/law enforcement. Fires auto/semi-auto modes, high accuracy, customizable.
3. Grande - The player gets a smoke and frag grenade.

### **Overall Description**

The user interface will be logically divided into two sections: the “Lobby” and the “in-game” areas. The user interface will be fairly simple, with a focus on making its use a quick and easy process.

The lobby menu will present multiple options to the player and allow the player to choose among the following options:

| Lobby options |  |
| --- | --- |
| Avatar | The player can select the avatar according to their preference clan |
| Weapons | The player can choose weapons, apart from the default option, at a price. |
| Clan | Clans represent different character options the player can choose from. |
| Leaderboard | The leaderboard shows the players’ rank and top preforming players. |
| Invite | The player can invite their friends. |
| Play | The player can start the gameplay based on the game mode and map selection. |
| Settings | The player can view and edit their account information and change graphics, controls, and audio options. |
| Game modes | The player can select different gameplays like battle royal, survival etc. |

The settings options panel, which allows changing of the screen resolution and audio settings. Once the play clicks the “Play” button on the main menu, the game will transition to the “in-game” user interface.

Upon transition to the in-game user interface, the player object and the environment will be displayed. The user will control the player throughout the game by using his smartphone screen much like the “standard” TPS (Third-person-shooter) controls in many games.

If the user presses the back button when playing the game, an in-game menu is displayed. This menu will allow the player to resume the game, quit to the main menu, or restart the area. Choosing the “restart area” option will be equivalent to dying; that is, the player will start over at the last checkpoint reached.

For the in-game interface, a “health bar” will be displayed near the bottom-left corner of the screen and will represent the current health of the player. Above this bar, small icons will represent the possible tools (weapons or items) that the user can choose from. The active tool will be highlighted. 

### **Key Screen Images**

This section contains proposed images for various parts of the in-game user interface.

**Image 1 – Main Title Screen**

![login_ui_image copy.jpg](..\static\img\login_ui_image_copy.jpg)

**Image 2 – Lobby Panel**

![Lobby2 Copy 2.jpeg](..\static\img\Lobby2_Copy_2.jpeg)

**Image 3 -** **Avatar selection**

![Avatar_selection.png](..\static\img\Avatar_selection.png)

**Image 4 - The settings**

![settings-v1.png](../../Anarchy GDD/settings-v1.png)

**Image 5 -** **In-Game User Interface**

![Ingame_UI_V003.jpg](..\static\img\Ingame_UI_V003.jpg)

### **State Transition Diagram**

The state transition diagram given here illustrates the progression of the user interface as the user performs certain actions. In general, the user will start at the lobby and begin the game. After the user decides to quit, the user will press the escape key and will choose the “Quit to Main Menu” option. Then, the user will exit the program from the main menu by choosing the “exit” button.

**Image 6 -** **State Transition Diagram**

![Wireframe_UI_Flow.jpg](..\static\img\Wireframe_UI_Flow.jpg)

### **Design Rules**

One of the goals of this project is to ensure a well-designed user interface that is easy to learn and use. Although the current design is fairly simple, it is still necessary to correct any usability issues to avoid user frustration. Therefore, the design of the user interface will be prototyped, tested, and redesigned as necessary.

Time constraints do not allow for formal usability testing outside the team, which will require that user interface evaluation be primarily carried out by team members. To strive for a more accurate evaluation of the user interface, all team members will test each revision to the user interface and give feedback to the designer, who will then make changes as appropriate.

The “Lobby” portion of the interface is created in similar style to other battle royal and survival games for player to easily adapt to it. The in-game player controls are designed to match the “standard” Third-person-shooter game controls as much as possible. Designing the user interface in this way will minimize learning time of users that have experience with other games.

**Specific User Interface Goals:**

- Intuitive (easy to learn)
- Consistent
- Intuitive Icon Images (if no text labeling is included)
- Intuitive Labeling for UI Components
- Simple (focus on helping the user play; avoid complexity that is “just for show”)

## Game modes

Game models represent different gaming environments with various challengers. We have the following game modes:

### 1. Death Match

Death Match is a game mode in which players compete against each other in a free-for-all style. The goal is typically to be the last player or team standing. In Anarchy, the death match is played on a smaller map with a limited number of players. Players start with basic weapons and equipment and must scavenge for better gear as they fight to survive. The game usually has a time limit or a set number of kills required to win.

### 2. Mission

In Anarchy, the mission game mode involves players completing a series of objectives within a designated area. The objectives can vary from game to game, but typically involve collecting items or defeating enemies. The game is played on a larger map than the death match mode, with a larger number of players. Players start with basic weapons and equipment and must scavenge for better gear as they complete objectives and fight against other players. The game usually has a time limit or a set number of objectives required to win. The gameplay mechanics and rules in Anarchy's mission mode are similar to those in other battle royale games.

### 3. Battle Royale

In Anarchy, the Battle Royal game mode involves players competing against each other in a free-for-all style. The goal is to be the last player or team standing. The game is played on a larger map with a larger number of players compared to the death match mode. Players start with basic weapons and equipment and must scavenge for better gear as they fight to survive. The gameplay mechanics and rules in Anarchy's Battle Royal mode are similar to those in other Battle Royale games.

# **Artificial Intelligence**

This section describes how the artificial intelligence works and how the player interacts with the AI.

### **Opponent AI**

The opponent AI are armed with guns (ranged weapons):

### **Player Detection**

Players are detected when a player comes under certain radius.

### **Visual**

The AI scans for the player where all three checks have to succeed:

- The player is within visual range (distance)
- The player is within the AI’s Field of View
- No terrain, buildings, or objects are directly between the player and the AI

## Maps

### Survival

The survival map in Anarchy is a challenging and engaging environment for players to explore and fight over. It features a large, open world with a variety of terrain and structures. The player must scavenge for weapons and equipment to survive and defeat other players. The map is denoted by red and purple hues, and architecture is used as puzzles, creating unique ways to move from area to area.

![Battle_Royale_Open_World_V001.jpeg](..\static\img\Battle_Royale_Open_World_V001.jpeg)

### Mission map

In Anarchy, the mission mode involves completing objectives in a designated area. Players start with basic weapons and must scavenge for better gear as they complete objectives and fight against other players. The mission map is designed to be challenging and engaging with strategic locations and structures. Gameplay mechanics are similar to other battle royale games.

![mission.png](..\static\img\mission.png)

### **Battle Royale**

The Battle Royale map in Anarchy is similar to other games in the genre It features a large, open world with a variety of terrain and structures for players to explore and fight over. The map is designed to be challenging and engaging, with strategic locations and hide out places for players to discover. Players start with basic weapons and equipment and must scavenge for better gear as they fight. The gameplay mechanics and rules in Anarchy's Battle Royale mode are similar to those in other Battle Royale games.

![MapRender_names_v2.jpg](..\static\img\MapRender_names_v2.jpg)

## **Wow Factor**

The player should be fascinated with the look and feel of the alien worlds and the visual/audio effects in the game. The main clans, should stick in the players mind, since there was considerable effort to make the clans and the maps.

## Anarchy tech stack

The below image represents the tools we have use at Anarchy. 

![Techstack.jpg](..\static\img\Anarchy_Tech_Stack_v3 copy (1).jpg)