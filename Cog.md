# Ty-Cog-Documentation

The current level Cogs can be found in memory at the address pointed to by the module base address + 00270424
This document explains what each offset from this address does.

## Golden Cog Object

Each Cog uses 324 bytes. (0x144)

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x44 - 0x4F|Float[]|Position||
|0x64|Bool|???||
|0x65|Bool|???||
|0x6C|Int32|Cog ID|Indexed From 0|
|0X70|Byte|???||
|0xC4|Byte|Cog State|Changing To 2 Hides Cog Permanently|
|0xDC - 0xE7|Float[]|Camera Source||
|0xEC - 0xF7|Float[]|Camera Target||
|0xFC - 0x107|Float[]|Camera Source|Repeated?|
|0x10C - 0x117|Float[]|Camera Target|Repeated?|

## Cog State

|Value|Behaviour|Extra|
|---|---|---|
|0|Nothing||
|1|Normal Visible||
|2|Permanently Hidden||
|3|Not Spinning||
|4|Spinning Fast|Used During Claim Anim|
|5|Hidden||
|> 5|Doesn't Follow Camera||

