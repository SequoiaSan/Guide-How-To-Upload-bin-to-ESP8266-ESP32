# How To Upload *.bin to ESP8266/ESP32
This is a short guide how to upload precompiled bin files to ESP8266/ESP32 
If you have something to add or troubles - leave the issue that is not covered by this guide and we can try to figure it out.

# Method (Windows)
Don't be scared of this method by its old-school UI-UX, just follow the instructions with provided screenshots and you should be good.

1. Download official latest ESPRESSIF flasher from [this page](https://www.espressif.com/en/support/download/other-tools). Link to version used for this guide you can find [here](https://www.espressif.com/sites/default/files/tools/flash_download_tool_3.9.2.zip)
2. Extract archive and start **flash_download_tool_X.X.X.exe**
3. Select your ESPRESSIF chip in opened window.
For example for ESP8266 select ESP8266 (your captain)

![Select_ESP8266](https://github.com/SequoiaSan/Guide-How-To-Upload-bin-to-ESP8266-ESP32/blob/main/rep_images/espriff_flasher_select_chip_type_esp8266_1.png?raw=true)

**For FlipperZero's dev board select ESP32S2**

![FlipperZero_devboard_chip](https://github.com/SequoiaSan/Guide-How-To-Upload-bin-to-ESP8266-ESP32/blob/main/rep_images/espriff_flasher_select_chip_type_esp32s2_2.png?raw=true)

4. On next window leave all by default. See next screenshots as reference.
Choose .bin file. Don't forget to tick the box on the left near the text box with chosen .bin

### **!ATTENTION! Choose appropriate offset!!!**
| Chip  | Offset |
| - | - |
| ESP8266  | 0x0  |
| ESP32  | 0x10000  |

### Note to FlipperZero's Dev Module v.1 and any other boards that have BOOT button
The BOOT button has to be pressed while connecting the dev board to the usb port to detect the board as the right one and to show the right COM Port.

Choose - COM port to which your ESP currently connected
And you may want to choose higher BAUD rate to speed up flash process.


For ESP8266

![ESP8266_1](https://github.com/SequoiaSan/Guide-How-To-Upload-bin-to-ESP8266-ESP32/blob/main/rep_images/espriff_flasher_interface_esp8266_1.png?raw=true)

For ESP32S2

![ESP32S2_1](https://github.com/SequoiaSan/Guide-How-To-Upload-bin-to-ESP8266-ESP32/blob/main/rep_images/espriff_flasher_interface_esp32s2_1.png?raw=true)

5. Click START. After successful flash your window will look like this

For ESP8266

![ESP8266_2](https://github.com/SequoiaSan/Guide-How-To-Upload-bin-to-ESP8266-ESP32/blob/main/rep_images/espriff_flasher_interface_esp8266_2.png?raw=true)

For ESP32S2

![ESP32S2_2](https://github.com/SequoiaSan/Guide-How-To-Upload-bin-to-ESP8266-ESP32/blob/main/rep_images/espriff_flasher_interface_esp32s2_2.png?raw=true)

**That's it! Have fun :)**
