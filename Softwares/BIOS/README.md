# BIOS

包含官方支持分支的正式版与测试版 BIOS 及相关工具

- ⚠ 一般情况只应升级同分支 BIOS, 仅当测试不同 BIOS 功能时才需要跨分支升级.
- ⚠ 跨分支升级会使安全启动密钥失效
- ⚠ 升级错误的 BIOS 分支可能导致载板功能无法正常工作

## BIOS 命名规则

> 例:  
> LP-BS-S70NC1R200-SR-A-SATA
>
> - **LP**: LattePanda
> - **BS**: BIOS
> - **S70NC1R200**: LattePanda Mu 内部代号
> - **SR**:
>   - SR: Single Rank 单面内存
>   - DR: Dual Rank 双面内存
> - **A**: 版本号, 新版本将按字母顺序编号
> - **SATA**: BIOS 接口配置分支, 各分支详细配置区别见分支目录内 README 说明.
>   - 无后缀: DFLT 默认分支
>   - SATA: SATA 分支
>   - PCIE: PCIE 分支
>   - MUSB: MUSB 分支

## 文件说明

- Beta: 测试版 BIOS, 不区分分支, 供专业开发者评估新功能用

- DFLT: 默认版 BIOS, 也是 LattePanda Mu 出厂自带的 BIOS 分支.

- MUSB: 最大化 USB 3.2 10Gbps 接口配置的 BIOS 分支 (即将发布)

- PCIE: 最大化 PCIe 3.0 通道配置的 BIOS 分支 (即将发布)

- SATA: 提供 SATA 接口的 BIOS 分支

- Tools: BIOS 维护工具
