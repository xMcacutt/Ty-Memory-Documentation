## Ty-KoalaKid-Documentation

### Koala Kid Objective

To me, the koala kid objective structure makes no sense whatsoever just by looking at the memory addresses.
There are pointers scattered everywhere and it is exceptionally difficult to work out where the object starts and ends.
Instead of worrying about this, I have simply used a consistent set of offsets for each koala which always work regardless of level.
The rest of this document only discusses the Koala Kid object itself.

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
