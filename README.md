# Bananapi-m64 running kodi

This is a prebuilt Ubuntu 18.04 minimal image with linux 5.2.0-rc7 to run Kodi.

Kernel features on BananaPi M64:

* cedrus (VPU)
* mali (GPU)
* hdmi
* hdmi-sound
* wifi
* bt
* eth 100 Mbps / Gbps
* ir
* v4l2

Tested with  **Kodi 18.3 RC1**

Initial bootlog: https://gist.github.com/avafinger/17600cd3ef6014e3ad3d620a27ac5550

# What works and what not (simple table)

This is a WiP (Work in Progress) and intended for testing purpose.


|  SBC Dev Board tested  |    BananaPi M64           |
|------------------------|---------------------------|
| KODI version           |      18.3 RC1             |
| kernel version         |       5.2.0-rc7           |
| gcc version            |       7.3.0               |
| display                |       hdmi                |
| graphical interface    |       CLI                 |
| KODI version           | 19.0-alpha1 / 18.3-rc1    |
| idle Temp ºC / freq    |   40 ºC / ~120 Mhz   *    |
| full Temp ºC / freq    |   75 ºC / 1.15 GHz   *    |
| RAM memory usage (avg) |      75   Mbytes          |
| i2c                    |       ?                   |
| spi                    |                           |
| Wifi                   |   brcmfmac43430a0         |
| BT                     |       yes                 |
| ethernet               |       Gbps / 100Mbps      |
| sound                  |   hdmi-sound              |
| ir                     |      yes                  |
| linux-cedrus           |      yes                  |
| mali-utgard            |      Mali-400             |
|------------------------|---------------------------|
| issues                 |spdif and analog not works |
|                        |   Initial tests           |
