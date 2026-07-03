This a split keyboard that maintains most of the traditional layout of a standard keyboard.

69 total keys (nice)
4 programmable buttons (hardware macros :3)
2 layer switch buttons for even more keys (mmmmm function row)
USB-C connectivity (orph picos my beloved)
Dynamic master/slave (double the connectivity) 
TRRS cable connections (very sproingey)
2 128x32 OLED displays (2xBongo Cats not included)
Built in QMK (low latency for all the gamin)
VIA support (yk, unofficially)
Simple pcb shape (for making many many cases)
Hotswap keys (i'm thinking linears today, tactiles tomorrow)
Preconfigured out-of-the-box (some eeprom flashing required)

Everything was done by me, @aerogull.

Schematic:
    The schematic set up the basics for how the keyboard functions, outlining serial communication between the halves, setting up matricies, and i2c communication for the displays. Each key has it's own diode to prevent ghost taps and other crosstalk.

PCB Design:
    This was where the layout really mattered. I wanted to copy my existing keyboard, a keychron 60 percent, but make it split for easier transport and travel use. The macro keys were placed on the sides to help mirror the shape of the keyboard halves, allowing for more uniform cases and designs. 
Case:
    I went with a really simple and open layout for 2 reasons, I like the sound better, and I did not have an easy way to prototype test tolerences and fit. It was originally designed to be used with heatset inserts, but it ended up being easier to drive the screws directly into the plastic. The plate was made with ai03 plate-gen, but the stabs are the wrong kind so I had to dremel away some material to make them fit.
Firmware:
    QMK, pretty simple design with all the display hardcoded and eeprom flashing so you can't mess up where you plug the cord in. This firmware was developed in about 2 days or work, split across several years, so it went through some drastic changes. NKRO is enabled by default, and has unofficial via support included.
Render:
    Yay, blender! This was a lot of work trying to figure out why my mesh was in the GBs and why everything was a blog, but I think it turned out pretty good.
Build:
    I uh, didn't have any microcontroller headers, and broke something I only had one spare for so, It went about as good as it could go. It took about 9 hours of work to put it all together and get firmware tested and bug fixed.