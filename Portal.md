# Ty-Portal-Documentation

The current level portals can be found in memory at the address pointed to by the module base address + 0x267408
This document explains what each offset from this address does.

## Portal Object

Each portal uses 176 bytes.

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x0|Byte|No. Bytes For Object|Always 176 (0xB0)|
|0x14 - 0x17|Int32|ID in lv2||
|0x94|Byte|Max Portal State?|Defined Later In Document|
|0x96|Byte|Starting Portal State?|Defined Later In Document|
|0x9C - 0x9F|Int32|Last Portal Function Call|Defined Later In Document|
|0xAC - 0xAF|Int32|Connecting Level|Defined Later In Document|

## Portal Function Calls

|Value|Behaviour|Extra Information|
|---|---|---|
|0|Remove Portal||
|1|Spawn Portal|Automatically Calls Function Value 2|
|2|Spawn Particles||
|3|Hide Portal||
|> 3|Portal Breaks|Exclaim Persists On Screen|

## Portal State

|Value|Visual|Interactable|Follows Camera|Lights Ty|Text Displayed|
|---|---|---|---|---|---|
|0|Nothing|NA|NA|NA|NA|
|1|Particles Only|No|NA|No|No|
|2|Nothing|NA|NA|NA|NA|
|3|Particles Only|No|NA|No|No|
|4|Portal Only|No|No|No|No|
|5|Portal & Particles|No|Yes|Yes|No|
|6|Portal Only|Yes|No|No|Yes|
|7|Portal & Particles|Yes|Yes|Yes|Yes|

## Connecting Level

Connecting Level ID defines which level the portal should lead to.
Changing this value also causes the text displayed on the portal to change.
This text pulls strings directly from Translations.[LANGUAGE] starting from Rainbow Cliffs.

This means that although the following IDs do apply to their connecting levels,
going past these values will cause the text on the portal to display strings from the translations text file.

Entering a portal with a connecting level that does not exist will cause a white load screen to appear and the game to crash.

|Level ID|Level Name|Level Code|Extra|
|---|---|---|---|
|0|Rainbow Cliffs|Z1||
|1|Rainbow Cliffs|Z2|Old Development Version|
|2|||
|3|||
|4|Two Up|A1||
|5|Walk In The Park|A2||
|6|Ship Rex|A3||
|7|Bull's Pen|A4||
|8|Bridge On The River Ty|B1||
|9|Snow Worries|B2||
|10|Outback Safari|B3||
|11||B4|Originally Kumu Caves|
|12|Lyre, Lyre Pants On Fire|C1||
|13|Beyond The Black Stump|C2||
|14|Rex Marks The Spot|C3||
|15|Fluffy's Fjord|C4||
|16||D1|Originally MinMin|
|17|Cass' Crest|D2|Originally No Man Groves|
|18||D3|Originally Neverwarm|
|19|Crikey's Cove|D4||
|20|Cass' Pass|E1|Originally The Gauntlet|
|21|Bonus World|E2||
|22|Bonus World|E3||
|23|Final Battle|E4||
