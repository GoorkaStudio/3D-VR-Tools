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
- Megascan - Quixel - https://quixel.com/
- Surface Trails - https://www.unrealengine.com/marketplace/en-US/product/surface-trails-with-snow-deformation-example
- Winter Forest Set - https://www.unrealengine.com/marketplace/en-US/product/winter-forest-set
- Runtime Files Downloader - https://marketplace-website-node-launcher-prod.ol.epicgames.com/ue/marketplace/en-US/product/runtime-files-downloader

## Project managment
1. For your game use "_YourProjectName" folder.  In jour project you will be use many assets (Epic Starter, Megascan ...) don't move their location! Ue4 have strong refenerce and tools to rename and remove but this not work well in case of move directory.

![image](https://user-images.githubusercontent.com/54003204/148658692-bd063fd8-ccee-4246-aab5-f82070aac493.png)

2. Create folder for every type 
- Characters - parent directory for your's charactes (everyone in difrent subdirectory) ![image](https://user-images.githubusercontent.com/54003204/148658888-b3ee8dfa-9f09-447b-8f01-9ac248e96a4a.png)
- Maps - subdirectory for everyone map ![image](https://user-images.githubusercontent.com/54003204/148658906-83f0894e-71b6-4e97-a447-09139402a4ef.png)

- Sounds
- GameLogic
- UI
