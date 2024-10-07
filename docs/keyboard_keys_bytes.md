
### keycode byte mapping
```
0x0003 7100 + [64-bit value for key combination]
- [0003 7100] + [0000 0000]
- [0000 0000 0000 0800]
- [0000 0000 0000 0800]
```
[0003 7100 ...] - alphanumeric key pressed

---
```
[0003 7100 0000 0000] 

[0000 0000 0000 0800] - letter k pressed (one key)
```
---
```
[0003 7100 0000 0000] 

[0000 0000 0000 0000] - no button pressed (one key)
```
---
```
[0003 7100 0000 0000] 

[0000 0000 0020 0000] - letter u pressed (one key)
```
---
```
[0003 7100 0000 0000] 

[0040 0000 0000 0000] - letter r pressed (one key)
```
---
```
[0003 7100 0010 0000] 

[0000 0000 0000 0000] - letter w pressed (one key)
```
---
```
[0003 7100 1000 0000] 

[0000 0000 0000 0000] - letter a pressed (one key)
```
---