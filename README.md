# Beyond Reach Knowledge Pack

A SkyrimNet world-knowledge pack for the Beyond Reach mod. Adds 346 entries across locations, quests, NPCs, and factions, with quest entries that adapt their narration to the player's current quest stage.
Every entry's condition_expr keys off Beyond Reach-specific factions (arnimapeople, ArnimaGuard, ArnimaOrcs, DivideGuard, etc.). So the Beyond Reach lore only injects for NPCs tagged with those factions. Vanilla Skyrim characters never see it in their prompts.

Features

66 locations

10 broad regional entries (Arnima, Evermore, Jehanna, Ol-Yernuk, The Divide, The Lowlands, The Outpost, Quarry Prison, The Grey)
56 specific sub-locations: caves, forts, shrines, watchtowers, hamlets, manors

61 quests across main, side, misc, Orc storyline, and radiant chains

56 use multi-branch Inja templates gated on get_quest_stage(editorID, false). The same entry reads differently before the quest starts, at each major beat, and after completion
{{ playerName }} interpolation throughout
condition_expr narrowed per quest to 3-7 relevant factions (Imperials see Malacath's March, beggars see Trickle Down, etc.) instead of flooding every Reach NPC with every quest

180 NPCs and 39 factions covering most major characters and groups in the mod

Requirements

Beyond Reach (and prerequisite worldspace mods)
SkyrimNet (duh)

Known gaps

3 quests left with flat (non-stage-gated) content because their FormIDs couldn't be auto-matched at build time: Defeat The Undead, Kill The Beast, Deliver the gold to Elritch

Source
Entries authored from the Beyond Reach wiki on https://tes-mods.fandom.com/wiki/Beyond_Reach
