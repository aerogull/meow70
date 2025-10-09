# Meow70
![render](https://hc-cdn.hel1.your-objectstorage.com/s/v3/e9d4dfca12c62388194c156511e3229996377a35_pcbbb.png)

## Building the Board
My idea started with how I wanted a split keyboard that wasn't ortholinear or ergo. So, I took a picture of my Keychron K6 Pro, and designed a split keyboard off of it. It runs on 2 Raspberry Pi Picos (or drop in replacements) with a simple, open case design and qmk firmware.\
This was a pretty difficult build, I ended up redoing the routing and placement several times, going from a staggered edge with the controllers mounted underneath, to what I have today. The most difficult part was doing the render of the keyboard (which is still a WIP, this is just temporary). My KICAD always gave me destroyed meshes that would take hours to import into any software. Once I finally got something imported, it took me 2 days of constantly doing little things and saving my work before blender crashed. The final render took over 8 minutes to finish, so it was quite an undertaking getting it to work.

## Bill of Materials
* 1x set of pcbs
* 2x Raspberry Pi Pico H
* 69x Kailh Hotswap Sockets (MX Style)
* 69x 1N4148 Diodes
* 69x MX-Style Switches
* 4x Plate-Mounted Stabilizers
* 2x 0.91" I2C PCB-Mounted OLED Displays
* 2x TRRS Audio Jack Connectors
* 8x M3 Screws
* 8x M3 Heatset Inserts

## More Photos
![schematic](https://hc-cdn.hel1.your-objectstorage.com/s/v3/861ee88085adb3ed38c9c139cd76bb08c1c6f49c_screenshot_2025-03-09_154452.png)
![pcb](https://hc-cdn.hel1.your-objectstorage.com/s/v3/4fb86ea1f16ce5646c4538d2c452d8ba963b1977_screenshot_2025-03-09_154533.png)
![case](https://hc-cdn.hel1.your-objectstorage.com/s/v3/6bef63617453d71a1472ec37ec80bc572794aa9b_screenshot_2025-03-09_155011.png)

## KICAD BOM (with prices for what I used)
|Id|Designator|Footprint|Quantity|Designation|Price Each|
|----|----|----|----|----|----|																																																																			
|1|"SW17	SW20	SW24	SW3	SW67	SW47	SW49	SW2	SW62	SW52	SW44	SW11	SW40	SW9	SW1	SW64	SW50	SW39	SW51	SW60	SW34	SW36	SW37	SW38	SW10	SW28	SW16	SW35	SW19	SW32	SW27	SW7	SW21	SW68	SW66	SW25	SW45	SW69	SW23	SW26	SW13	SW65	SW22	SW8	SW54	SW63	SW18	SW5	SW46	SW43	SW30	SW61	SW31	SW4	SW6	SW33	SW48	SW12"|"MX-Hotswap-1U"|58|"SW_Push"|$0.247|
|2|"SW53	SW15"|"MX-Hotswap-1.25U"|2|"SW_Push"|$0.247|
|3|"A1	A3"|"RaspberryPi_Pico_Common_THT_wModel"|2|"RaspberryPi_Pico"|$4.975|
|4|"SW42	SW14	SW41"|"MX-Hotswap-1.75U"|3|"SW_Push"|$0.247|
|5|"U2	U1"|"SSD1306-0.91-OLED-4pin-128x32"|2|"~"|$15.02|
|6|"SW56	SW29	SW57	SW55"|"MX-Hotswap-1.5U"|4|"SW_Push"|$0.247|
|7|"J2	J1"|"TENSILITY_54-00174"|2|"AudioJack4"|$1.865|
|8|"SW59	SW58"|"MX-Hotswap-2U"|2|"SW_Push"|$0.247|
|9|"D44	D54	D62	D55	D63	D69	D28	D52	D53	D45	D17	D9	D35	D12	D4	D31	D43	D18	D50	D26	D47	D33	D23	D39	D24	D7	D27	D48	D49	D58	D13	D32	D19	D57	D64	D30	D38	D8	D37	D68	D66	D20	D29	D60	D36	D15	D21	D2	D1	D10	D11	D61	D40	D56	D6	D25	D59	D34	D46	D16	D22	D67	D65	D42	D3	D51	D41	D5	D14"|"D_DO-35_SOD27_P7.62mm_Horizontal"|69|"1N4148"|$0.0644|

### What Else I Used
69 mx mechanical switches - gateron g pro 3.0 silvers ($0.455)\
69 keycaps (3D printed)\
8 heatset inserts - 97164A112 aluminium tapered for plastic ($1.15)\
4 stabilizers - divinikey tx ap stabs ($6.27)\
1 trrs cable ($17.18)\