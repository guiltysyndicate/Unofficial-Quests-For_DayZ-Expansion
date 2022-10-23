**You will need to adjust the Loadout's for NPC's and the Quest rewards**

# Quest Naming Convention
---
The name of the quest files is arbitrary so I have mapped them out this way for ease of use, feel free to rename then however you want.

## Naming Convention Mapping
```
100 - Action Quests
200 - AiCamp Quests
300 - AiPatrol Quests
400 - AiVIP Quests ( These currently do not work, bug is known and should be addressed in the next Expansion Patch )
500 - Collection Quests
600 - Crafting Quests
700 - Delivery Quests
800 - Target Quests
900 - Travel Quests
1000 - TreasureHunt Quests
```

# How to use these Templates

## 1. Quests
---
Copy the Quest's that you want or all of them from ```chernarusplus\Profile\ExpansionMod\Quests\Quests\``` and paste/ftp them to your Expansion Quests directory ```(Profile or SC)\ExpansionMod\Quests\Quests\```.


## 2. Objectives
---
Copy the Objectives for the Quests that you pulled from step 1 from ```chernarusplus\Profile\ExpansionMod\Quests\Objectives\``` and paste/ftp them to your Expansion Objectives directory ```(Profile or SC)\ExpansionMod\Quests\Objectives\```.

## 3. Quest Objects
---
Copy the Quest Objects for the Quests that you pulled from step 1 from ```chernarusplus\mpmissions\(Your_MAP)\expansion\quests\objects\``` and paste/ftp them to your Expansion Quest Objects directory ```mpmissions\(Your_Map)\expansion\quests\objects```. If the directory does not exist, create it.

## 4. NPC's
---
If you are adding these quests to your existing setup, you will need to update the QuestNPC.json files in ```(Profile or SC)\ExpansionMod\Quests\NPCs\``` and include the Quest ID's from this repository.

```
    "QuestIDs": [
        200,
        300,
        400,
        401,
        500,
        501,
        502,
        503,
        504,
        505
    ],
```
If you are starting from scratch with your quest system, copy the NPC's from ```chernarusplus\Profile\ExpansionMod\Quests\NPCs\``` and paste/ftp them to your Expansion NPC's directory ```mpmissions\(Your_Map)\ExpansionMod\Quests\NPCs\```. **Note: These are the quest ID's for each quest under ```chernarusplus\Profile\ExpansionMod\Quests\Quests\``` and not the Objective ID's from ```chernarusplus\Profile\ExpansionMod\Quests\Objectives```** 

## 5. Loadouts
---
If there are Loadouts here that you want to incorporate into your existing setup, copy them from ```chernarusplus\Profile\ExpansionMod\Loadouts\``` and paste/ftp them to your Expansion Loadouts directory ```(Profile or SC)\ExpansionMod\Loadouts\```. To use them, add the Loadout file name to your Quest NPC under ```mpmissions\(Your_Map)\ExpansionMod\Quests\NPCs\```
```
        {
            "NPCLoadoutFile": "TraderGroup",
        }
```
or your Ai Patrols under ```mpmissions\(Your_Map)\expansion\settings\AIPatrolSettings.json```
```
        {
            "LoadoutFile": "UmbrellaLoadout",
        }
```        