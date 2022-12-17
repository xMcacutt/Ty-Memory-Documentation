## Ty-KoalaKid-Documentation

### Koala Kid Objective

To me, the koala kid objective structure makes no sense whatsoever just by looking at the memory addresses.
There are pointers scattered everywhere and it is exceptionally difficult to work out where the object starts and ends.

### Koala Kid

The Koala Kid object is 0x518 bytes long.
The first Koala Kid is always located at [Module Base + 0x26B070] + 0

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x14|Int32|Object ID|Defined In LV2|
|0x44|Bool|bVisible|Changed During TA|
|0x26C|Int32|Koala Index|\*\*|
|0x298|Bool|bCollisionActive||
|0x2A4|Float[]|Position Coordinates XYZ||
|0x2B4|Float[]|Rotation Coordinates PYR||

\*\*Koala Index is based on the order of the Koalas in the LV2. Specifically, the index counts from 1 to 8 (typically) in reverse order from the order listed in the LV2.

Koala Kids are always created in the same order
KATIE -> MIM -> ELIZABETH -> SNUGS -> GUMMY -> DUBBO -> KIKI -> BOONIE

This means for levels with multiple of the same Koala, the two duplicates will be next to each other in memory.

For Mul-Ty-Player, the first koala of each type is always the one placed at the bottom of the LV2
