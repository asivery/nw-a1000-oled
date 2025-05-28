# A replacement display for the NW-A1000 Network Walkman

![Photo of a device with a working screen.](https://github.com/asivery/nw-a1000-oled/blob/master/res/photo.png?raw=true)

## How it works

Since the Sony NW-A1000 uses an obsolete SSD1328U1-based screen, to make it work with a generic SSD1327 screen I had to patch the firmware.

There's, of course, no new screens available with that exact pinout, so I designed a flex PCB which simply translates the pin layout to the one used by new OLEDs.

[Here](https://aliexpress.com/item/1005006480988390.html)'s the screen I used.

## How to patch?

1. Download the official Sony upgrade tool for the NW-A1000, and start it with the walkman unplugged.
2. Once you see this window, open task manager.

![Connect the device to update the software.](https://github.com/asivery/nw-a1000-oled/blob/master/res/sc01.png?raw=true)

3. Open task manager, find `FWUpdater.exe`, right click, select `Open file location`. Then copy all the files to somewhere on your desktop.

![Open file location](https://github.com/asivery/nw-a1000-oled/blob/master/res/sc02.png?raw=true)

4. Go to [my patching site](https://asivery.github.io/NW-A1000/), and provide it the `ver3.00/NW_A1000.UPG` file from that folder.
5. Download the new file, delete all files in `ver3.00` and replace them with the one from my site.
6. Run the patcher and flash the Walkman.

## Is the NW-A1200 / NW-A3000 supported?

I don't know - I haven't tested them with this method, but probably.
