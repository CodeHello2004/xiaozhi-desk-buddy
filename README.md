# Simple Circuits Xiaozhi Web Flasher 1.1.0

This browser installer lets the user select a supported ESP32-S3 board and a country or time-zone offset before installation.

Supported boards:

- Seeed Studio XIAO ESP32-S3 with 8 MB flash and 8 MB PSRAM
- ESP32-S3 DevKitC-1 N8R8 with 8 MB flash and 8 MB PSRAM
- Waveshare ESP32-S3-Zero FH4R2 with 4 MB flash and 2 MB PSRAM

All three options use the same external hardware and GPIO numbers:

- Touch OUT: GPIO1
- INMP441 SCK: GPIO2
- INMP441 WS: GPIO3
- INMP441 SD: GPIO4
- SH1106 SDA: GPIO5
- SH1106 SCL: GPIO6
- MAX98357A BCLK: GPIO7
- MAX98357A LRC: GPIO8
- MAX98357A DIN: GPIO9

Upload the complete contents of the generated release folder to one HTTPS static-site directory. Keep the firmware, manifests, and timezones folders unchanged. Open index.html using desktop Chrome or Microsoft Edge.

The selected time-zone file contains only the clock/timezone_offset setting. It contains no Wi-Fi name or password. A new installation clears saved settings and starts the Xiaozhi Wi-Fi setup process.

Before reinstalling an already-bound device, delete its old device entry from xiaozhi.me if you need the server to issue a new six-digit activation code.

The selected UTC offset is fixed and does not automatically follow daylight-saving changes.
