# FlashForge firmware tool
Supported printers:
* FlashForge Dreamer
* FlashForge Dreamer NX
* FlashForge Finder
* FlashForge Creator Max
* FlashForge Guider ( not linux based firmware like in Guider II, II S )
* FlashForge Inventor ( not linux based firmware like FlashForge Inventor II )
* Dremel 3D20
* PowerSpec Ultra 3D
------------
### Building
**Linux:**

`gcc main.c -o ff_fw_tool`

**Windows:**

Pelles C project included

**Firmware encryption keys:**
| Key | Vendor |
| ---------- | ---------- |
| flashforge790315 | FlashForge/PowerSpec |
| flashforge123456 | Dremel |
### Usage
**Decrypt firmware:**

`ff_fw_tool -k key -i firmware.bin -o decrypted_firmware.bin`

**Encrypt firmware:**

`ff_fw_tool -k key -e -i firmware.bin -o encrypted_firmware.bin`


#### Support me
- <a href="https://www.patreon.com/bePatron?u=58145249" data-patreon-widget-type="become-patron-button">Become a Patron!</a>
- **Bitcoin (P2WPKH):** bc1qstnsjqu2kw9v2axens54ycegn3stwvluq7ze5j
