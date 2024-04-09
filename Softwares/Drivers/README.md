# 驱动程序

此仓库仅包括 LattePanda Mu 驱动程序. 由载板扩展的硬件驱动请查看载板说明

## Windows 10/11

Windows 系统安装完成后，会自动连接互联网以获取驱动程序更新。如果无法连接到 Windows 更新服务，或自动更新后仍缺少某些驱动程序，可在此处下载离线驱动程序包。

| Name                                | Version         | Size    | Download                                                                        |
|--------------------------------------------|-----------------|---------|---------------------------------------------------------------------------------|
| Intel Chipset Driver                       | 10.1.19376.8374 | 2.72 MB | [⬇️](./Chipset_10.1.19376.8374.zip) |
| Intel Iris Xe Graphics Driver              | Latest          | N/A     | [⬇️](https://www.intel.com/content/www/us/en/download/785597/)[^1] |
| intel Serial IO Driver                     | 30.100.2229.4   | 353 KB  | [⬇️](./SerialIO_30.100.2229.4.zip)                                                         |
| intel HID Event Filter Driver              | 2.2.1.386       | 46.6 KB | [⬇️](./HID_2.2.1.386.zip)                                                         |
| Intel Management Engine Interface Driver   | 2306.4.10.0      | 20.5 MB | [⬇️](./MEI_2306.4.10.0.zip)                                                         |
| Intel GNA Scoring Accelerator Driver       | 03.00.00.1457   | 54 KB | [⬇️](./GNA_03.00.00.1457.zip)                                                         |
| Intel Integrated Sensor Solution Driver    | 3.1.0.4589      | 2.73 MB | [⬇️](./ISH_3.1.0.4589.zip)                                                         |
| TouchPanel Driver                          | 1.3.2.0         | 67.5 KB | [⬇️](./TouchPanel_1.3.2.0.zip)                                                         |

[^1]: 从 intel 官网下载

## Linux

Linux 驱动程序通常由发行版随内核和内核模块更新提供，请使用新内核以获得完整的驱动程序支持。

- 最低内核版本: 5.15
- 推荐内核版本: 6.1 或更新版本
