## Keycode bytes for _side control knob button_ (near LED screen)

|          |    |    |        |        |        |        |
|----------|----|----|--------|--------|--------|--------|
| option 1 | 00 | 03 | **91** | **00** | **00** | **00** |
| option 2 | 00 | 03 | **91** | **00** | **00** | **01** |
| option 3 | 00 | 03 | **91** | **00** | **00** | **02** |
| option 4 | 00 | 03 | **91** | **00** | **00** | **03** |
| option 5 | 00 | 03 | **91** | **00** | **00** | **04** |
| option 6 | 00 | 03 | **91** | **00** | **00** | **05** |

### knob button pressed up sequence:

|              |    |    |        |        |
|--------------|----|----|--------|--------|
| key pressed  | 00 | 03 | **72** | **04** |
| ?            | 00 | 03 | **70** | **40** |
| key released | 00 | 03 | **72** | **00** |

### knob button pressed down sequence

|              |    |    |        |        |
|--------------|----|----|--------|--------|
| key pressed  | 00 | 03 | **72** | **01** |
| ?            | 00 | 03 | **70** | **40** |
| key released | 00 | 03 | **72** | **00** |

### knob button pressed middle sequence

|              |    |    |        |        |
|--------------|----|----|--------|--------|
| key pressed  | 00 | 03 | **72** | **02** |
| ?            | 00 | 03 | **70** | **40** |
| key released | 00 | 03 | **72** | **00** |

---

### knob button pressed up/down/middle

example data: 0x0003 7201

**0003** - knob keycode identifier

**72 [00, 01, 02, 04]** - button code
```
- 00 - no button
- 01 - down
- 02 - middle
- 03 - _unknown purpose, currently unused_
- 04 - up
```
0x7040 - internal keyboard communication? 

---

### knob button side-pressed 
```
example data: 0x0003 9100 0001 0000 (?)
```
0x0003 - knob button keycode identifier

**9100** - side press

0x _9100_ 000[X] - assuming X in range [0, 5].  
[0, 6] is carousel menu item. 0 is first in list, and 5 - the last item in list

### LED ? TODO INVESTIGATE 
```
example data: 0x0003 9200 0064 0000 (?)
- 0x0003 9200 0000 0000
- 0x0003 9200 0064 0000
- 0x0003 9200 004B 0000
```

