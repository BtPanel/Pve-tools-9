# PVE Tools 9 🚀

<div align="center">

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Shell Script](https://img.shields.io/badge/Shell-Script-4EAA25?logo=gnu-bash&logoColor=white)](https://www.gnu.org/software/bash/)
[![Proxmox VE](https://img.shields.io/badge/Proxmox-VE%209.0-E57000?logo=proxmox&logoColor=white)](https://www.proxmox.com/)
[![Debian](https://img.shields.io/badge/Debian-13%20(Trixie)-A81D33?logo=debian&logoColor=white)](https://www.debian.org/)

---

```
██████╗ ██╗   ██╗███████╗    ████████╗ ██████╗  ██████╗ ██╗     ███████╗     █████╗
██╔══██╗██║   ██║██╔════╝    ╚══██╔══╝██╔═══██╗██╔═══██╗██║     ██╔════╝    ██╔══██╗
██████╔╝██║   ██║█████╗         ██║   ██║   ██║██║   ██║██║     ███████╗    ╚██████║
██╔═══╝ ╚██╗ ██╔╝██╔══╝         ██║   ██║   ██║██║   ██║██║     ╚════██║     ╚═══██║
██║      ╚████╔╝ ███████╗       ██║   ╚██████╔╝╚██████╔╝███████╗███████║     █████╔╝
╚═╝       ╚═══╝  ╚══════╝       ╚═╝    ╚═════╝  ╚═════╝ ╚══════╝╚══════╝     ╚════╝
```

**🎯 一键配置神器，让 PVE 配置变得简单快乐**

</div>

---

### 🚪 开门见山

#### 中国大陆网络

```
bash <(curl -sSL https://ghfast.top/raw.githubusercontent.com/BtPanel/Pve-tools-9/refs/heads/main/PVE-Tools.sh)
```

#### 国际网络

```
bash <(curl -sSL https://raw.githubusercontent.com/BtPanel/Pve-tools-9/refs/heads/main/PVE-Tools.sh)
```

---

### 📖 项目简介

PVE Tools 9 是专为 Proxmox VE 9.0 设计的一键配置工具，基于 Debian 13 (Trixie) 系统。本工具旨在简化 PVE
的初始配置过程，提供友好的用户界面和安全的操作体验。

<div align="center">


</div>

### ✨ 主要特性

- 🚀 **一键换源** - 自动配置清华大学镜像源，大幅提升下载速度
- 🚫 **删除订阅弹窗** - 彻底消除烦人的订阅提醒
- 💾 **存储优化** - 智能合并 local 与 local-lvm 存储
- 🔄 **Swap 管理** - 可选删除 Swap 分区释放更多空间
- 📦 **系统更新** - 安全的系统升级和清理
- 📊 **系统监控** - 实时显示系统运行状况
- 🔧 **硬件直通** - 轻松配置 PCI 设备直通功能
- ⚙️ **CPU 电源管理** - 灵活调整 CPU 性能模式
- 🌡️ **温度监控** - 实时显示 CPU 和硬盘温度
- 🐙 **Ceph 支持** - 支持 ceph-squid 和 ceph-quincy 源
- 🎨 **美观界面** - 彩色输出和友好的用户交互
- 🛡️ **安全备份** - 操作前自动备份重要文件

### 🎯 支持的功能

| 功能          | 描述                            | 推荐度   |
|-------------|-------------------------------|-------|
| 🚀 更换软件源    | 配置清华镜像源，包含 Debian、PVE、Ceph 源  | ⭐⭐⭐⭐⭐ |
| 🚫 删除订阅弹窗   | 移除"无有效订阅"提醒弹窗                 | ⭐⭐⭐⭐⭐ |
| 💾 合并存储     | 合并 local 与 local-lvm（适合小硬盘）   | ⭐⭐⭐   |
| 🔄 删除 Swap  | 释放 Swap 空间给系统使用               | ⭐⭐⭐   |
| 📦 系统更新     | 更新系统软件包到最新版本                  | ⭐⭐⭐⭐  |
| 📊 系统信息     | 查看 PVE 系统运行状态                 | ⭐⭐⭐⭐  |
| 🔧 硬件直通     | 配置 PCI 设备直通功能                 | ⭐⭐⭐⭐  |
| ⚙️ CPU 电源模式 | 调整 CPU 性能模式（节能/性能等）           | ⭐⭐⭐   |
| 🌡️ 温度监控    | 实时显示 CPU 和硬盘温度                | ⭐⭐⭐⭐  |
| 🐙 Ceph 源   | 支持 ceph-squid 和 ceph-quincy 源 | ⭐⭐⭐   |
| 🗑️ Ceph 卸载 | 完全移除 Ceph 相关组件                | ⭐⭐    |

### 🚀 快速开始

#### 系统要求

- ✅ Proxmox VE 9.0 或更高版本
- ✅ Debian 13 (Trixie) 基础系统
- ✅ Root 权限
- ✅ 网络连接

#### 安装使用

```bash
# 1. 下载脚本
wget https://raw.githubusercontent.com/siyrs/pve-tools-9/main/PVE-Tools.sh

# 2. 添加执行权限
chmod +x PVE-Tools.sh

# 3. 运行脚本
sudo ./PVE-Tools.sh
```

运行脚本后，您将看到包含以下选项的菜单：

1. 🚀 更换软件源 - 配置清华大学镜像源
2. 🚫 删除订阅弹窗 - 移除订阅提醒
3. 💾 合并存储 - 合并 local 与 local-lvm
4. 🔄 删除 Swap - 释放 Swap 空间
5. 📦 系统更新 - 更新系统软件包
6. 📊 系统信息 - 查看系统运行状态
7. ⚡ 一键配置 - 自动执行换源、删除弹窗和系统更新
8. 🔧 硬件直通配置 - 配置 PCI 设备直通
9. ⚙️ CPU 电源模式 - 调整 CPU 性能模式
10. 🌡️ 温度监控设置 - 添加温度监控功能
11. 🗑️ 移除温度监控 - 移除温度监控功能
12. 🐙 添加 ceph-squid 源 - 为 PVE 8/9 添加 Ceph 源
13. 🐙 添加 ceph-quincy 源 - 为 PVE 7/8 添加 Ceph 源
14. 🗑️ 卸载 Ceph - 完全移除 Ceph 组件

> 💡 **调试模式**: 开发者和高级用户可以使用 `sudo ./PVE-Tools.sh --debug` 命令启动调试模式。此模式将跳过 PVE
> 系统检测，但会显示严重警告，因为在此模式下在非 PVE 系统上运行可能导致系统损坏。

#### 一键配置（推荐新用户）

```bash
# 直接运行并选择选项 7 进行一键配置
sudo ./PVE-Tools.sh
# 然后输入 7 选择一键配置
```

### 📋 详细功能说明

#### 🚀 更换软件源

- **Debian 源**: 使用 DEB822 格式配置清华大学镜像
- **企业源**: 自动注释 PVE 企业源（需付费）
- **Ceph 源**: 配置 Ceph 存储镜像源
- **无订阅源**: 添加适用于社区版的免费源
- **CT 模板源**: 加速容器模板下载

#### 🚫 删除订阅弹窗

自动修改 `proxmoxlib.js` 文件，彻底移除"No valid subscription"弹窗提醒。

#### 💾 存储管理

**合并 local 与 local-lvm**:

- 适用于小容量系统盘
- 自动备份配置
- 安全的 LVM 操作

**删除 Swap 分区**:

- 释放 Swap 空间给系统使用
- 适合内存充足的环境
- 自动修改 fstab 配置

#### 🔧 硬件直通配置

**开启硬件直通**:

- 自动检测 CPU 类型（Intel/AMD）
- 配置 IOMMU 设置
- 添加 VFIO 驱动模块
- 设置显卡和音频设备黑名单

**关闭硬件直通**:

- 恢复原始 GRUB 配置
- 移除 VFIO 相关设置
- 删除黑名单配置

#### ⚙️ CPU 电源模式

支持多种 CPU 性能模式：

- **Performance**: 高性能模式（默认）
- **Powersave**: 节能模式
- **Ondemand**: 按需调频模式
- **Conservative**: 保守调频模式
- **Schedutil**: 负载优化模式

#### 🌡️ 温度监控

**添加温度监控**:

- 安装 lm-sensors、nvme-cli 等工具
- 自动检测硬件传感器
- 修改 PVE Web UI 显示 CPU/主板/硬盘温度
- 支持 NVME 和 SATA 硬盘温度显示

**删除温度监控**:

- 恢复原始 PVE Web UI 文件
- 移除相关工具和配置

#### 🐙 Ceph 存储支持

**添加 ceph-squid 源**:

- 适用于 PVE 8/9
- 配置清华大学镜像源

**添加 ceph-quincy 源**:

- 适用于 PVE 7/8
- 配置清华大学镜像源

**卸载 Ceph**:

- 停止所有 Ceph 服务
- 删除 Ceph 相关软件包
- 清理配置文件和数据

### ⚠️ 注意事项

- 🔒 **权限要求**: 必须使用 root 权限运行
- 💾 **数据备份**: 重要操作前会自动备份配置文件
- 🌐 **网络需求**: 换源功能需要稳定的网络连接
- ⚡ **内存要求**: 删除 Swap 前请确保内存充足
- 🔧 **硬件直通**: 需要硬件支持 IOMMU/VT-d 功能
- 🌡️ **温度监控**: 需要硬件支持传感器检测
- 🐙 **Ceph 功能**: 请根据您的 PVE 版本选择合适的 Ceph 源

### 🐛 故障排除

#### 常见问题

**Q: 脚本提示"不是 PVE 环境"?**
A: 请确保您在 Proxmox VE 系统上运行此脚本。

**Q: 换源后更新失败?**
A: 请检查网络连接，或尝试重新运行换源功能。

**Q: 删除弹窗后仍然出现?**
A: 请清除浏览器缓存或使用无痕模式访问。

#### 获取帮助

如遇到问题，请：

1. 📋 查看脚本运行日志
2. 🔍 检查系统环境是否符合要求
3. 💬 在 GitHub Issues 中提交问题

---

## 📄 开源协议

本项目采用 MIT 协议发布，详见 [LICENSE](LICENSE) 文件。

```
MIT License

Copyright (c) 2025 Siyrs

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
