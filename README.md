
# mqTrains

*Model railroad electronics using* ***MQTT*** *.*

---

**⸢ [Website] ⸥ ⸢ [Download] ⸥ ⸢ [Documentation] ⸥**

---


<br>

## Linux | Pi | MacOS

### Requirements

- **[Python]** & **[PIP]**

    ```sh
    sudo apt install python python-pip
    ```

- **[ESPTool]**

    ```sh
    sudo pip install esptool
    ```

<br>

### Uploading

```sh
esptool.py                      \
    --baud 460800               \
    --chip esp8266              \
    --port /dev/ttyUSB0         \
    --before default_reset      \
    --after hard_reset write_flash 0x0 mqTrains_ServoPCA_0.98_1MB.bin
```

<br>

---

<br>

## Windows

### Requirements

- Install **[NodeMCU-Flasher]**.

<br>

### Uploading

Use the following settings :

| Settings | Value |
|:--------:|:-----:|
| **Baudrate** | `230400m`
| **Flash Speed** | `40MHz`
| **Flash Size** | `1MB`
| **SPI Mode** | `DOUT`


<!----------------------------------------------------------------------------->

[Website]: https://www.mqtrains.com/
[Documentation]: ./released/mqTrains-UserReference.pdf
[Download]: ./preReleased/IOMCP/mqTrains_IO_0.77_1MB.bin

[Python]: https://www.python.org/
[PIP]: https://pypi.org/project/pip/
[ESPTool]: https://pypi.org/project/esptool/

[NodeMCU-Flasher]: https://github.com/nodemcu/nodemcu-flasher
