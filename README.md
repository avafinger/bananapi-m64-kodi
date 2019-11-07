# Bananapi-m64 running kodi

This is a prebuilt Ubuntu 18.04 minimal image with mainline linux 5.2.0 to run Kodi.

Kernel features on BananaPi M64:

* cedrus (VPU)
* mali (GPU)
* hdmi
* hdmi-sound
* wifi
* eth 100 Mbps / Gbps
* ir
* v4l2
* i2c

Tested with  **Kodi 18.3 RC1**

Initial bootlog: https://gist.github.com/avafinger/17600cd3ef6014e3ad3d620a27ac5550

**Image for testing:**
https://github.com/avafinger/bananapi-m64-kodi/releases/tag/v1.0

# Kernel 5.3.1 (upgrade)

https://github.com/avafinger/bananapi-m64-kodi/releases/tag/v1.1

**NOTE**
The linux-image was re-uploaded to fix **DTB**

# Kernel 5.3.8 (update to run KODI again)

linux-image: https://github.com/avafinger/bananapi-m64-kodi/releases/tag/v1.2

There is a fix for the board version 1.2. 
Apply the fix from here:  https://github.com/avafinger/bananapi-m64-kodi/releases/tag/v1.3

# Kernel 5.3.9 (i2c)

linux-image: https://github.com/avafinger/bananapi-m64-kodi/releases/tag/v1.4

There is a fix for the I2C, tested with ssd1306
Testing SSD1306
![Testing SSD1306](https://github.com/avafinger//bananapi-m64-kodi/raw/master/ssd1306.gif)


# What works and what not (simple table)

This is a WiP (Work in Progress) and intended for testing purpose.


|  SBC Dev Board tested  |    BananaPi M64           |
|------------------------|---------------------------|
| KODI version           |      18.3 RC1             |
| kernel version         |       5.3.9 mainline      |
| gcc version            |       7.4.1               |
| display                |       hdmi                |
| graphical interface    |       CLI                 |
| KODI version           |      18.3-rc1             |
| idle Temp ºC / freq    |        45ºC *             |
| full Temp ºC / freq    |        75ºC *             |
| RAM memory usage (avg) |      85   Mbytes          |
| i2c                    |       ?                   |
| spi                    |       ?                   |
| Wifi                   |   brcmfmac                |
| BT                     |       no                  |
| ethernet               |       Gbps / 100Mbps      |
| sound                  |   hdmi-sound              |
| ir                     |      yes                  |
| linux-cedrus           |      yes                  |
| mali-utgard            |      Mali-400             |
|------------------------|---------------------------|
| issues                 |spdif and analog not works |
|                        |   Initial tests           |
|                        | Board shutdown (seems ok) |
|                        |   Thermal readout (fix)   |

Updates for Kernel 5.2.0
  * Thermal issues fixed
  * frequent rcu stall seems fixed
  
Issue:
  * analog sound
  * spdif sound
  * wlan0 works but is lazy to get IP from AP
  * Bluetooth
  

Kodi 18.3-rc1
![Kodi 2](https://github.com/avafinger/bananapi-m64-kodi/raw/master/kodi.jpg)  
