# 🌀 OpenClash_Overwrite 覆写模块

> 建议新装 **OpenClash** 用户使用，无需修改任何 LuCI 设置
> 适配版本：**OpenClash v0.47.006 及以上**

---

## 📌 使用建议

* 建议切换更新分支为 **Dev** 并不启用 **Smart 内核**

分流规则与策略组基于项目：
👉 [Aethersailor/Custom_OpenClash_Rules](https://github.com/Aethersailor/Custom_OpenClash_Rules.git)

---

## ⚙️ 使用方法

### 1️⃣ 新增覆写模块

* **文件名**：可自定义
* **类型**：`http`
* **订阅链接**：根据需求选择

#### 主路由用户

```bash
https://raw.githubusercontent.com/Giveupmoon/OpenClash_Overwrite/refs/heads/main/Overwrite/Overwrite.conf
```

#### 无需 IPv6 用户

```bash
https://raw.githubusercontent.com/Giveupmoon/OpenClash_Overwrite/refs/heads/main/Overwrite/Overwrite-noipv6.conf
```

#### 旁路由用户

```bash
https://raw.githubusercontent.com/Giveupmoon/OpenClash_Overwrite/refs/heads/main/Overwrite/Overwrite-bypass.conf
```

---

### 2️⃣ 配置环境变量

所有配置需注意以下环境变量：

* **机场订阅链接**（必填）

```bash
EN_KEY=你的机场订阅链接
```

* **自定义 DNS**（仅旁路由可选，主路由默认追加上游DNS）

```bash
EN_DNS=DNS
```

配置完成后，**保存 → 前往其他配置页底部 → 点击「应用配置」**。

---

## 💡 温馨提示

1. 本仓库文件引用的均为 **原始链接**，需确保路由器本身可访问 GitHub
2. 初次运行成功后，可能会提示 **内核错误**，多重启几次即可
3. 默认 OpenClash 不含 **GeoIP 数据库**：

   * 第一次运行会自动下载 `GeoIP.dat`
   * 不能热重载，导致第一次运行可能报错
   * 建议手动提前更新 GeoIP 数据库

---