```
0000   1b 00 80 c7 83 14 0f c3 ff ff 00 00 00 00 09 00
0010   00 01 00 04 00 02 01 40 00 00 00 c0 81 24 00 63
0020   00 00 00 6b ff 00 00 73 00 00 00 7b ff 00 00 04
0030   ff 00 00 0c 00 00 00 14 ff ff 00 1c ff ff 00 24
0040   ff ff 00 2c ff ff 00 34 ca b4 80 3c d0 80 52 44
0050   d6 73 4b 4c d6 7d 55 54 d5 8a 61
```

```

0030   -- -- -- -- -- -- -- 14 ff ff 00 1c ff ff 00 24
0040   ff ff 00 2c ff ff 00 -- -- -- -- -- -- -- -- --
0050   -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- --
```

assuming, indexing is like:
- ff:ff:00 (yellow) - to 14 (Z) 
- ff:ff:00 (yellow) - to 1c (X) 
- ff:ff:00 (yellow) - to 24 (C) 
- ff:ff:00 (yellow) - to 2c (V) 

buttons colors send per line

first key code (1 byte) and color information (3 bytes) 

TODO: get keycodes for all buttons
## keymapping
- 6D - arrow left
- 75 - arrow down
- 7d - arrow right
- 14 - z
- 1c - x
- 24 - c
- 2c - v