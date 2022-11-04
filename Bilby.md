# Ty-Bilby-Documentation

## Bilby Object

The current level bilbies can be found in memory at the address reached via pointer path: module base address + [0x2CEB8378] + [0] + 0
This document explains what each offset from this address does.

Each bilby uses 308 bytes. (0x134)

|Offset|Data Type|Definition|Extra Information|
|---|---|---|---|
|0x34|Int32|Bilby State||
|0x58|Bool|Cage Collision||

## Bilby State

|Value|Behaviour|Extra|
|---|---|---|
|0|Cage & Bilby Hidden||
|1|Normal Visible||
|2|Collecting||
|> 2|Broken||
