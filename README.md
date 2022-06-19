# <div align="center">Dell Vostro 3460 Hackintosh</div> 
## Bootloader versions

|OpenCore|Clover|
|--------|------|
|0.8.2|5146| 

## Supported macOS versions
- Mavericks
- Yosemite
- El Captain
- Sierra
- High Sierra
- Mojave
- Catalina
- Big Sur (Use SMBIOS ```MacBookPro11,5```)
- Monterey (OpenCore only. And patch iGPU with [Patch-HD4000-Monterey](https://github.com/chris1111/Patch-HD4000-Monterey) by [chris1111](https://github.com/chris1111)
## Screenshots

<div align="center">
  
![Screenshot](Screenshots/Monterey.png)
   
</div>
<details>
		<summary>Other OSes</summary>
      <br>
  
![Screenshot](Screenshots/Mavericks.png)
![Screenshot](Screenshots/HighSierra.png)
![Screenshot](Screenshots/Mojave.png)
![Screenshot](Screenshots/Catalina.png)
![Screenshot](Screenshots/BigSur.png)
  
</details>

## Laptop specs
 
|                     | Specifications| 
| ---------------------------- | ---------------------- |
| ``Chipset``| Intel Ivy Bridge |
| ``CPU``| Intel Core i3-3110M 2.40GHz |
| ``Memory``| 8GB DDR3-1600MHz |
| ``GPU``| Intel HD Graphics 4000 |
| ``Disk 0``| SSD Lexar NS100 128GB |
| ``Disk 1``| HDD HGST HTS725050A7E630 500GB |
| ``Screen``| 14.0" 1366 x 768 |
| ``Ethernet``| Qualcomm Atheros AR8161 |
| ``WiFi and Bluetooth``| Intel® Dual Band Wireless-AC 7260 |
| ``Audio``| Conexant Cx20590 (alcid=14) |
| ``Keyboard``| Requied patching DSDT for brightness key |
| ``Touchpad``| Dell Touchpad (ALPS, PS/2) |
| ``Dimensions``| 30mm x 345.5mm x 244mm |
|``Weight``| 2.23kg | 
  
<div align="center">
  
![Screenshot](Screenshots/specs.png)
  
</div>

## Features


|                               | OpenCore             | Clover|
| ----------------------------- | -------------------- | ------------------|
| ``Wifi and Bluetooth``|✅|✅|
| ``Audio``|✅|✅|
| ``Keyboard and Trackpad``|✅|✅|
| ``Headphone Jack``|✅|✅|
| ``Graphics``|✅|✅|
| ``Battery``|✅|✅|
| ``Power Management``|✅|✅|
| ``Multigesture Trackpad``|✅|✅|                                                                          
| ``Webcam``|✅|✅|
| ``USB Port``|✅|✅|
| ``Facetime and iMessage``|✅|✅|
| ``Sleep``|✅|✅|
| ``Ethernet``|✅|✅|
| ``Hotkeys``|✅|✅|

# Post-Install
After installation, open System Preferences and go to Displays -> Color, uncheck `Show profiles for this display only`, then select `sRGB IEC61966-2.1`, this will make your colors look right (definitely not calibrated or anything but yeah, not an oversaturated mess)

<div align="center">
  
![Screenshot](Screenshots/Display.png)

</div>

If you want your fucking Display like RealMac, you can use [one-key-hidpi](https://github.com/xzhih/one-key-hidpi) (not recommended)

<div align="center">
  
![Screenshot](Screenshots/Display_2.png)
  
</div>

# How to use this EFI ?
You download the macOS installer from [HeaVietNam](https://heavietnam.github.io/image/index.html) (although the online recovery method is still better), then use MiniTool or other software to mount the EFI partition, then use Explorer++ to access the EFI partition and copy it to your EFI folder. Remember to add the entry to your firmware afterwards, using [EasyUEFI](https://www.easyuefi.com/index-us.html) or your firmware's built-in boot configurator.
# Thanks
- [NLTD2010](https://github.com/NLTD2010) and [Olarila](https://olarila.com) for my EFI folders.
- [khanhmuy](https://github.com/khanhmuy) for my README file.
- [Võ Nguyễn HoangLong](https://www.facebook.com/profile.php?id=100070274020733) for [HeaVietNam](http://heavietnam.ga/) guide.
- [Stijn Rombouts](https://www.facebook.com/stijn.rombouts2) for help me fixed something.
