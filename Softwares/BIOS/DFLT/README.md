💡**Note:** The LattePanda Mu compute module is available in 8GB and 16GB memory versions. It is essential to select the correct BIOS firmware as described below.

### For LattePanda Mu N100 **8GB** RAM Model:

- LP-BS-S70NC1R200-SR-B
- S70NC1R200-8G-A **(Latest)**

### For LattePanda Mu N100 / N305 **16GB** RAM Model:

- LP-BS-S70NC1R200-DR-B
- S70NC1R200-16G-A **(Latest)**

---

# BIOS Release Notes

## [2025-12] Latest Release
### 📂 BIOS Files
| Variant | Compatible Model | Filename | Build Date |
| :--- | :--- | :--- | ---- |
| **PCIe** | LattePanda Mu N100 **8GB** | `S70NC1R200-8G-A.bin` | 2025/12/19 |
| **PCIe** | LattePanda Mu N100 / N305 **16GB** | `S70NC1R200-16G-A.bin` | 2025/12/19 |
| **SATA** | LattePanda Mu N100 **8GB** | `S70NC1R200-8G-A-SATA.bin` | 2025/12/19 |
| **SATA** | LattePanda Mu N100 / N305 **16GB** | `S70NC1R200-16G-A-SATA.bin` | 2025/12/19 |

### 📝 Changelog
1. Added SMBIOS information.
2. Added information for eMMC, SATA, NVMe, etc. in the Main tab.
3. Unlocked PCIe Clock configuration menu.
4. Unlocked PCIe port ASPM configuration menu (Default: Disabled).
5. Added toggle options for TP (Touch Panel) and eDP display.
6. Added GPIO function support and configuration menu.
7. Enabled SpeedStep(TM) and RC6; changed Package C State Limit to Auto.
8. Added RTL8111H PXE boot support.
9. Fixed the issue of duplicate UART numbering in the OS.
10. Added Windows Recovery support (Requires customized OS).

---

## [2024-06/07] Initial Release
### 📂 BIOS Files
| Variant | Compatible Model | Filename | Build Date |
| :--- | :--- | :--- | ---- |
| **PCIe** | LattePanda Mu N100 **8GB** | `LP-BS-S70NC1R200-SR-B.bin` | 2024/07/08 |
| **PCIe** | LattePanda Mu N100 / N305 **16GB** | `LP-BS-S70NC1R200-DR-B.bin` | 2024/06/19 |
| **SATA** | LattePanda Mu N100 **8GB** | `LP-BS-S70NC1R200-SR-B-SATA.bin` | 2024/07/05 |
| **SATA** | LattePanda Mu N100 / N305 **16GB** | `LP-BS-S70NC1R200-DR-B-SATA.bin` | 2024/06/20 |


### 📝 Changelog
- Initial BIOS firmware release.

---

# DFLT Branch Introduction

Default factory BIOS interface configuration for LattePanda Mu.

## Interface Configuration

### Special Notes

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

- **TCP0**: HDMI 2.0

- **TCP1**: USB Type-C (requires external PD controller)

### GPIOs

- **I2C1**: Touch panel (touch connector on LattePanda Mu)
- **I2C2**: Communication with Type-C PD controller
- **GPP_B11**: Type-C PD controller PMCALERT\#
- **GPP_B14**: SATA HDD LED
- **GPP_D0**: WWAN_Power_Off
- **GPP_D1**: WWAN_Reset
- **GPP_D2**: Communication interrupt with Type-C PD controller

Other GPIOs not listed are not allocated specific functions.
