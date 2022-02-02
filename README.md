# My Shared Compendia
A Foundry VTT module to share Data between worlds via compendia as explained by u/solfolango on r/FoundryVTT; [here](https://www.reddit.com/r/FoundryVTT/comments/fvw3c7/how_to_create_a_tiny_module_for_shared_content/ "here").
Its not hard to do, but you can jumpstart your efforts and just use this module.

## Installation
1.  Simply use the install module screen within the FoundryVTT setup

The deletion of line 68/69 shouldn be unnecessary if you installed after 27.4.2021 thanks to [BadIdeasBureau](https://github.com/BadIdeasBureau "BadIdeasBureau").<br/><br/>
But I strongly recommend you still read why the edit was necessary.

### Installation pre 27.4.2021

1.  Simply use the install module screen within the FoundryVTT setup
2.  Open you local My-Shared-Compendia/module.json
3.  Delete line 68 to 69

68   "download": "https://github.com/shirizaan/shared-compendia/releases/download/1.0.0/My-Shared-Compendia.zip",    
69   "manifest": "https://github.com/shirizaan/shared-compendia/releases/download/1.0.0/module.json"    


🚨 Whenever there is an update,  👏 FoundryVTT  👏 will  👏 erase  👏 your  👏 compendia 👏.

Therefore you want to prevent FoundryVTT to **ever** update this module.
 
Alternatively, and better, modify this to your own local and custom module. 

### Unlock your Compendia!

*Remeber*   that you need to unlock your compendia to add to them.  

Compendia are locked by default, because every change you manually did will be reverted on an update. Thats why you need to break the update function. 


## Default Setup
This module comes with 8 Default compendia. One for each Type of Entity that is [supported by FoundryVTT](https://foundryvtt.com/article/compendium/ "supported by FoundryVTT") and one extra "Actors".
- Bestiary ([Actor](https://foundryvtt.com/api/Actor.html "Actor"))
- Edges ([Item](https://foundryvtt.com/api/Item.html "Item"))
- Hindrances ([Item](https://foundryvtt.com/api/Item.html "Item"))
- Skills ([Item](https://foundryvtt.com/api/Item.html "Item"))
- Powers ([Item](https://foundryvtt.com/api/Item.html "Item"))
- Special Abilities ([Item](https://foundryvtt.com/api/Item.html "Item"))
- Scenes ([Scene](https://foundryvtt.com/api/Scene.html "Scene"))
- Journal Entries ([JournalEntry](https://foundryvtt.com/api/JournalEntry.html "JournalEntry"))
- Macros ([Macro](https://foundryvtt.com/api/Macro.html "Macro"))
- Roll Tables ([RollTable](https://foundryvtt.com/api/RollTable.html "RollTable"))
- Playlists ([Playlist](https://foundryvtt.com/api/Playlist.html "Playlist"))

## Customize
To change the default setup simple edit the module.json. All compendia are defined within the "packs" attribute beginning with line 10. 

Theres a sample for each possible compendium Entity - so start there.
Delete or change as you see fit and/or [fork](https://github.com/user/repository/fork) for your convenience.


### Classes, Feats or Features
There are no enteties for Classes, Feats, Features or anything more than the seven listed available in FoundryVTT. Best practices is to use the "[Item](https://foundryvtt.com/api/Item.html "Item")"  entity for those.

For Example:

    		{
    			"name": "feats",
    			"label": "My Feats",
    			"path": "packs/feats.db",
       "module": "My-Shared-Compendia",
    			"entity": "Item"
    		},
    		{
    			"name": "classes",
    			"label": "My Classes",
    			"path": "packs/classes.db",
       "module": "My-Shared-Compendia",
    			"entity": "Item"
    		},
    		{
    			"name": "class-features",
    			"label": "My Class Features",
    			"path": "packs/class-features.db",
       "module": "My-Shared-Compendia",
    			"entity": "Item"
    		}



## Dependencies
There a no known Dependencies.
But, [Compendium Folders](https://github.com/earlSt1/vtt-compendium-folders "Compendium Folders") is highly recomended.

❤

**I only intent to update this if it breaks. Anyway, delete line 67 to 70 in the module.json**

<img alt="GitHub all releases" src="https://img.shields.io/github/downloads/stschoelzel/My-Shared-Compendia/total">
