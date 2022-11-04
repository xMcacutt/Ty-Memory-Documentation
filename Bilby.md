# Ty-Bilby-Documentation

UNFINISHED

## Bilby Cage

Bilbies and their cages are separate objects. As such, they should need to be handled separately.
However, hiding the bilby will also hide its cage. This can be utilised to avoid treating them separately.

The two will be documented separately here.

## Bilby Cage

The current level bilby cages can be found in memory at the address pointed to by the module base address + 
This document explains what each offset from this address does.

Each Thunder Egg uses 324 bytes. (0x144)

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x44 - 0x4F|Float[]|Position||
|0x64|Bool|???||
|0x65|Bool|???||
|0X70|Byte|???||
|0xC4|Byte|Thunder Egg State|Changing To 2 Hides TE Permanently|
|0xDC - 0xE7|Float[]|Camera Source||
|0xEC - 0xF7|Float[]|Camera Target||
|0xFC - 0x107|Float[]|Camera Source|Repeated?|
|0x10C - 0x117|Float[]|Camera Target|Repeated?|

## Bilby Object

The current level bilbies can be found in memory at the address pointed to by the module base address + [0x2CEB8378] + [0] + 0
This document explains what each offset from this address does.

Each Thunder Egg uses 324 bytes. (0x144)

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x44 - 0x4F|Float[]|Position||
|0x64|Bool|???||
|0x65|Bool|???||
|0X70|Byte|???||
|0xC4|Byte|Thunder Egg State|Changing To 2 Hides TE Permanently|
|0xDC - 0xE7|Float[]|Camera Source||
|0xEC - 0xF7|Float[]|Camera Target||
|0xFC - 0x107|Float[]|Camera Source|Repeated?|
|0x10C - 0x117|Float[]|Camera Target|Repeated?|

## Thunder Egg State

|Value|Behaviour|Extra|
|---|---|---|
|0|Nothing||
|1|Normal Visible||
|2|Permanently Hidden||
|3|Not Spinning||
|4|Spinning Fast|Used During Claim Anim|
|5|Hidden||
|> 5|Doesn't Follow Camera||

