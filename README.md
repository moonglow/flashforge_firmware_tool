# FlashForge firmware tool
Supported printers:
* FlashForge Dreamer
* FlashForge Dreamer NX
* FlashForge Finder
* FlashForge Creator Max
* FlashForge Guider ( not linux based firmware like in Guider II, II S )
* FlashForge Inventor ( not linux based firmware like FlashForge Inventor II )
* Dremel 3D20
------------
### Building
**Linux:**

`gcc main.c -o ff_fw_tool`

**Windows:**

Pelles C project included

**Firmware encryption keys:**
| Key | Vendor |
| ---------- | ---------- |
| flashforge790315 | FlashForge |
| flashforge123456 | Dremel |
### Usage
**Decrypt firmware:**

`ff_fw_tool [-k <key>] -i firmware.bin -o decrypted_firmware.bin`

**Encrypt firmware:**

`ff_fw_tool [-k <key>] -e -i firmware.bin -o encrypted_firmware.bin`