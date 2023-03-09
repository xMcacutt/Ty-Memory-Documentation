## Ty-PictureFrame-Documentation

### InvisiCrate
Invisi crate data can be found in memory at the address pointed to by the value at the module base address + 0x254DB0

InvisiCrate data is 476 bytes long.

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x48|Bool|Crate Collision||
|0x114|Bool|Crate Visible|1: Visible, 2: Broken|
|0x150 - 0x177|IntPtr[]|Opals||
|0x178|Byte|Opal Count||

### Picutre Frame
