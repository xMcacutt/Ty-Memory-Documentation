# Ty-Save-Data-Documentation

The in game save data can be found in memory at the address pointed to by the module base address + 0x288730
This document explains what each offset from this address does.

## Save File Header

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x8|Byte|Saved Level ID||
|0xC|Byte|Percentage Completion||
|0xD|Byte|Total Thunder Egg Count||
|0xE|Bool|Hardcore||

## Level Data

### Rainbow Cliffs Z1

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x10|Byte|No. Times Entered|Two Up Portal Shown If > 1|
|0x11 - 0x14|Byte[]|Rainbow Scales|1 Bit Per Scale|
|0x15 - 0x1CF|Byte[]|Empty|Size Of 3 Levels' Data (probably unused)|

### Two Up A1

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x1D0|Byte|No. Times Entered|Display Game Info If > 0|
|0x1D1 - 0x1F6|Byte[]|Opals|1 Bit Per Opal|
|0x1F7|Byte|Padding||
|0x1F8 - 0x1FF|Bool[]|Thunder Eggs Collected||
|0x200 - 0x209|Bool[]|Cogs Collected||
|0x20A - 0x20E|Byte[]|Bilbies Collected|Last Bilby Collected Marked 3|
|0x20F|Byte|Padding||
|0x210 - 0x213|Float|Time Attack|Best Time Achieved|
|0x214 - 0x217|Float|Time Attack|Time To Beat|
|0x218 - 0x23F|Byte[]|Triggers Entered|EnterOnceOnly Activation (probably)|

### Walk In The Park A2

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x240|Byte|No. Times Entered|Display Game Info If > 0|
|0x241 - 0x266|Byte[]|Opals|1 Bit Per Opal|
|0x267|Byte|Padding||
|0x268 - 0x26F|Bool[]|Thunder Eggs Collected||
|0x270 - 0x279|Bool[]|Cogs Collected||
|0x27A - 0x27E|Byte[]|Bilbies Collected|Last Bilby Collected Marked 3|
|0x27F|Byte|Padding||
|0x280 - 0x283|Float|Time Attack|Best Time Achieved|
|0x284 - 0x287|Float|Time Attack|Time To Beat|
|0x288 - 0x2AF|Byte[]|Triggers Entered|EnterOnceOnly Activation (probably)|

### Ship Rex A3

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x2B0|Byte|No. Times Entered|Display Game Info If > 0|
|0x2B1 - 0x2D6|Byte[]|Opals|1 Bit Per Opal|
|0x2D7|Byte|Padding||
|0x2D8 - 0x2DF|Bool[]|Thunder Eggs Collected||
|0x2E0 - 0x2E9|Bool[]|Cogs Collected||
|0x2EA - 0x2EE|Byte[]|Bilbies Collected|Last Bilby Collected Marked 3|
|0x2EF|Byte|Padding||
|0x2F0 - 0x2F3|Float|Time Attack|Best Time Achieved|
|0x2F4 - 0x2F7|Float|Time Attack|Time To Beat|
|0x2F8 - 0x31F|Byte[]|Triggers Entered|EnterOnceOnly Activation (probably)|

### Bull's Pen A4

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x320|Byte|No. Times Entered|Spawn Portal In Z1 & Display Game Info If > 0|
|0x321 - 0x38F|Byte[]|Empty|Likely Populated With Data If Save Data Items Are Added To Level|

### Bridge On The River Ty B1

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x390|Byte|No. Times Entered|Display Game Info If > 0|
|0x391 - 0x3B6|Byte[]|Opals|1 Bit Per Opal|
|0x3B7|Byte|Padding||
|0x3B8 - 0x3BF|Bool[]|Thunder Eggs Collected||
|0x3C0 - 0x3C9|Bool[]|Cogs Collected||
|0x3CA - 0x3CE|Byte[]|Bilbies Collected|Last Bilby Collected Marked 3|
|0x3CF|Byte|Padding||
|0x3D0 - 0x3D3|Float|Time Attack|Best Time Achieved|
|0x3D4 - 0x3D7|Float|Time Attack|Time To Beat|
|0x3D8 - 0x3FF|Byte[]|Triggers Entered|EnterOnceOnly Activation (probably)|

### Snow Worries B2

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x400|Byte|No. Times Entered|Display Game Info If > 0|
|0x401 - 0x426|Byte[]|Opals|1 Bit Per Opal|
|0x427|Byte|Padding||
|0x428 - 0x42F|Bool[]|Thunder Eggs Collected||
|0x430 - 0x439|Bool[]|Cogs Collected||
|0x43A - 0x43E|Byte[]|Bilbies Collected|Last Bilby Collected Marked 3|
|0x43F|Byte|Padding||
|0x440 - 0x443|Float|Time Attack|Best Time Achieved|
|0x444 - 0x447|Float|Time Attack|Time To Beat|
|0x448 - 0x46F|Byte[]|Triggers Entered|EnterOnceOnly Activation (probably)|

