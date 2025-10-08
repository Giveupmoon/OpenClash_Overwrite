# 🌀 OpenClash_Overwrite 覆写模块

> 💬 **欢迎 [Issue](https://github.com/Giveupmoon/OpenClash_Overwrite/issues) 提出您的建议和想法！**
> 🧩 适配版本：**OpenClash v0.47.006 及以上**
> 🧱 建议新装 **OpenClash** 用户使用，无需修改任何 LuCI 设置

---

<p align="center">
  <img src="https://img.shields.io/github/last-commit/Giveupmoon/OpenClash_Overwrite?style=for-the-badge&logo=git&label=Last%20Update" />
  <img src="https://img.shields.io/github/repo-size/Giveupmoon/OpenClash_Overwrite?style=for-the-badge&logo=github&label=Repo%20Size" />
  <img src="https://img.shields.io/badge/OpenClash-v0.47.006%2B-blue?style=for-the-badge&logo=openwrt" />
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" />
</p>

---

## 📖 目录

* [📌 使用建议](#-使用建议)
* [⚙️ 使用方法](#️-使用方法)

  * [1️⃣ 新增覆写模块](#1️⃣-新增覆写模块)
  * [2️⃣ 配置环境变量](#2️⃣-配置环境变量)
* [💡 温馨提示](#-温馨提示)
* [📂 项目来源](#-项目来源)

---

## 📌 使用建议

* 建议切换更新分支为 **Dev** 并 **不启用 Smart 内核**。
* 分流规则与策略组基于以下项目：
  👉 [Aethersailor/Custom_OpenClash_Rules](https://github.com/Aethersailor/Custom_OpenClash_Rules.git)

---

## ⚙️ 使用方法

### 1️⃣ 新增覆写模块

* **文件名**：可自定义
* **类型**：`http`
* **订阅链接**：根据使用场景选择

#### 🔹 主路由用户

```bash
https://raw.githubusercontent.com/Giveupmoon/OpenClash_Overwrite/refs/heads/main/Overwrite/Overwrite.conf
```

#### 🔹 主路由无需 IPv6 用户

```bash
https://raw.githubusercontent.com/Giveupmoon/OpenClash_Overwrite/refs/heads/main/Overwrite/Overwrite-noipv6.conf
```

#### 🔹 旁路由用户

```bash
https://raw.githubusercontent.com/Giveupmoon/OpenClash_Overwrite/refs/heads/main/Overwrite/Overwrite-bypass.conf
```

---

### 2️⃣ 配置环境变量

在 OpenClash 中启用覆写模块前，请根据需要设置以下环境变量：

#### ✴️ 必填变量 — 机场订阅链接

```bash
EN_KEY=你的机场订阅链接
```

#### ✴️ 可选变量 — 自定义 DNS（仅旁路由）

```bash
EN_DNS=DNS
```

配置完成后，**保存 → 前往其他配置页底部 → 点击「应用配置」**。

---

## 💡 温馨提示

1. 仓库文件均使用 **GitHub 原始链接**，请确保路由器可正常访问 GitHub。
2.  默认 OpenClash 不包含 **GeoIP 数据库**：
   * 建议手动提前更新 GeoIP 数据库
3. 如未提前下载GeoIP数据库，初次运行可能提示 **内核错误**，多次重启后即可恢复。


---

✨ **如果本项目对你有帮助，请点个 Star 支持一下！**
🧡 [Giveupmoon/OpenClash_Overwrite](https://github.com/Giveupmoon/OpenClash_Overwrite)

---
