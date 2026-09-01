# Carrier Board Sample Projects

LattePanda Mu carrier board sample projects for engineers' reference, designed with KiCAD. Please open with KiCAD version 9.0 or higher.

It's recommended to start your design  by referring to the *\[DFR1142\] Lite Carrier for LattePanda Mu(V2)*.

- [Carrier Board Design Guide for LattePanda Mu](https://docs.lattepanda.com/content/mu_edition/design_guide_foreword/)

## Project Files

- **\[DFR1141\] Full EVA Carrier for LattePanda Mu**: The evaluation carrier board that includes nearly all features of the LattePanda Mu, designed to ITX motherboard dimensions, suitable for professional developers.

- **\[DFR1142\] Lite Carrier for LattePanda Mu**: The lite carrier board that includes essential interfaces such as HDMI, USB, PCIe, designed to 3.5-inch embedded motherboard dimensions.

- **\[DFR1142\] Lite Carrier for LattePanda Mu(V2)**: The upgraded version of DFR1142 Lite Carrier. Optimized for evaluation use and small-batch deployment.
  - **Auto Power-On Support:** The system can boots automatically upon receiving power.
  - **New MX1.25-10P Connector:** Designed for compatibility with the DFR1247 LattePanda Smart UPS expansion board.
  - **Side-Mounted Buttons:** Power and Reset buttons have been changed to a side-mounted vertical design to accommodate protective cases better.
  - **External Control Headers:** Added pin headers for external power control and status indication.
  - **Sleep Indicator:** Added a dedicated LED for sleep mode status.
  - **BIOS Flash Chip Footprint:** Added a footprint for a carrier board BIOS flash chip (not soldered by default) for advanced customization.

- **\[DFR1144\] GPU Carrier for LattePanda Mu**: The GPU carrier board features six video output ports, supports Type A/B MXM standard graphics cards, and adopts the 3.5-inch embedded motherboard form factor. It is suitable for local AI inference or multi-screen display matrix applications.

- **\[DFR1293\] Mini Carrier for LattePanda Mu \\ Mu Ultra**: a compact, highly expandable carrier board compatible with the LattePanda Mu and LattePanda Mu Ultra compute module. It integrates commonly used ports such as two full-featured Type-C, 2.5G Ethernet, USB 3.2 Gen2, OCuLink, M.2 M Key, M.2 E Key, HDMI, and GPIO. 

## Compatibility List

Compatibility varies between different compute modules and different carrier boards. Please visit the [**Carrier Board Docs**](https://docs.lattepanda.com/content/mu_edition/module_carrier_compatibility/) for the compatibility list.