### Outback Safari B3

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x470|Byte|No. Times Entered|Display Game Info If > 0|
|0x471 - 0x496|Byte[]|Opals|1 Bit Per Opal|
|0x497|Byte|Padding||
|0x498 - 0x49F|Bool[]|Thunder Eggs Collected||
|0x4A0 - 0x4A9|Bool[]|Cogs Collected||
|0x4AA - 0x4AE|Byte[]|Bilbies Collected|Last Bilby Collected Marked 3|
|0x4AF|Byte|Padding||
|0x4B0 - 0x4B3|Float|Time Attack|Best Time Achieved|
|0x4B4 - 0x4B7|Float|Time Attack|Time To Beat|
|0x4B8 - 0x4DF|Byte[]|Triggers Entered|EnterOnceOnly Activation (probably)|

### Kumu Caves B4 ?

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x4E0|Byte|No. Times Entered|Unused Level|
|0x4E1 - 0x54F|Byte[]|Empty|Likely Populated With Data If Save Data Items Are Added To Level|

### Lyre, Lyre Pants On Fire C1

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x550|Byte|No. Times Entered|Display Game Info If > 0|
|0x551 - 0x576|Byte[]|Opals|1 Bit Per Opal|
|0x577|Byte|Padding||
|0x578 - 0x57F|Bool[]|Thunder Eggs Collected||
|0x580 - 0x589|Bool[]|Cogs Collected||
|0x58A - 0x58E|Byte[]|Bilbies Collected|Last Bilby Collected Marked 3|
|0x58F|Byte|Padding||
|0x590 - 0x593|Float|Time Attack|Best Time Achieved|
|0x594 - 0x597|Float|Time Attack|Time To Beat|
|0x598 - 0x5BF|Byte[]|Triggers Entered|EnterOnceOnly Activation (probably)|

### Beyond The Black Stump C2

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x5C0|Byte|No. Times Entered|Display Game Info If > 0|
|0x5C1 - 0x5E6|Byte[]|Opals|1 Bit Per Opal|
|0x5E7|Byte|Padding||
|0x5E8 - 0x5EF|Bool[]|Thunder Eggs Collected||
|0x5F0 - 0x5F9|Bool[]|Cogs Collected||
|0x5FA - 0x5FE|Byte[]|Bilbies Collected|Last Bilby Collected Marked 3|
|0x5FF|Byte|Padding||
|0x600 - 0x603|Float|Time Attack|Best Time Achieved|
|0x604 - 0x607|Float|Time Attack|Time To Beat|
|0x608 - 0x62F|Byte[]|Triggers Entered|EnterOnceOnly Activation (probably)|

### Rex Marks The Spot C3

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x630|Byte|No. Times Entered|Display Game Info If > 0|
|0x631 - 0x656|Byte[]|Opals|1 Bit Per Opal|
|0x657|Byte|Padding||
|0x658 - 0x65F|Bool[]|Thunder Eggs Collected||
|0x660 - 0x669|Bool[]|Cogs Collected||
|0x66A - 0x66E|Byte[]|Bilbies Collected|Last Bilby Collected Marked 3|
|0x66F|Byte|Padding||
|0x670 - 0x673|Float|Time Attack|Best Time Achieved|
|0x674 - 0x677|Float|Time Attack|Time To Beat|
|0x678 - 0x69F|Byte[]|Triggers Entered|EnterOnceOnly Activation (probably)|

### Fluffy's Fjord C4

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x6A0|Byte|No. Times Entered|Spawn Portal In Z1 & Display Game Info If > 0|
|0x6A1 - 0x70F|Byte[]|Empty|Likely Populated With Data If Save Data Items Are Added To Level|

### MinMin D1

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x710|Byte|No. Times Entered|Unused Level|
|0x711 - 0x77F|Byte[]|Empty|Likely Populated With Data If Save Data Items Are Added To Level|

### Cass' Crest D2

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x780|Byte|No. Times Entered|Display Game Info If > 0|
|0x781 - 0x7EF|Byte[]|Empty|Likely Populated With Data If Save Data Items Are Added To Level|

### Neverwarm D3

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x7F0|Byte|No. Times Entered|Unused Level|
|0x7F1 - 0x85F|Byte[]|Empty|Likely Populated With Data If Save Data Items Are Added To Level|

### Crikey's Cove D4

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x860|Byte|No. Times Entered|Spawn Portal In Z1 & Display Game Info If > 0|
|0x861 - 0x8CF|Byte[]|Empty|Likely Populated With Data If Save Data Items Are Added To Level|

