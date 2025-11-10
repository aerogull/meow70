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
|Quantity|Item|Designation|Price Each|Total Price + Shipping|Link|
|----|----|----|----|----|----|
|69|"MX-Hotswap"|"SW_Push"|$0.138|$9.65|[here](https://www.aliexpress.us/item/3256807039037559.html)|
|2|"RaspberryPi_Pico_Common_THT_wModel"|"RaspberryPi_Pico"|$4|Provided by HackClub HQ!||
|2|"SSD1306-0.91-OLED-4pin-128x32"|"~"|$1.845|$3.69|[here](https://www.aliexpress.us/item/3256805967573053.html)|
|2|"TENSILITY_54-00174" (PJ-332)|"AudioJack4"|$0.234|$2.34|[here](https://www.aliexpress.us/item/3256807580272301.html)|
|69|"D_DO-35_SOD27_P7.62mm_Horizontal"|"1N4148"|$0.0174|$1.74|[here](https://www.aliexpress.us/item/3256806058794623.html)|
|69|MX Mechanical Switches|Gateron G Pro 3.0 Silvers|$0.345|$50.11|[here](https://www.gateron.co/products/gateron-g-pro-3-0-switch-set?variant=40479583043673)
|69|Keycaps|3D Printed (Cherry or DSA)|Printing Legion||[this](https://github.com/rsheldiii/KeyV2) or [this](https://github.com/anhthang/dsa-keycap)|
|8|Heatset Inserts|97164A112|$0.0574|$5.74|[here](https://www.aliexpress.us/item/3256805603102147.html)|
|4|Stabilizers|Gateron 2u Stabs|$2.547|$15.28|[here](https://www.aliexpress.us/item/3256805212136654.html)|
|1|TRRS Cable|Random Aliexpress Coiled TRRS Cable|$6.94|$6.94|[here](https://www.aliexpress.us/item/3256806811164725.html)|
|1|Full Case|4 Parts Split Up for Printing|Self or Printing Legion||[here](https://github.com/aerogull/meow70/tree/main/prod)|
|8|Screws|3mm 0.5x16mm|$0.345|$2.76|[here](https://www.lowes.com/pd/Hillman-3mm-0-5-x-16mm-Allen-Drive-Cap-Screws-4-Count/50088880)|
|5|Sets of PCBs|JLCPCB|$20.70 (for 5)|$55.95|[here](https://cart.jlcpcb.com/quote?orderType=1&homeUploadNum=360e6b78f3044f3bb4ea106e3b9b02fb&businessType=example&fileName=keyboardv2_364.2375x100.5mm_for_Default.zip)|

[link to step model of completed board](https://hc-cdn.hel1.your-objectstorage.com/s/v3/b98df7d8c57167f14ca20340c5cecc1c217099e2_full_assembly_para.step)