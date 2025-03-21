# Description

Manhunt is a multiplayer game mode divided where the Runners must beat the Ender Dragon and the Hunters must stop them.
This is an evolution of this principle in a new format with special attention to fairness, competitiveness and fun! 

# How to Play

### Prerequisites
- Install Forge version 1.19.4 -> https://files.minecraftforge.net/net/minecraftforge/forge/index_1.19.4.html

### Instructions
1. Download the mod from Releases on this same page
2. Put the mod in the mods/ folder
3. Load with Forge client
4. Start a server and invite players
5. Are you playing 1v1?
  - Yes:
    - Run the command: /Manhunt \<runner\> \<hunter\>
  - No:
    - Create teams using the built-in teams commands:
      - /team add \<teamName\>
      - /team join \<playerName\>  
    - Run the command: /Manhunt teams \<runnerTeam\> \<hunterTeam\>
6. Good luck and have fun!

# Want to look at the source code?
Just clone the repository!

# Rules

- All players start in the same area
- The Runners have a headstart of 30s, during which the Hunters are stunned
- The Runners win when the Ender Dragon dies, by any means
- The Hunters win when the Runners run out of time
  - When a Runner dies, 5 minutes are subtracted from the Runner's total time to complete the game
- Spawners of any kind cannot be broken

 # Mechanics

 ## Hunter's Compass

 The Hunters are equipped with a compass which allows tracking of any player, Runner or Hunter.
 - Using the compass tracks Runners
 - Holding shift whilst using the compass tracks other Hunters
 - The compass is enchanted when the currently tracked player is in the same dimension as the wielder and not enchanted otherwise
   - When the compass changes its enchantment state, the compass gives feedback via a sound cue
 - The compass is not dropped when a Hunter dies

## Player respawning

### Nether Portal respawning
When a player now dies, they may be able to respawn at the last entered Nether Portal, either in the Overworld or in the Nether.
This does not affect their set respawn point, created by a bed or a respawn anchor.

### Partial Keep Inventory
A player no longer loses their entire inventory when dying.  
Certain items such as tools and armor will be retained after respawning.

# All Commands
Use these commands to configure your manhunt game!

#### Starts a manhunt game between two players.
- /Manhunt \<runner\> \<hunter\>

#### Starts a manhunt game between two teams.
- /Manhunt teams \<runnerTeam\> \<hunterTeam\>

#### Change the amount of time for a given timer.
- /ManhuntTimer \<game\|headstart\|deathPenalty\|pause\> \<timeMinutes|timeSeconds\>

#### Pausing and Resuming
Can be called by an admin to pause the entire game.  
- /Manhunt pause
- /Manhunt resume

#### Stop the Manhunt
- /Manhunt stop
