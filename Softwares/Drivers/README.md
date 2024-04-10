# Drivers

This repository contains only the LattePanda Mu drivers. For drivers related to the carrier board, please refer to the carrier board documentation.

## Windows 10/11

After installing Windows, the system will automatically connect to the internet to download driver updates. If it is unable to access the Windows Update service, or if there are missing drivers after the automatic updates, you can download the offline driver package here.


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

[^1]: Download from intel official website

## Linux

Linux drivers are generally provided by the distribution through kernel and kernel module updates. Please use a newer kernel version to ensure full driver support.

- Minimum kernel version: 5.18
- Recommended kernel version: 6.1 or later
