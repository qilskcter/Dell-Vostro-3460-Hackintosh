# You can download my EFI at [releases](https://github.com/qilskcter/Dell-Vostro-3460-Hackintosh/releases) tab or clone this Repo

# Dell Vostro 3460 Hackintosh (Using Clover 5116)
## Supported macOS versions: High Sierra, Mojave, Catalina, BigSur (I don't think it's supported because I don't test. I just test this EFI on High Sierra and Mojave)
![Screenshot](Screenshots/HighSierra.png)
![Screenshot](Screenshots/Mojave.png)
## Laptop specs:

- Intel Core i3-3110M
- 4GB RAM
- Graphics: Intel HD4000 1366 x 768
- Wi-fi/Bluetooth card: Qualcomm Atheros AR9485
- Audio: Cx20590
- Ethernet: Qualcomm Atheros AR8161
- HDD: HGST HTS725050A7E630 500GB
## Working:
- Wifi 
- Audio
- Keyboard and Trackpad
- Headphone Jack
- Graphics
- Bluetooth
- Battery
- Native Power Management
- Something...

## Not working:
- Ethernet
- Sleep
- Something...
## Issues
- Trackpad settings are not showing (because my computer's battery is dead).
# How to use this EFI?
You download the macOS Mojave installer at [here](https://drive.google.com/file/d/1i8QDEaajCXy9L56oh5sEavWZ52wi4JnZ/view), then use MiniTool or other software to mount EFI, then use Explorer++ to access the EFI partition and then copy it.
# How to fix Wifi and Bluetooth?
- You go to Kext folder, you can see these kext: ATH9KInjector.kext, IO80211Family_ATH.kext, IOath3kfrmwr.kext
- Download Kext Droplet at [here](https://github.com/chris1111/Kext-Droplet) and then you put these kext in S/L/E (System/Library/Extensions) and Reboot.
