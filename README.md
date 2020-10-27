# FlashForge firmware tool
Supported printers:
* FlashForge Dreamer
* FlashForge Dreamer NX
* FlashForge Finder
* FlashForge Guider ( not linux based firmware like in Guider II, II S )
* FlashForge Inventor ( not linux based firmware like FlashForge Inventor II )
------------
### Building
**Linux:**

`gcc main.c -o ff_fw_tool`

**Windows:**

Pelles C project included
### Usage
**Decrypt firmware:**

`ff_fw_tool -i firmware.bin -o decrypted_firmware.bin`

**Encrypt firmware:**

`ff_fw_tool -e -i firmware.bin -o encrypted_firmware.bin`
