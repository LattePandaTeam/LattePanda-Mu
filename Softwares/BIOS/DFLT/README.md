# DEFT Branch

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