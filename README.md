# 📌 Description

**EN:** Custom Linux system development for R36 Ultra. Includes modified DTBs and flashing tools with tutorials.
**中文:** R36 Ultra 自定义 Linux 系统开发，包含修改后的设备树文件 (DTBs) 及刷机工具与教程。
-从R36U提取的资源，未作任何改动。介绍由GPT生成
---

# 📌 README.md

```markdown
# R36Ultra Linux — DTBs & Flash Tools  
# R36Ultra Linux — 设备树与刷机工具

---

## 📖 Description / 项目简介

**English:**  
This repository provides resources for developing a custom Linux system on the **R36 Ultra (RK3326-based handheld)**.  
It contains:  
- **dtbs/**: Original and modified DTB files, as well as kernel/system images.  
- **flashtools/**: Tools and tutorials for flashing, backup, and recovery.

**中文:**  
本仓库用于在 **R36 Ultra (基于 RK3326 的掌机)** 上开发自定义 Linux 系统。  
包含：  
- **dtbs/**：官方与修改后的设备树文件，以及内核/系统镜像。  
- **flashtools/**：刷机、备份与恢复所需的工具与教程。

---

````

---

## 🚀 Features / 功能特性

- 📑 Compare official vs custom DTBs for hardware bring-up  
- 🖥️ Provide ready-to-flash images and scripts  
- 🛠️ Documented flashing, partition layout, and recovery steps  

- 📑 对比官方与自定义 DTB，方便硬件适配  
- 🖥️ 提供可直接刷写的镜像与脚本  
- 🛠️ 完整的刷机、分区、恢复文档  

---

## 🔧 Quick Start / 快速开始

**English:**  
1. Install required tools (`rkdeveloptool`, `fastboot`, `adb`).  
2. Backup important partitions before flashing.  
3. Use provided scripts under `flashtools/` to flash u-boot, trust, and system images.  
4. Reboot and verify system.  

**中文:**  
1. 安装必要工具（`rkdeveloptool`、`fastboot`、`adb`）。  
2. 刷机前先备份关键分区。  
3. 使用 `flashtools/` 下的脚本刷写 u-boot、trust、系统镜像。  
4. 重启并验证系统。  

---

## 💾 Backup & Restore / 备份与恢复

**English:**  
```bash
# Backup u-boot
dd if=/dev/by-name/uboot of=backup/uboot.img bs=512
# Restore u-boot
dd if=backup/uboot.img of=/dev/by-name/uboot bs=512
````

**中文:**

```bash
# 备份 u-boot
dd if=/dev/by-name/uboot of=backup/uboot.img bs=512
# 恢复 u-boot
dd if=backup/uboot.img of=/dev/by-name/uboot bs=512
```

---

## 🤝 Contributing / 贡献

* **English:** PRs for new DTBs, patches, or improved flashing docs are welcome.
* **中文:** 欢迎提交 PR：新增/修正 DTB、驱动补丁、改进刷机文档等。

---

## ⚖️ License / 许可证

* Code & scripts: MIT License

* Third-party binaries/tools: Original licenses apply

* 代码与脚本：MIT 协议

* 第三方工具：遵循各自原始协议

---

## ⚠️ Disclaimer / 免责声明

**English:**
Flashing and modifying system partitions carries risk. Please backup data before proceeding. The author is not responsible for data loss or device damage.

**中文:**
刷写和修改系统分区存在风险。请务必先备份数据。因使用本仓库造成的数据丢失或设备损坏，作者概不负责。

```
