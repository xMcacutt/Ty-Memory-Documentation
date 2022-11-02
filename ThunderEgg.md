# Ty-ThunderEgg-Documentation

The current level Thunder Eggs can be found in memory at the address pointed to by the module base address + 0x270280
This document explains what each offset from this address does.

## Thunder Egg Object

Each portal uses 324 bytes. (0x144)

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x44 - 0x4F|Float[]|Position||
|0x64|Bool|???||
|0x65|Bool|???||
|0X70|Byte|???||
|0xC4|Byte|Thunder Egg State|Changing To != 2 Hides TE Permanently|
|0xDC - 0xE7|Float[]|Camera Source||
|0xEC - 0xF7|Float[]|Camera Target||
|0xFC - 0x107|Float[]|Camera Source|Repeated?|
|0x10C - 0x117|Float[]|Camera Target|Repeated?|