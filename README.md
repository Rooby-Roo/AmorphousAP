# AmorphousAP

This project contains all the custom files necessary to run Amorphous+ as a Manual game in Archipelago.

The game mod is distributed as a .xdelta patch. You will need an unmodified v2.1 version of the base game, and a patcher program. You can download the game [here](http://onemorelevel.com/static/games3/amorph.swf), and for the .xdelta patcher I use [this one.](https://www.romhacking.net/utilities/598) Simply patch your game with the patcher and then run it on the offline Flash Player of your choice. I use Adobe Flash Player 31, since I've had that on my computer for a while.

## How does this work? 

This guide assumes you know how to use the AP Manual system.

The AP win condition is to slay the Razor Queen at the end of a Huge nest. To beat this, this logically requires you to clear a Huge nest with every Gloople type enabled in the practice menu. It is possible to fight a Razor Queen in other nest sizes or in Bounty or Practice modes; only the Huge nest counts as an Archipelago victory.

This game is modified to have the in-game Award ribbons as checks. Each Award is a unique location. Some Awards have been excluded as locations for convenience (see FAQ below.)

As for AP items, you unlock each of the 12 Reward items, all 3 equipment slots, and the ability to enable certain Gloople types to spawn. At the game onset, only the default green Glooples are capable of spawning. Each organically-spawning, non-boss Gloople type is an item ("Spawn Clutters", "Spawn Grinders", etc). The ability for each of the progressive Gloople glom types (Oozle, Grey & Void Eater) is locked behind the "Spawn Gloople Fusions". The Biter glom is locked behind "Spawn Horrors". The different game modes are also items. At game start, only Small Nests are available to you. The ability to unlock Big and Huge nests are locked behind "Progressive Nest Size" and Bounty modes are locked behind "Progressive Bounty Speed".

To enable certain Gloople types to spawn, open the Practice menu and select the Glooples that you have the items for. Then, leave the practice menu, and select your game mode. Please note that as of now, the Boss Gloople buttons (Amalgam, Queen, Razor Queen) are non-functional outside of Practice mode. Additionally, only Oozle needs to be selected in order to enable all Gloople fusion types, making Gray and Void Eater buttons non-functional as well.

## FAQ

Q. Why did you exclude [Award]?  
A. Some Awards have been pre-cleared because they promote issues for AP synchronous play. Some checks are literally an idle game, some require going out of your way to die repeatedly, and some are just too grindy to be practical. The option to re-enable most of these checks is tabled for some future date in which Manual has YAML option support.

Q. Why are all the Gloople fusions one item?  
A. Blocking Gray fusions is proving to be extraordinarily difficult. Code won't behave. This is something I hope to dig deeper into at some later date. For now, you can enable all three Gloople fusions by selecting "Oozle" in the Practice menu.

Q. Why are you using v2.1 instead of v2.3?  
A. I literally didn't know v2.3 exists until after I started hacking. I'm not a Newgrounds regular. I hope to make this compatible with v2.3 at a later date.

Q. Why do I get a reward key and the D item slot shortly after I start playing?  
A. The game grants all item slots by faking the game into thinking it has more achievements than it really does. It's a couple short of 110, which is the number that gives the D item slot. You'll technically need to clear 4 or so Awards before you can use the slot, but being restricted on this is a rare enough of an occurance that I think it's acceptable.

Q. Why are there so many basic Glooples?  
A. A weird side effect of excluding certain Gloople types the easy way like I did. Game gets upset if you don't keep the Active Enemies list populated, so every time the game removes one, it replaces it with a Gloople. Currently looking into a better solution.

## TODO

> Test Boss Spawn blocking  

> Implement Progressive Gloople Fusion Spawns  

> Implement logic for max score and single-swing score to be fairer  

> Adjust logic for being able to crack grinders  

> Rename "Biter" Award

> Reassess validity of existing Award spread. Remove Unfortunate, Absentee? Add tier two fights?  

> "Level Unlocks" category adjustment
