<p align="center">
  <a href="https://github.com/mcusee">
    <img src="https://github.com/mcusee/OpenWrt/raw/main/img/openwrt-log_02.jpg" 
         width="500" 
         style="border-radius: 20px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" 
         alt="OpenWrt Logo" />
  </a>
</p>
</p>
<p align="center">
  <a href="https://github.com/mcusee/OpenWrt-build/actions/workflows/build.yml">
    <img src="https://github.com/mcusee/OpenWrt-build/actions/workflows/build.yml/badge.svg" alt="Build OpenWrt">
  </a>
<p align="center">
  <a href="https://t.me/+6lVxjVM3ttVmMWM1">
    <img src="https://img.shields.io/badge/Telegram-加入通知群组-blue.svg?logo=telegram&style=for-the-badge" alt="Telegram" height="40">
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/OpenWrt-X86--64位-32C955.svg?logo=openwrt" alt="Platform">
  <a href="https://github.com/mcusee/OpenWrt-build/actions/workflows/build.yml">
    <img src="https://github.com/mcusee/OpenWrt-build/actions/workflows/build.yml/badge.svg" alt="Build Status">
  </a>
  <a href="https://github.com/coolsnowwolf/lede">
    <img src="https://img.shields.io/badge/License-GPL--3.0-red.svg" alt="License">
  </a>
</p>
<p align="center">
  <a href="https://github.com/mcusee/OpenWrt-build/actions">
    <img src="https://img.shields.io/github/actions/workflow/status/mcusee/OpenWrt-build/build-openwrt.yml?branch=main&style=for-the-badge&logo=github-actions&label=Build%20Status" alt="Build Status">
  </a>
  <a href="https://github.com/mcusee/OpenWrt-build/releases">
    <img src="https://img.shields.io/github/v/release/mcusee/OpenWrt-build?include_prereleases&style=for-the-badge&logo=github&color=blue&label=Firmware" alt="Release">
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/github/stars/mcusee/OpenWrt-build?style=flat-square&color=yellow&logo=github" alt="Stars">
  <img src="https://img.shields.io/github/forks/mcusee/OpenWrt-build?style=flat-square&color=lightgrey&logo=github" alt="Forks">
  <img src="https://img.shields.io/github/last-commit/mcusee/OpenWrt-build?style=flat-square&logo=git" alt="Last Commit">
</p>

<div align="center">

| 平台+设备名称 | 固件编译状态 | 配置文件 | 固件下载 |
| :-------------: | :-------------: | :-------------: | :-------------: |
| **OpenWrt X86_64 (Kernel 5.15)** | [![Build Status](https://github.com/mcusee/OpenWrt-build/actions/workflows/build.yml/badge.svg)](https://github.com/mcusee/OpenWrt-build/actions/workflows/build.yml) | [![](https://img.shields.io/badge/编译-脚本-orange.svg?logo=gnubash)](https://github.com/mcusee/OpenWrt-build/blob/main/build-diy.sh) | [![](https://img.shields.io/badge/下载-最新固件-blueviolet.svg?logo=github)](https://github.com/mcusee/OpenWrt-build/releases) |
| **OpenWrt X86_64 (Kernel 5.4)** | [![Build Status](https://github.com/mcusee/OpenWrt-build/actions/workflows/build.yml/badge.svg)](https://github.com/mcusee/OpenWrt-build/actions/workflows/build.yml) | [![](https://img.shields.io/badge/编译-脚本-orange.svg?logo=gnubash)](https://github.com/mcusee/OpenWrt-build/blob/main/build-diy.sh) | [![](https://img.shields.io/badge/下载-最新固件-blueviolet.svg?logo=github)](https://github.com/mcusee/OpenWrt-build/releases) |

</div>
📊 项目统计
<p align="center">
  <img src="https://ghchart.rshah.org/mcusee" alt="mcusee's Github Chart" />
</p>

## ✨ 项目亮点

* ☁️ **云端自动编译**: 基于 GitHub Actions，无需本地高性能电脑，一键开启编译任务。
* ⚡ **多固件支持**: 默认适配 **x86_64 (软路由)架构。
* 🔄 **上游同步**: 启动自动拉取 [Lean's LEDE](https://github.com/coolsnowwolf/lede) 源码，保持内核与插件最新。
* 🛠️ **一键定制**: 支持通过修改 `.config` 文件精准控制固件功能。

---

## 🛠️ 快速上手

### 1. 准备工作
首先 **Fork** 本仓库到你的账号下。

### 2. 配置固件
将你的配置文件命名为 `.config` 并放置在仓库根目录下。（记得修改build-diy.sh脚本里的配置文件.config地址）

### 3. 触发编译
1. 点击页面顶部的 **Actions** 选项卡。
2. 在左侧列表选择对应的 Workflow (如 `Build OpenWrt`)。
3. 点击右侧的 **Run workflow** 按钮。

### 4. 获取成品
编译完成后，前往 **Releases** 页面下载生成的固件镜像。

---

## 📂 目录结构

```text
.
├── .github/workflows/       # GitHub Actions 自动化脚本
├── .config                  # 自行在build-diy.sh脚本里修改自己的 https://raw.githubusercontent.com/mcusee/studio/main/.config
├── build-diy.sh             # 核心编译配置文件 (需自行添加)
└── README.md                # 本文档
