# BIOS

This repository includes official releases and beta versions of BIOS for various branches, as well as related tools.

- ⚠ Generally, you should only upgrade the BIOS of the same branch. Cross-branch upgrades should only be performed when testing different BIOS features.
- ⚠ Upgrading the BIOS across different branches will invalidate the Secure Boot keys.
- ⚠ Upgrading to the incorrect BIOS branch may result in some functions of the carrier board not working properly.

## BIOS Naming Rule

> Example:  
> LP-BS-S70NC1R200-SR-A-SATA
>
> - **LP**: LattePanda
> - **BS**: BIOS
> - **S70NC1R200**: Internal version number for LattePanda Mu
> - **SR**:
>   - SR: Single Rank memory
>   - DR: Dual Rank memory
> - **A**: BIOS version number, with new versions sequentially labeled in alphabetical order
> - **SATA**: The interface configuration for this BIOS branch, with detailed configuration differences for each branch available in the README within the branch directory.
>   - No suffix: DFLT (Default) branch
>   - SATA: SATA branch
>   - PCIE: PCIE branch
>   - MUSB: MUSB branch

## File Description

- Beta: Beta version BIOS, not specific to any branch, intended for professional developers to assess new features.

- DFLT: Default version BIOS, which is the BIOS branch that comes pre-installed on the LattePanda Mu.

- MUSB: A BIOS branch configured to maximize USB 3.2 10Gbps interface capabilities (coming soon).

- PCIE: A BIOS branch configured to maximize PCIe 3.0 lane configurations (coming soon).

- SATA: A BIOS branch that provides SATA interface signal.

- Tools: Tools for BIOS maintenance.
