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

After Flashing firmware you will be able to connect with the follwoing settings
Baud:   115200
Data:   8
Stop:   1
Parity: None
FLow:   None

TO get ESP-01 to work with Blynk & Arduino you need to also issue the following commands (in putty you will need to press enter and then CTRL+J)

AT+CWMODE=3                 // sets the ESP01 to have both AP and Station mode
AT+CIPMUX=1                 // sets the ESP01 to have up to 4 simultaneous connections
AT+UART_DEF=19200,8,1,0,0   // Sets Baud rate to 19200, if this does not work use the command below.
AT+IPR=19200                // Sets Baud rate to 19200, use if the above comand does not work. 
