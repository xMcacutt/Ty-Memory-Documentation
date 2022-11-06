## Ty-Opal-Documentation

### Crates

#### B3 Crate
B3 crate data can be found in memory at the address pointed to by the value at the module base address + 0x255190

Crate data is 448 bytes long (0x1C0).

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x48|Bool|Crate Collision||
|0x114|Bool|Crate Visible||
|0x150 - 0x177|IntPtr[]|Opals||
|0x178|Byte|Opal Count||

If box has been broken, making it visible does not bring collision back. Otherwise it does.
Since the bushpig goes straight through the boxes, turning the box off visually also prevents it from being broken.
This means that, for the Outback boxes only, turning off the box visually is sufficient to remove the box.

#### Normal Crate

B3 crate data can be found in memory at the address pointed to by the value at the module base address + 0x254CB8

Crate data is 448 bytes long = 0x1C0

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x48|Bool|Crate Collision||
|0x114|Bool|Crate Visible||
|0x150 - 0x177|IntPtr[]|Opals||
|0x178|Byte|Opal Count||

___

### Opals

#### Gem Pointers

There are many places that live opal type objects (gems) are stored in memory.

The following all point to the first opal of that type in the current level. 

If that opal spec does not exist in the current level, the pointer path is invalid.

The paths can all be found using the same base address -> Module Base Address + [0x28AB7C]

This address is a pointer to an array of pointers for the different gems.

|Gem Type|Offset To Pointer|Hence Full Path|
|---|---|---|
|Opal (Not In Crate)|0x0|TY.exe + [0x28AB7C] + [0x0] + 0x0|
|Rainbow Scale|0x20|TY.exe + [0x28AB7C] + [0x20] + 0x0|
|B3 Crate Opal|0x2B0|TY.exe + [0x28AB7C] + [0x2B0] + 0x0|
|Normal Crate Opal|0x4AC|TY.exe + [0x28AB7C] + [0x4AC] + 0x0|

#### Opal Data

Opal data is 276 bytes long (0x114).

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x78|Int32|Opal State|Defined Later In Document|
|0xFE|Int16|???|Makes Opal Translucent If = 2 Or 3|
