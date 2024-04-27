# Pinouts

All pin definitions for LattePanda Mu

⚠️ Note:  
Due to the large number of functionally multiplexing pins, you should check the [BIOS functionality documentation](../../Softwares/BIOS/README.md) before starting your design. Do not design directly from the pin definition documentation here.

![pinout](./pinout.jpg)

## eDP

I-PEX 20455-040E

| Number | Name      | Type | Description              |
|--------|-----------|:----:|--------------------------|
| 1      | NC        |      |                          |
| 2      | GND       |      |                          |
| 3      | DDIA_TX3- | O    | Lane 3 (-)               |
| 4      | DDIA_TX3+ | O    | Lane 3 (+)               |
| 5      | GND       |      |                          |
| 6      | DDIA_TX2- | O    | Lane 2 (-)               |
| 7      | DDIA_TX2+ | O    | Lane 2 (+)               |
| 8      | GND       |      |                          |
| 9      | DDIA_TX1- | O    | Lane 1 (-)               |
| 10     | DDIA_TX1+ | O    | Lane 1 (+)               |
| 11     | GND       |      |                          |
| 12     | DDIA_TX0- | O    | Lane 0 (-)               |
| 13     | DDIA_TX0+ | O    | Lane 0 (+)               |
| 14     | GND       |      |                          |
| 15     | DDIA_AUX+ | O    | Auxiliary channel (+)    |
| 16     | DDIA_AUX- | O    | Auxiliary channel (-)    |
| 17     | GND       |      |                          |
| 18     | LCD_VCC   |      | LCD Power Supplies       |
| 19     | LCD_VCC   |      | LCD Power Supplies       |
| 20     | LCD_VCC   |      | LCD Power Supplies       |
| 21     | LCD_VCC   |      | LCD Power Supplies       |
| 22     | Selftest  | O    | Default Grounding        |
| 23     | GND       |      |                          |
| 24     | GND       |      |                          |
| 25     | GND       |      |                          |
| 26     | GND       |      |                          |
| 27     | HPD       | I    | Plug Detection           |
| 28     | GND       |      |                          |
| 29     | GND       |      |                          |
| 30     | GND       |      |                          |
| 31     | GND       |      |                          |
| 32     | BL_EN     | O    | Backlight enable         |
| 33     | BL_PWM    | O    | Backlight PWM dimming    |
| 34     | NC        |      |                          |
| 35     | NC        |      |                          |
| 36     | BL_PWR    |      | Backlight Power Supplies |
| 37     | BL_PWR    |      | Backlight Power Supplies |
| 38     | BL_PWR    |      | Backlight Power Supplies |
| 39     | BL_PWR    |      | Backlight Power Supplies |
| 40     | NC        |      |                          |

- **LCD_VCC**: +3.3V
- **BL_PWR**: Same as LattePanda Mu input voltage
- **Selftest**: Factory test pin, ground by default

## Touch

Clamshell 6P 0.5mm FFC/FPC Connector

| Number | Name       | Type | Description           |
|--------|------------|:----:|-----------------------|
| 1      | I2C0_SCL   | O    | I2C Bus               |
| 2      | I2C0_SDA   | I/O  | I2C Bus               |
| 3      | GND        |      |                       |
| 4      | TOUCH_RST# | O    | Touch panel reset     |
| 5      | TOUCH_INT  | I    | Touch event interrupt |
| 6      | +3.3V      |      | Touch panel power     |

## MIPI CSI-2

Clamshell 22P 0.5mm FFC/FPC Connector

| Number | Name      | Type | Description       |
|--------|-----------|:----:|-------------------|
| 1      | GND       |      |                   |
| 2      | CSI_B_D0- | I    | MIPI Data Lane 0  |
| 3      | CSI_B_D0+ | I    | MIPI Data Lane 0  |
| 4      | GND       |      |                   |
| 5      | CSI_B_D1- | I    | MIPI Data Lane 1  |
| 6      | CSI_B_D1+ | I    | MIPI Data Lane 1  |
| 7      | GND       |      |                   |
| 8      | CSI_B_CK- | I    | MIPI Clock        |
| 9      | CSI_B_CK+ | I    | MIPI Clock        |
| 10     | GND       |      |                   |
| 11     | CSI_B_D2- | I    | MIPI Data Lane 2  |
| 12     | CSI_B_D2+ | I    | MIPI Data Lane 2  |
| 13     | GND       |      |                   |
| 14     | CSI_B_D3- | I    | MIPI Data Lane 3  |
| 15     | CSI_B_D3+ | I    | MIPI Data Lane 3  |
| 16     | GND       |      |                   |
| 17     | CAM_RST   | O    | Camera reset      |
| 18     | CAM_MCLK  | O    | Camera main clock |
| 19     | GND       |      |                   |
| 20     | I2C1_SCL  | O    | I2C bus           |
| 21     | I2C1_SDA  | I/O  | I2C bus           |
| 22     | +3.3V     |      | Camera power      |

- **CAM_RST**: SoC GPP_A21
- **CAM_MCLK**: SoC GPP_D4

## SODIMM

DDR4 SODIMM pin table is too long, so I put it in a separate csv file.

- [Front Side](./front.csv)
- [Back Side](./back.csv)

⚠️ Note:  
Due to the large number of functionally multiplexing pins, you should check the [BIOS functionality documentation](../../Softwares/BIOS/README.md) before starting your design. Do not design directly from the pin definition documentation here.