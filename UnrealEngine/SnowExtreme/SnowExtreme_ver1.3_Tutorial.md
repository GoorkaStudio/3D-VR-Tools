# How to create game in Unreal Engine 4.26 - SnowExtreme version 1.3

Game SnowExtreme Unreal Engine project with blueprints, models and maps. 
Playable version is avaliable on project site https://tajemnice-trzebini.pl

NOTE:
The game uses a third part assets which aren't included in this downloaded project due to legal restrictions. (source project use free assets and may look a litte diffrent)
Below are full game dependencies which can by bought on markeplace for about $50

## Tip 1
Don't do everything yourself.
Creating a game is a huge project, if you do it alone or in a small team use as many other works as possible.

## Game dependencies
- GoorkaStudio GameLogic version 1 - https://github.com/GoorkaStudio/3D-VR-Tools/blob/main/UnrealEngine/GameLogic/Version1/GameLogic-ver1.md
- Megascan - Quixel - https://quixel.com/
- Surface Trails - https://www.unrealengine.com/marketplace/en-US/product/surface-trails-with-snow-deformation-example
- Winter Forest Set - https://www.unrealengine.com/marketplace/en-US/product/winter-forest-set
- Runtime Files Downloader - https://marketplace-website-node-launcher-prod.ol.epicgames.com/ue/marketplace/en-US/product/runtime-files-downloader

## Project managment
1. For your game use "_YourProjectName" folder.  In your project you will be use many assets (Epic Starter, Megascan ...) don't move their location! Ue4 have strong refenerce and tools to rename and remove but this not work well in case of move directory.

![image](https://user-images.githubusercontent.com/54003204/148658692-bd063fd8-ccee-4246-aab5-f82070aac493.png)

2. Create folder for every type 
- Characters - parent directory for your's charactes (everyone in difrent subdirectory) ![image](https://user-images.githubusercontent.com/54003204/148658888-b3ee8dfa-9f09-447b-8f01-9ac248e96a4a.png)
- Maps - subdirectory for everyone map ![image](https://user-images.githubusercontent.com/54003204/148658906-83f0894e-71b6-4e97-a447-09139402a4ef.png)
- Sounds
- GameLogic
- UI

## Controls used
- GoorkaStudio/Checkpoint - change current game step when interacted. Used for menu and slalom.
- GoorkaStudio/Teleport - teleport player to destination. Used for restar map.

## Game steps
Avaliable step
![image](https://user-images.githubusercontent.com/54003204/148659314-df143654-43e5-4be2-8012-6bf923a044d9.png)

Init is used in start menu. The ame was publish on December 20, 2021, but the game's launch began on December 30, 2021 at 6 p.m. 
Init is the first setep in game, the in map Start Level Blueprint is checked if the game activation file is avalible.

Steps s1-s25 are use for slalom.

## Characters
Most of game logic is in character blueprints, there are 3 version of character. Each differ of physic and controls
![image](https://user-images.githubusercontent.com/54003204/148659601-dda31252-8f43-423f-bd9d-926e0dd37b3f.png)
### Version 1.1 
The game version 1.0 to 1.2 use: SnowboarderCharacterFast1_ver1_1, SnowboarderCharacterFast2_ver1_1.
This is a very simple version base on Parent class: Character with land movement mode : Walking and some 
![image](https://user-images.githubusercontent.com/54003204/148659843-9e00f211-0f8c-4ce6-99cc-39502119b0fc.png)

### version 1.3
The game version 1.3 use SnowboarderCharacter_ver1_3 witch use land movement mode : Flying and gravity and friction need to by calculated
![image](https://user-images.githubusercontent.com/54003204/148659910-00dea723-a5aa-4d84-b5aa-97f9053e03d8.png)

