# ESP-01-AI-Cloud-Black-Drivers
Firmware drivers for ESP-01 AI-Cloud Inside Black 

Flashing settings are as follows

AT_V1.1_on_ESP8266_NONOS_SDK_V1.5.4


### Flash size 16Mbit: 512KB+512KB
    boot_v1.2+.bin              0x00000
    user1.1024.new.2.bin        0x01000
    esp_init_data_default.bin   0x1fc000 (optional) (In tested version this was not flashed)
    blank.bin                   0x7e000 & 0x1fe000


Use application in "FLASH_DOWNLOAD_TOOLS_v2.4_150924.rar" to flash to esp-01(ESP8266)
Firmware is : "AT_V1.1_on_ESP8266_NONOS_SDK_V1.5.4.zip"
