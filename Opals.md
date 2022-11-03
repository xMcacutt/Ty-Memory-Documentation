##

### B3 Crate
B3 crate data can be found in memory at the address pointed to by the value at the module base address + 0x255190

Crate data is 448 bytes long = 0x1C0

0x48 -> Crate state 

0 = Hidden

1 = Visible

If box has been broken, making it visible does not bring collision back. Otherwise it does.

### Normal Crate

B3 crate data can be found in memory at the address pointed to by the value at the module base address + 0x254CB8

Crate data is 448 bytes long = 0x1C0


|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x48|Bool|Crate Collision||
|0x114|Bool|Crate Visible||
|0x150 - 0x177|IntPtr[]|Opals||
|0x178|Byte|Opal Count||

