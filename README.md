### UE-fasttest

Initial task:
* Make basic inventory w/o UI
* Make lootable object that will be hold by inventory
* Make basic AI (w/o Behaviour Tree and EQS) that will move to custom map point
* Blueprint only

Made up at two parts - Guide-based inventory system with over needed functionality and self-made task required features.

First part bring some knowledge about WBP functionality and basic scheme of realization. In a nutshell pickup works like - Components for player and lootable, linetrace to check items, if found lootable -> button to loot -> make struct array record in player that contain component with info bringed by lootable -> destroy lootable. Button event to open UI which represent sorted struct array from player with some conditions like stack size, icon e.t.c

Second part was much simpler in case no need UI and no requirements to item struct. So, I decide to make lootable on overlap with player. In a nutshell - Player overlap lootable actor -> store looted data in struct array -> destroy lootable actor. On button event debug print name and count of picked items. As for AI from inital task, AI contorller and nav mesh, on begin play AI follow player and when reach him, walk around points that made with array of location value for better setup experience.      


Task took around 12h (with breaks) to learn and make own simplified version.
