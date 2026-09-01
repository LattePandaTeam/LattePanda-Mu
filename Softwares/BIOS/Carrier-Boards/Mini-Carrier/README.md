*This mini carrier board was developed alongside the LattePanda Mu Ultra compute module (based on the Intel Lunar Lake processor). The carrier board is code-named Lunar Lake IO Board, or LIO for short, which is the origin of the "LIO" suffix in the BIOS name.*

**These BIOS firmwares enable the LattePanda Mu N100 / N305 compute module to be compatible with the DFR1293 Mini Carrier Board.**

💡**Note:** The LattePanda Mu compute module is available in 8GB and 16GB memory versions. It is essential to select the correct BIOS firmware as described below.

- For LattePanda Mu N100 **8GB** RAM Model:

    - S70NC1R200-8G-B-LIO-001

- For LattePanda Mu N100 / N305 **16GB** RAM Model:

    - S70NC1R200-16G-B-LIO-001

---

# BIOS Release Notes

## [2026-07] Initial Release
### 📂 BIOS Files
| Compatible Model | Filename | Build Date |
| :--- | :--- | ---- |
| LattePanda Mu N100 **8GB** | `S70NC1R200-8G-B-LIO-001.bin` | 2026/07/30 |
| LattePanda Mu N100 / N305 **16GB** | `S70NC1R200-16G-B-LIO-001.bin` | 2026/07/30 |


### 📝 Changelog
- Initial BIOS firmware release: Based on `S70NC1R200-8G-B`, enabling the LattePanda Mu compute module to be compatible with the DFR1293 Mini Carrier Board.

---

## Interface Configuration

### Special Notes

- **USB2_P5**: Dedicated for USB Type-C, must be used in conjunction with a PD controller, **cannot be used as a standard USB port**.
- **USB2_P6**: Dedicated for USB Type-C, must be used in conjunction with a PD controller, **cannot be used as a standard USB port**.

### HSIO (High-Speed Input/Output)

- **HSIO0**: USB 3.2 10Gbps
- **HSIO1**: USB 3.2 10Gbps
- **HSIO2**: PCIe 3.0 x1
- **HSIO3**: PCIe 3.0 x1
- ==========
- **HSIO8**: PCIe 3.0 x4 (Lane 0)
- **HSIO9**: PCIe 3.0 x4 (Lane 1)
- **HSIO10**: PCIe 3.0 x4 (Lane 2)
- **HSIO11**: PCIe 3.0 x4 (Lane 3)
- ==========
- **HSIO6**: PCIe 3.0 x1

### DDI/TCP

- **DDIA**: eDP 1.4b (eDP interface on LattePanda Mu)

- **DDIB**: HDMI 2.0

- **TCP0**: USB Type-C (requires external PD controller)

- **TCP1**: USB Type-C (requires external PD controller)

### GPIOs

- **I2C1**: Touch panel (touch connector on LattePanda Mu)
- **I2C2**: Communication with Type-C PD controller
- **GPP_D1**: Communication interrupt with Type-C PD controller
- **GPP_E0**: Communication interrupt with Type-C PD controller
- **GPP_D3**: Output blink signal in sleep state

Other GPIOs not listed are not allocated specific functions.
