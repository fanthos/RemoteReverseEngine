Aux AC remote

bits | usage | data
---- | ----- | ----
00-07 | magic? | 1100 0011
08-10 | wind scan | on: 111, off: 000
11-15 | temprature | 
16-31 | ? | 0101 0000 1001 0000
32-36 | timer time (hours) |
37-39 | wind speed | 1:011, 2:010, 3:001, 4:101
40-45 | timer time (minutes) |
46-46 | strong power |
47-49 | ? | 000
50-50 | sleep mode | on: 1
51-52 | ? | 00
53-55 | mode | 0: wind, 1: cold, 2: dry, 6: auto, 4: heat
56-63 | ? | 0000 0000
64-68 | add humid % |
69-73 | ? | 00000
74-74 | add humid en | on: 1
75-77 | ? | 001
78-78 | timer en | on: 1
79-87 | ? | 000000000
88-95 | ? button pressed |
96-103 | checksum |
Checksum is the sum mod 256 by adding each bytes.