### Cass' Pass E1

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x8D0|Byte|No. Times Entered|Display Game Info If > 0|
|0x8D1 - 0x93F|Byte[]|Empty|Likely Populated With Data If Save Data Items Are Added To Level|

### Bonus World E2

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x940|Byte|No. Times Entered|Display Game Info If > 0|
|0x941 - 0x9AF|Byte[]|Empty|Likely Populated With Data If Save Data Items Are Added To Level|

### Bonus World E3

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x9B0|Byte|No. Times Entered|Display Game Info If > 0|
|0x9B1 - 0xA1F|Byte[]|Empty|Likely Populated With Data If Save Data Items Are Added To Level|

### Final Battle E4

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0xA20|Byte|No. Times Entered|Spawn Portal In Z1 & Display Game Info If > 0|
|0xA21 - 0xA8F|Byte[]|Empty|Likely Populated With Data If Save Data Items Are Added To Level|

## Rainbow Cliffs Objects

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0xA90|???|???||
|0xA91|???|???||
|0xA92|???|???||
|0xA93|???|???||
|0xA94|Bool|TE Machine Gone From Hub 1 To Hub 2|Also Displays Talisman|
|0xA95|Bool|Activated TE Machine Hub 1 ??|Not Sure What This Does|
|0xA96|Bool|Ice Wall Removed||
|0xA97|Bool|TE Machine Gone From Hub 2 To Hub 3|Also Displays Talisman|
|0xA98|Bool|Activated TE Machine Hub 2 ??|Not Sure What This Does|
|0xA99|Bool|Flaming Logs Removed||
|0xA9A|Bool|TE Machine Gone From Hub 3 to Hub 4?|Also Displays Talisman|
|0xA9B|Bool|Activated TE Machine Hub 3 ??|Not Sure What This Does|
|0xA9C|Bool|Smashrock Removed||
|0xA9D|Bool|TE Machine Gone From Hub 4|Also Displays Talisman|
|0xA9E|Bool|Activated TE Machine Hub 4 ??|Not Sure What This Does|
|0xA9F|Bool|E Zone Gate Open||
|0xAA0 - 0xAA3|???|???||

## Current Info

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0xAA4|Byte|Current Level ID||
|0xAA8|Byte|Previous Level ID||
|0xAAC|Byte|Current Hub|AKA Zone|
|0xAB0|Byte|Current Rang ID||

## Ty Attributes

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0xAB4|Bool|Learnt To Swim||
|0xAB5|Bool|Learnt To Dive||
|0xAB6|Bool|Got Second Rang||
|0xAB7|Bool|Got Extra Health|All Rainbow Scales|
|0xAB8|Bool|Got Boomerang||
|0xAB9|Bool|Got Frostyrang||
|0xABA|Bool|Got Flamerang||
|0xABB|Bool|Got Kaboomerang||
|0xABC|Bool|Got Doomerang||
|0xABD|Bool|Got Megarang||
|0xABE|Bool|Got Zoomerang||
|0xABF|Bool|Got Infrarang||
|0xAC0|Bool|Got Zappyrang||
|0xAC1|Bool|Got Aquarang||
|0xAC2|Bool|Got Multirang||
|0xAC3|Bool|Got Chronorang||

## Talisman & Hub Completion

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0xAC4|Bool|Got Talisman 1||
|0xAC5|Bool|Got Talisman 2||
|0xAC6|Bool|Got Talisman 3||
|0xAC7|Bool|Got Talisman 4||
|0xAC8|Bool|Got Talisman 5||
|0xAC9|Bool|Hub 1 Boss Complete||
|0xACA|Bool|Hub 2 Boss Complete||
|0xACB|Bool|Hub 3 Boss Complete||
|0xACC|Bool|Hub 4 Boss Complete|Shadow In Cass' Crest|
|0xACD|Bool|Final Battle Complete||

## Lives

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0xAD0-0xAD1|Int16|Life Count||

## Picture Frames

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0xAD2-0xB00|Byte[]|Picture Frames|1 Bit Per Frame|

## Misc

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0xB13|Byte|Last Played Cutscene ID||
|0xB14 - 0xB17|Int|Game Timer (Seconds)||
|0xB18|Byte|No. Enemies Bitten Up To 200|What Big Teeth You Have! Achv.|
|0xB1C|Byte|No. Enemies Zapped Up To 75|Tesla Time Achv.|
|0xB20|Byte|No. Enemies Flamed Up To 100|Nice & Toasty Achv.|
|0xB24|Byte|No. Skink Cricket Bats Burnt Up To 50|The Ashes Achv.|
|0xB28 - 0xB29|Bool[]|Cheats Used|Likely Switches To "Using Cheats" Leaderboards|
|0xB2A - 0xB2B|???|???|Related To Cheats Somehow|
|0xB2C|Byte|Skin ID||
