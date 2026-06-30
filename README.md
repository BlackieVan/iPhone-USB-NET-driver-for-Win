# iPhone USB & NET Drivers for Windows (Extreme Light Edition)

🚀 **一个只有几 MB 的纯净驱动包，让断网的 Windows 电脑直接通过 USB 共享 iPhone 网络。**

[![License](https://img.shields.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Platform](https://img.shields.shields.io/badge/platform-Windows%207%20%7C%2010%20%7C%2011-orange.svg)]()

---

## 💡 项目背景与痛点

在电脑**没有 Wi-Fi、没有网络、没装 iTunes**，但你手里只有**一台 iPhone** 和**一条 USB 数据线**的极端情况下：
* ❓ 想通过 iPhone 的 USB 共享网络让电脑上网？
* ❓ 想把 iPhone 里的照片和文件拷贝到电脑？
* ❌ 官方 iTunes 安装包动辄几百 MB，且在没网的情况下根本无法下载安装。

**本项目正是为了解决这个“鸡生蛋、蛋生鸡”的断网死循环而生。**

---

## ✨ 核心特性

* 📦 **极限精炼**：完全剔除官方 iTunes 软件全家桶，只提取最核心的驱动文件（不到 3MB）。
* 👥 **双架构支持**：同时完美集成 **x64（64位）** 与 **x86（32位）** 核心驱动，通杀从老旧 Win7 到现代 Win11 的绝大多数机型。
* 🔒 **纯净无后台**：纯手动设备管理器强刷，没有任何后台常驻服务、无开机自启，绿色环保。
* 🗺️ **套娃黑科技**：支持将驱动隐写伪装在 JPG 图片中，直接用手机相册当“U盘”安全带出。

---

## 🛠️ 隐写术原理（怎么做到的？）

利用 Windows 的二进制合并命令，将驱动压缩包藏在图片数据末尾，生成一张在手机和电脑上都能正常预览、但暗藏玄机的“套娃图片”：
```bash
copy /b iPhone-USB&NET-driver-for-Win.jpg + iPhone-USB&NET-driver-for-Win.zip iPhone-USB&NET-driver-for-Win.jpg
