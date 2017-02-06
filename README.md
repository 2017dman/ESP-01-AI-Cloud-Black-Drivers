# ESP-01-AI-Cloud-Black-Drivers
Firmware drivers for ESP-01 AI-Cloud Inside Black 

Flashing setting as follows

AT_V1.1_on_ESP8266_NONOS_SDK_V1.5.4


### Flash size 16Mbit: 512KB+512KB
    boot_v1.2+.bin              0x00000
    user1.1024.new.2.bin        0x01000
    esp_init_data_default.bin   0x1fc000 (optional)
    blank.bin                   0x7e000 & 0x1fe000
