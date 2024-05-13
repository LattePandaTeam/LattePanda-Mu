# SATA 分支

在标准 BIOS 的基础上, 启用了集成的 SATA 控制器

## 接口配置

### 特别说明

- **USB2_P6**: USB TypeC 专用, 需要与 PD 控制器一起工作, **不可作为普通 USB 接口使用**

### HSIO (高速 I/O 通道)

- **HSIO0**: USB 3.2 10Gbps
- **HSIO1**: USB 3.2 10Gbps
- **HSIO2**: PCIe 3.0 x1
- **HSIO3**: PCIe 3.0 x1
- ==========
- **HSIO8**: PCIe 3.0 x2 (Lane 0)
- **HSIO9**: PCIe 3.0 x2 (Lane 1)
- **HSIO10**: SATA 3.0
- **HSIO11**: SATA 3.0
- ==========
- **HSIO6**: PCIe 3.0 x1

### DDI/TCP

- **DDIA**: eDP 1.4b (Mu 上的 eDP 接口)

- **DDIB**: HDMI 2.0

- **TCP0**: HDMI 2.0

- **TCP1**: USB Type-C (需要外置PD控制器)

### GPIOs

- **I2C1**: 触摸面板 (Mu 上触屏排线接口)
- **I2C2**: Type-C PD 控制器通信
- **GPP_B11**: Type-C PD 控制器 PMCALERT\#
- **GPP_B14**: SATA HDD LED
- **GPP_D0**: WWAN_Power_Off
- **GPP_D1**: WWAN_Reset
- **GPP_D2**: Type-C PD 控制器通信中断

其它未列出 GPIO 没有分配特定功能