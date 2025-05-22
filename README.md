# Codex
World of Warcraft (1.12) addon which displays mob spells on mouseover.

## Disclaimer
The data reflected by this addon is based on brotalnia's database (`world_full_08_february_2019`).
Depending on the server you are playing, this addon may report incorrect information and custom content will not be supported for this exact reason.

## Spell information
- Name (ex: Fireball)

## Technical Notes
Spell descriptions have different placeholders which need to be replaced with the proper values. Here is how I processed each of them for this addon:

| Placeholder | Formula |
| ------------- | ------------- |
| a1 | effectRadiusIndex1 passed to SpellRadius.dbc |
| d | durationIndex passed to SpellDuration.Dbc, then divide by 1000 |
| e1 | effectMultipleValue1 |
| g | Evaluated in Lua depending on character gender |
| h | procChance |
| i | maxAffectedTargets |
| l | Evaluated depending on the quantity |
| m1 | effectBasePoints1 + 1 |
| n | procCharges |
| o1 | (effectBasePoints1 + 1) * (duration/effectAmplitude1) |
| o2 | (effectBasePoints2 + 1) * (duration/effectAmplitude2) |
| r1 | effectRadiusIndex1 passed to SpellRadius.dbc |
| s1 | effectBasePoints1 + 1 |
| s2 | effectBasePoints2 + 1 |
| s3 | effectBasePoints3 + 1 |
| t1 | effectAmplitude1/1000 |
| t2 | effectAmplitude2/1000 |
| t3 | effectAmplitude3/1000 |
| x1 | effectChainTarget1 |
