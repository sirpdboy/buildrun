## 访问数：![hello](https://views.whatilearened.today/views/github/sirpdboy/deplives.svg)[![](https://img.shields.io/badge/TG群-点击加入-FFFFFF.svg)](https://t.me/joinchat/AAAAAEpRF88NfOK5vBXGBQ)

<p align="center">
<img alt="Github" src="https://img.shields.io/badge/Github-PASSWALL.RUN-green?logo=Github&logoColor=white">   <img alt="Github" src="https://img.shields.io/badge/Github-PASSWALL2.RUN-green?logo=Github&logoColor=white">   <img alt="Github" src="https://img.shields.io/badge/Github-OPENCLASH.RUN-green?logo=Github&logoColor=white">   <img alt="Github" src="https://img.shields.io/badge/Github-NIKKI.RUN-green?logo=Github&logoColor=white">   <img alt="Github" src="https://img.shields.io/badge/Github-SSR.RUN-green?logo=Github&logoColor=white">

# 🚀 自动构建 应用商店（store) IPK/APK RUN文件安装包

【[ENGLISH](https://github.com/sirpdboy/buildrun/edit/main/readme_en.md)】

 这是一个工作流。同步各位大佬项目里最新编译的ipk文件 生成适用于 OpenWrt/iStoreOS 用的run自解压包<br>
 本质上是利用makeslef,将ipk和shell文件打包成自解压程序。<br>
 iStoreOS 可以在iStore商店手动安装<br>

---

## 📥 RUN安装文件下载

[构建下载] 👇🏻   [进入讨论区](https://github.com/sirpdboy/buildrun/discussions/1)

[https://github.com/siropboy/CloudBuildRun/releases](https://github.com/siropboy/CloudBuildRun/releases)

## 📥 安装说明

### 一、 应用商店 RUN文件安装方法
<img width="1050" height="671" alt="image" src="https://github.com/user-attachments/assets/c74e5c00-c0d9-4c06-bf2d-a66d5124d80f" />


### 二、 通用安装方法

所有 `.run` 文件都是自解压安装包，使用方法如下：

```bash
# 1. 赋予执行权限
chmod +x *.run

# 2. 执行安装
./文件名.run
```

### 三、 根据系统选择正确的安装包

#### 1、🔹 OpenWrt 24.10 系统 (使用 opkg)

请选择文件名中包含 `ipk` 的安装包：

```bash
# x86_64 架构
./passwall-fw3-ipk-x86_64-*.run
# aarch64 架构
./passwall-fw3-ipk-aarch64-*.run
```

#### 2、🔹 Alpine 25.12 系统 (使用 apk)

请选择文件名中包含 `apk` 的安装包：

```bash
# x86_64 架构
./passwall-fw3-apk-x86_64-*.run
# aarch64 架构
./passwall-fw3-apk-aarch64-*.run
```

---

## 📋 详细文件列表

### 1. Passwall / Passwall2 (16 个文件)

#### FW3 (iptables) 模式 - 适用于传统防火墙

| 格式 | 架构 | 文件名示例 |
|------|------|------------|
| IPK (OpenWrt) | x86_64 | `passwall-fw3-ipk-x86_64-<version>.run` |
| IPK (OpenWrt) | aarch64 | `passwall-fw3-ipk-aarch64-<version>.run` |
| APK (Alpine) | x86_64 | `passwall-fw3-apk-x86_64-<version>.run` |
| APK (Alpine) | aarch64 | `passwall-fw3-apk-aarch64-<version>.run` |

#### FW4 (nftables) 模式 - 适用于新版防火墙 (OpenWrt 22.03+)

| 格式 | 架构 | 文件名示例 |
|------|------|------------|
| IPK (OpenWrt) | x86_64 | `passwall-fw4-ipk-x86_64-<version>.run` |
| IPK (OpenWrt) | aarch64 | `passwall-fw4-ipk-aarch64-<version>.run` |
| APK (Alpine) | x86_64 | `passwall-fw4-apk-x86_64-<version>.run` |
| APK (Alpine) | aarch64 | `passwall-fw4-apk-aarch64-<version>.run` |

**依赖说明：**
- **FW3 模式**：需要 `iptables`、`iptables-mod-tproxy`、`ipset` 等
- **FW4 模式**：需要 `nftables`、`kmod-nft-tproxy` 等

---

### 2. OpenClash (8 个文件)

#### FW3 (iptables) 模式

| 格式 | 架构 | 文件名示例 |
|------|------|------------|
| IPK (OpenWrt) | x86_64 | `openclash-fw3-ipk-x86_64-<version>.run` |
| IPK (OpenWrt) | aarch64 | `openclash-fw3-ipk-aarch64-<version>.run` |
| APK (Alpine) | x86_64 | `openclash-fw3-apk-x86_64-<version>.run` |
| APK (Alpine) | aarch64 | `openclash-fw3-apk-aarch64-<version>.run` |

#### FW4 (nftables) 模式

| 格式 | 架构 | 文件名示例 |
|------|------|------------|
| IPK (OpenWrt) | x86_64 | `openclash-fw4-ipk-x86_64-<version>.run` |
| IPK (OpenWrt) | aarch64 | `openclash-fw4-ipk-aarch64-<version>.run` |
| APK (Alpine) | x86_64 | `openclash-fw4-apk-x86_64-<version>.run` |
| APK (Alpine) | aarch64 | `openclash-fw4-apk-aarch64-<version>.run` |

---

### 3. Nikki -FW4 (4 个文件)

| 格式 | 架构 | 文件名示例 |
|------|------|------------|
| IPK (OpenWrt) | x86_64 | `nikki-ipk-x86_64-<version>.run` |
| IPK (OpenWrt) | aarch64 | `nikki-ipk-aarch64-<version>.run` |
| APK (Alpine) | x86_64 | `nikki-apk-x86_64-<version>.run` |
| APK (Alpine) | aarch64 | `nikki-apk-aarch64-<version>.run` |

---

### 4. SSR Plus FW3/FW4 (2 个文件)

| 格式 | 架构 | 文件名示例 |
|------|------|------------|
| IPK (OpenWrt) | x86_64 | `ssr-plus-ipk-x86_64-<version>.run` |
| IPK (OpenWrt) | aarch64 | `ssr-plus-ipk-aarch64-<version>.run` |

> **注意**：SSR Plus 目前仅支持 IPK 格式（OpenWrt），APK 格式暂不可用。

---

## 🔧 如何选择正确的防火墙模式

### 检查当前防火墙版本

```bash
# 查看防火墙版本
opkg list-installed | grep firewall

# 或
uci show firewall.@default[0].name
```

- **输出包含 `firewall3`** → 使用 **FW3 (iptables)** 模式
- **输出包含 `firewall4`** → 使用 **FW4 (nftables)** 模式
- **OpenWrt 21.02 及以下** → FW3 模式
- **OpenWrt 22.03 及以上** → FW4 模式

---

## ❓ 常见问题

### Q1: 安装时提示 "kernel (= xxx) 依赖缺失"

**解决方案：**
```bash
# 使用强制安装模式
opkg install --force-depends *.ipk
```

### Q2: OpenClash 无法启动

**解决方案：**
1. 检查内核是否已下载：`ls -la /etc/openclash/core/`
2. 如果没有内核文件，进入 Luci → OpenClash → 版本更新 → 下载内核
3. 手动下载内核并放置到 `/etc/openclash/core/`，命名为 `clash_meta`

### Q3: 如何查看已安装的版本

```bash
opkg list-installed | grep -E "(passwall|openclash|nikki|ssr-plus)"
```

### Q4: 如何卸载

```bash
# 卸载 Passwall
opkg remove luci-app-passwall

# 卸载 OpenClash
opkg remove luci-app-openclash

# 卸载 Nikki
opkg remove luci-app-nikki

# 卸载 SSR Plus
opkg remove luci-app-ssr-plus
```

### Q5: 在菜单中看不到安装的插件

请注销或者重启一下系统

---


```

## 在 action yaml中使用

可以这样调用：

```yaml
      
    - name: Build passwall run files
      uses: sirpdboy/buildrun@passwall
      with:
        OUTPUT_DIR: "./pkgrun"
      
    - name: Build passwall2 run files
      uses: sirpdboy/buildrun@passwall2
      with:
        OUTPUT_DIR: "./pkgrun"
      
    - name: Build openclash run files
      uses: sirpdboy/buildrun@openclash
      with:
        OUTPUT_DIR: "./pkgrun"
      
    - name: Build nikki run files
      uses: sirpdboy/buildrun@nikki
      with:
        OUTPUT_DIR: "./pkgrun"
      
    - name: Build ssrp run files
      uses: sirpdboy/buildrun@ssrp
      with:
        OUTPUT_DIR: "./pkgrun"
```


<details>
<summary><h2>鸣谢和引用的项目</h2></summary>
  
 【打包】https://github.com/megastep/makeself<br>
 【引用】https://github.com/Openwrt-Passwall/openwrt-passwall<br>
 【引用】https://github.com/Openwrt-Passwall/openwrt-passwall2<br>
 【引用】https://github.com/vernesong/OpenClash<br>
 【引用】https://dl.openwrt.ai<br>
 【引用】https://github.com/wukongdaily/RunFilesBuilder/<br>
 【引用】https://github.com/morytyann/OpenWrt-mihomo/wiki<br>
