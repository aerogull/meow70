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
|69|"MX-Hotswap"|"SW_Push"|$0.125|$16.74|[here](https://www.amazon.com/gp/product/B096WZ6TJ5?smid=A257ALKOU7JKIJ&psc=1)|
|2|"RaspberryPi_Pico_Common_THT_wModel"|"RaspberryPi_Pico"|$4|Provided by HackClub HQ!|[here](https://www.digikey.com/en/products/detail/raspberry-pi/SC0915/13684020)|
|2|"SSD1306-0.91-OLED-4pin-128x32"|"~"|$2.997|$17.26|[here](https://www.amazon.com/gp/product/B0F36YPH1W?smid=A3AG45GXH6FGYX&psc=1)|
|2|"TENSILITY_54-00174"|"AudioJack4"|$0.69|$1.38|[here](https://www.digikey.com/en/products/detail/tensility-international-corp/54-00174/12140150?s=N4IgTCBcDaIKwBYC0AGFBGA7AkBdAvkA)|
|69|"D_DO-35_SOD27_P7.62mm_Horizontal"|"1N4148"|$0.039|$10.22|[here](https://www.digikey.com/en/products/detail/onsemi/1N4148/458603)|
|69|MX Mechanical Switches|Gateron G Pro 3.0 Silvers|$0.345|$50.11|[here](https://www.gateron.co/products/gateron-g-pro-3-0-switch-set?variant=40479583043673)
|69|Keycaps|3D Printed (Cherry or DSA)|Printing Legion||[this](https://github.com/rsheldiii/KeyV2) or [this](https://github.com/anhthang/dsa-keycap)|
|8|Heatset Inserts|97164A112|$0.3492|$8.73 (+whatever mcmaster carr does for shipping)|[here](https://www.mcmaster.com/products/heat-set-inserts/tapered-heat-set-inserts-for-plastic-7)|
|4|Stabilizers|Divinikey TX AP Plate-Mount Stabs|$3.667|$29.80|[here](https://divinikey.com/products/tx-ap-stabilizers-rev-4?variant=40406837395521)|
|1|TRRS Cable|Random Amazon 1ft TRRS Cable|$4.99|$12.49|[here](https://www.amazon.com/gp/product/B083L982CM?smid=A1F4MO8CLOOQSY&th=1)|
|1|Full Case|4 Parts Split Up for Printing|Priting Legion||[here](https://github.com/aerogull/meow70/tree/main/prod)|
|8|Screws|3mm 0.5x16mm|$0.345|$2.76|[here](https://www.lowes.com/pd/Hillman-3mm-0-5-x-16mm-Allen-Drive-Cap-Screws-4-Count/50088880)|