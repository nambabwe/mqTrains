
# Uploading

<br>

## ![Badge Linux]   ![Badge Pi]   ![Badge MacOS]

```Shell
esptool.py                      \
    --baud 460800               \
    --chip esp8266              \
    --port /dev/ttyUSB0         \
    --before default_reset      \
    --after hard_reset write_flash 0x0 mqTrains_ServoPCA_0.98_1MB.bin
```

<br>
<br>

## ![Badge Windows]

*Use the following settings.*

| Settings | Value 
|:--------:|:-----:
| **Baudrate**    | `230400m`
| **Flash Speed** | `40MHz`
| **Flash Size**  | `1MB`
| **SPI Mode**    | `DOUT`

<br>


<!---------------------------------[ Badges ]---------------------------------->

[Badge Windows]: https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logoColor=white&logo=Windows
[Badge Linux]: https://img.shields.io/badge/Linux-00A95C?style=for-the-badge&logoColor=white&logo=Linux
[Badge MacOS]: https://img.shields.io/badge/MacOS-525252?style=for-the-badge&logoColor=white&logo=MacOS
[Badge Pi]: https://img.shields.io/badge/Pi-A22846?style=for-the-badge&logoColor=white&logo=RaspberryPi
