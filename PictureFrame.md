## Ty-PictureFrame-Documentation

### InvisiCrate
Invisi crate data can be found in memory at the address pointed to by the value at the module base address + 0x254DB0

InvisiCrate data is 476 bytes long.

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x48|Bool|Crate Collision||
|0x114|Bool|Crate Visible|1: Visible, 2: Broken|

### Picutre Frame

Picture Frame data is 216 bytes long
|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x88|Bool[4]|First always 0, second visible?, third collecting?, fourth collected?||
