# BIOS

This repository includes official releases and beta versions of BIOS for various branches, as well as related tools.

- ⚠ Generally, you should only upgrade the BIOS of the same branch. Cross-branch upgrades should only be performed when testing different BIOS features.
- ⚠ Upgrading the BIOS across different branches will invalidate the Secure Boot keys.
- ⚠ Upgrading to the incorrect BIOS branch may result in some functions of the carrier board not working properly.

------

## Naming Rule

### New Naming Scheme (2025-12 and later)

**Format**
`S70NC1R200-[Memory]-[Version][-Variant].bin`

- **S70NC1R200**: Platform identifier (LattePanda Mu N100/N305)
- **Memory**:
  - `8G` = 8GB RAM
  - `16G` = 16GB RAM
- **Version**:
  - `A`, `B`, `C`... (incremented alphabetically for each new release)
- **Variant** (optional):
  - *(no suffix)* = Default (PCIe)
  - `SATA` = SATA branch

**Examples**

- `S70NC1R200-8G-A.bin` → 8GB, Default (PCIe)
- `S70NC1R200-16G-A-SATA.bin` → 16GB, SATA

**Notes**

- New scheme is simplified and user-oriented.
- **All subsequent updates will follow this naming convention.**

### Legacy Naming Scheme (2024 Initial Release)

**Format**
`LP-BS-S70NC1R200-[Rank]-[Version][-Variant].bin`

- **LP**: LattePanda
- **BS**: BIOS
- **S70NC1R200**: Platform identifier(LattePanda Mu N100/N305)
- **Rank**:
  - `SR` = Single Rank (corresponds to 8GB models)
  - `DR` = Dual Rank (corresponds to 16GB models)
- **Version**:
  - `A`, `B`
- **Variant**:
  - *(no suffix)* = Default (PCIe)
  - `SATA` = SATA branch

**Example**

- `LP-BS-S70NC1R200-SR-B.bin` → 8GB, Default (PCIe)

- `LP-BS-S70NC1R200-DR-B-SATA.bin` → 16GB, SATA

### Mapping: Legacy → New Naming

- `SR` → `8G`
- `DR` → `16G`

**Examples**

- `LP-BS-S70NC1R200-SR-B.bin` → `S70NC1R200-8G-A.bin` (newer)
- `LP-BS-S70NC1R200-DR-B-SATA.bin` → `S70NC1R200-16G-A-SATA.bin` (newer)

------

## Folder Description

- Beta: Beta version BIOS, not specific to any branch, intended for professional developers to assess new features.
- DFLT: Default version BIOS, which is the BIOS branch that comes pre-installed on the LattePanda Mu.
- SATA: A BIOS branch that provides SATA interface signal.
- Tools: Tools for BIOS maintenance.

------

## Release Timeline

```text
    2024-06/07                 2025-12 (Latest)                      
        │                          │
        ●──────────────────────────●
        │                          │
[Initial Release]          [Current Recommended]
    DFLT,SATA                  DFLT,SATA 
```

For specific model compatibility and functional changes, please refer to the `BOS Release Notes` located in each branch's folder.
