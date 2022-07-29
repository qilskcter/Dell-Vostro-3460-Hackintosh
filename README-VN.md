# <div align="center">Dell Vostro 3460 Hackintosh</div> 
## Bootloader versions

|OpenCore|Clover|
|--------|------|
|0.8.2|5146| 

## Các bản macOS support
- Mavericks
- Yosemite
- El Captain
- Sierra
- High Sierra
- Mojave
- Catalina
- Big Sur (⚠️ Dùng SMBIOS ```MacBookPro11,1```)
- Monterey (OpenCore)
## Screenshots

<div align="center">
  
![Screenshot](Screenshots/Monterey.png)
   
</div>
<details>
		<summary>Các OS khác</summary>
      <br>
  
![Screenshot](Screenshots/Mavericks.png)
![Screenshot](Screenshots/HighSierra.png)
![Screenshot](Screenshots/Mojave.png)
![Screenshot](Screenshots/Catalina.png)
![Screenshot](Screenshots/BigSur.png)
  
</details>

## Thông tin laptop
 
|                     | Thông tin chi tiết| Ghi chú |
| ---------------------------- | ---------------------- |------------------|
| ``Chipset``| Intel 7 Series/C210 Series Chipset. |   |
| ``CPU``| Intel Core i3-3110M 2.40GHz | Dùng [HFSPlusLegacy.efi](https://github.com/acidanthera/OcBinaryData/blob/master/Drivers/HfsPlusLegacy.efi) |
| ``Memory``| 8GB DDR3-1600MHz | 2 x 4GB DDR3 và DDR3L. |
| ``iGPU``| Intel HD Graphics 4000 | Patch with [Patch-HD4000-Monterey](https://github.com/chris1111/Patch-HD4000-Monterey) tạo bởi [chris1111](https://github.com/chris1111) trong Monterey. |
| ``dGPU``| NVIDIA GeForce GT630M | Chỉ có ở i5-3210M. |
| ``Disk 0``| SSD Lexar NS100 128GB | Dualboot Windows và macOS. |
| ``Disk 1``| HDD HGST HTS725050A7E630 500GB | Dùng lưu DATA. |
| ``Screen``| 14.0" 1366 x 768 |    |
| ``Ethernet``| Qualcomm Atheros AR8161 | Dùng [AtherosE2200Ethernet](https://github.com/Mieze/AtherosE2200Ethernet/releases/tag/2.2.2). |
| ``WiFi and Bluetooth``| Intel® Dual Band Wireless-AC 7260 | (Card cũ là AR9485). Dùng [AirportItlwm](https://github.com/OpenIntelWireless/itlwm/releases) cho Wifi và [IntelBluetoothFirmware](https://openintelwireless.github.io/IntelBluetoothFirmware/) cho Bluetooth. | 
| ``Audio``| Conexant Cx20590 | Thêm `alcid=27` trong boot-args. |
| ``Keyboard``| - | Yêu cầu patch SSDT cho brightness key. |
| ``Touchpad``| Dell Touchpad (ALPS, PS/2) | Dùng [VoodooPS2-ALPS](https://github.com/SkyrilHD/VoodooPS2-ALPS/releases/tag/1.0.7). |
| ``Dimensions``| 30mm x 345.5mm x 244mm |     |
|``Weight``| 2.23kg |     |
  
<div align="center">
  
![Screenshot](Screenshots/specs.png)
  
</div>

## Các tính năng đã hoạt động


|                               | OpenCore             | Clover|
| ----------------------------- | -------------------- | ------------------|
| ``Wifi and Bluetooth``|✅|✅|
| ``Audio``|✅|✅|
| ``Keyboard và Trackpad``|✅|✅|
| ``Headphone Jack``|✅|✅|
| ``Graphics``|✅|✅|
| ``Battery``|✅|✅|
| ``Power Management``|✅|✅|
| ``Multigesture Trackpad``|✅|✅|                                                                          
| ``Webcam``|✅|✅|
| ``USB Port``|✅|✅|
| ``Facetime và iMessage``|✅|✅|
| ``Sleep``|✅|✅|
| ``Ethernet``|✅|✅|
| ``Hotkeys``|✅|✅|

# Hướng dẫn cài
Sau khi cài xong, mở System Preferences và tìm Displays -> Color, bỏ check `Show profiles for this display only`, sau đó chọn `sRGB IEC61966-2.1`, điều này sẽ làm cho màu sắc của bạn trông đúng hơn(chắc chắn không được hiệu chỉnh hoặc bất cứ điều gì, nhưng không phải là một mớ hỗn độn quá bão hòa)

<div align="center">
  
![Screenshot](Screenshots/Display.png)

</div>

Nếu bạn muốn màn hình của mình giống real Mac thì bạn hãy dùng [one-key-hidpi](https://github.com/xzhih/one-key-hidpi) (không khuyến khích)

<div align="center">
  
![Screenshot](Screenshots/Display_2.png)
  
</div>

# Dùng EFI thế nào ?
Tải bộ cài tại [HeaVietNam](https://heavietnam.github.io/image/index.html) (bộ cài recovery online vẫn hơn), sau đó dùng MiniTool or hoặc các phần mềm khác để mount EFI partition, sau đó sử dụng Explorer ++ để truy cập phân vùng EFI và sao chép nó vào thư mục EFI của bạn. Hãy nhớ thêm boot-options, sử dụng [EasyUEFI](https://www.easyuefi.com/index-us.html) hoặc bios.
# Cảm ơn
- [Apple](https://apple.com) vì macOS.
- Acidanthera, SkyrilHD, USBToolBox, etc. vì tất cả các kext.
- [NLTD2010](https://github.com/NLTD2010) cho EFI của tôi và bản dịch tiếng Việt.
- [Olarila](https://olarila.com) vì EFI ăn liền (≧▽≦)
- [khanhmuy](https://github.com/khanhmuy) vì file README của tôi.
- [Võ Nguyễn HoangLong](https://www.facebook.com/profile.php?id=100070274020733) vì [HeaVietNam](http://heavietnam.ga/) guide.
- [Stijn Rombouts](https://www.facebook.com/stijn.rombouts2) vì đã giúp tôi fix một số thứ.
