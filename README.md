<div align="center">
<img width="768" src="https://cdn.jsdelivr.net/gh/hubhike/OpenWrtNin1/images/openwrt.png"/>
<h1>OpenWrt — 多设备固件云编译</h1>

<img src="https://img.shields.io/github/downloads/hubhike/OpenWrtNin1/total.svg?style=for-the-badge&color=32C955"/>
<img src="https://img.shields.io/github/stars/hubhike/OpenWrtNin1.svg?style=for-the-badge&color=orange"/>
<img src="https://img.shields.io/github/forks/hubhike/OpenWrtNin1.svg?style=for-the-badge&color=ff69b4"/>
<img src="https://img.shields.io/github/license/hubhike/OpenWrtNin1.svg?style=for-the-badge&color=blueviolet"/>

[![](https://img.shields.io/badge/-目录:-696969.svg)](#readme) [![](https://img.shields.io/badge/-项目说明-FFFFFF.svg)](#项目说明-) [![](https://img.shields.io/badge/-固件特色-FFFFFF.svg)](#固件特色-) [![](https://img.shields.io/badge/-固件下载-FFFFFF.svg)](#固件下载-) [![](https://img.shields.io/badge/-近期更新-FFFFFF.svg)](#近期更新-) [![](https://img.shields.io/badge/-插件预览-FFFFFF.svg)](#插件预览-) [![](https://img.shields.io/badge/-定制固件-FFFFFF.svg)](#定制固件-) [![](https://img.shields.io/badge/-特别提示-FFFFFF.svg)](#特别提示-) [![](https://img.shields.io/badge/-鸣谢-FFFFFF.svg)](#鸣谢-)
</div>


## 项目说明 [![](https://img.shields.io/badge/-项目基本介绍-FFFFFF.svg)](#项目说明-)
- 固件构成：[![Lean](https://img.shields.io/badge/Lede-Lean-ff69b4.svg?style=flat&logo=appveyor)](https://github.com/coolsnowwolf/lede) [![P3TERX](https://img.shields.io/badge/OpenWrt-P3TERX-blueviolet.svg?style=flat&logo=appveyor)](https://github.com/P3TERX/Actions-OpenWrt) [![Flippy](https://img.shields.io/badge/Package-Flippy-orange.svg?style=flat&logo=appveyor)](https://github.com/unifreq/openwrt_packit) [![Haiibo](https://img.shields.io/badge/Build-Haiibo-32C955.svg?style=flat&logo=appveyor)](https://github.com/hubhike/OpenWrtNin1)
- 项目使用 Github Actions 拉取 [Lean](https://github.com/coolsnowwolf/lede) 的 Openwrt 源码仓库进行云编译
- 固件默认管理地址：`192.168.1.1` 默认用户：`root` 默认密码：`password`
- 提供适配于 ARMv8 电视盒子、Rockchip 平台、树莓派以及 X86 平台设备的 OpenWrt 固件
- ARMv8 盒子固件分为 [Mini版](https://github.com/hubhike/OpenWrtNin1/releases/tag/ARMv8_MINI) 和 [Plus版](https://github.com/hubhike/OpenWrtNin1/releases/tag/ARMv8_PLUS)，Mini 精简版以科学上网为主，Plus 多功能版插件多适合折腾
- ARMv8 系列固件包含 [F大](https://github.com/unifreq/openwrt_packit) 发布的所有已适配的盒子固件，并提供 Docker 镜像固件[➦使用方法](https://hub.docker.com/r/summary/openwrt-aarch64)
- 固件集成的所有 ipk 插件全部打包在 Packages 文件中，可以在 [Releases](https://github.com/hubhike/OpenWrtNin1/releases) 内进行下载
- 项目编译的固件插件为最新版本，最新版插件可能有 BUG，如果之前使用稳定则无需追新
- 第一次使用请采用全新安装，避免出现升级失败以及其他一些可能的 BUG


## 固件特色 [![](https://img.shields.io/badge/-本项目固件特色-FFFFFF.svg)](#固件特色-)
1. 固件每天定时自动编译，以确保获得最新体验
2. 集成部分常用有线、无线、3G / 4G 网卡驱动
3. 集成中文版 netdata 实时监控插件，小白也能轻松看懂系统概况
4. 集成 iStore 应用商店，可根据自己需求自由安装所需插件
5. 集成 Docker 服务，可在 OpenWrt 内自由部署 Docker 应用
6. 集成应用过滤插件，支持游戏、视频、聊天、下载等 APP 过滤
7. 集成在线用户插件，可查看所有在线用户 IP 地址与实时速率等
8. ARMv8 系列固件内置晶晨宝盒，支持在线更新固件及内核等


## 固件下载 [![](https://img.shields.io/badge/-编译状态及下载链接-FFFFFF.svg)](#固件下载-)
点击下表中 [![](https://img.shields.io/badge/下载-链接-blueviolet.svg?style=flat&logo=hack-the-box)](https://github.com/hubhike/OpenWrtNin1/releases) 即可跳转到该设备固件下载页面
| 平台+设备名称 | 固件编译状态 | 配置文件 | 固件下载 |
| :-------------: | :-------------: | :-------------: | :-------------: |
| [![](https://img.shields.io/badge/OpenWrt-X86_64位-32C955.svg?logo=openwrt)](https://github.com/hubhike/OpenWrtNin1/blob/main/.github/workflows/X86_64-OpenWrt.yml) | [![](https://github.com/hubhike/OpenWrtNin1/actions/workflows/X86_64-OpenWrt.yml/badge.svg)](https://github.com/hubhike/OpenWrtNin1/actions/workflows/X86_64-OpenWrt.yml) | [![](https://img.shields.io/badge/编译-配置-orange.svg?logo=apache-spark)](https://github.com/hubhike/OpenWrtNin1/blob/main/configs/x86_64.config) | [![](https://img.shields.io/badge/下载-链接-blueviolet.svg?logo=hack-the-box)](https://github.com/hubhike/OpenWrtNin1/releases/tag/X86_64) |
| [![](https://img.shields.io/badge/OpenWrt-ARMv8_Mini-32C955.svg?logo=openwrt)](https://github.com/hubhike/OpenWrtNin1/blob/main/.github/workflows/ARMv8-Mini-OpenWrt.yml) | [![](https://github.com/hubhike/OpenWrtNin1/actions/workflows/ARMv8-Mini-OpenWrt.yml/badge.svg)](https://github.com/hubhike/OpenWrtNin1/actions/workflows/ARMv8-Mini-OpenWrt.yml) | [![](https://img.shields.io/badge/编译-配置-orange.svg?logo=apache-spark)](https://github.com/hubhike/OpenWrtNin1/blob/main/configs/armv8-mini.config) | [![](https://img.shields.io/badge/下载-链接-blueviolet.svg?logo=hack-the-box)](https://github.com/hubhike/OpenWrtNin1/releases/tag/ARMv8_MINI) |
| [![](https://img.shields.io/badge/OpenWrt-ARMv8_Plus-32C955.svg?logo=openwrt)](https://github.com/hubhike/OpenWrtNin1/blob/main/.github/workflows/ARMv8-Plus-OpenWrt.yml) | [![](https://github.com/hubhike/OpenWrtNin1/actions/workflows/ARMv8-Plus-OpenWrt.yml/badge.svg)](https://github.com/hubhike/OpenWrtNin1/actions/workflows/ARMv8-Plus-OpenWrt.yml) | [![](https://img.shields.io/badge/编译-配置-orange.svg?logo=apache-spark)](https://github.com/hubhike/OpenWrtNin1/blob/main/configs/armv8-plus.config) | [![](https://img.shields.io/badge/下载-链接-blueviolet.svg?logo=hack-the-box)](https://github.com/hubhike/OpenWrtNin1/releases/tag/ARMv8_PLUS) |
| [![](https://img.shields.io/badge/OpenWrt-Rockchip_平台-32C955.svg?logo=openwrt)](https://github.com/hubhike/OpenWrtNin1/blob/main/.github/workflows/Rockchip-OpenWrt.yml) | [![](https://github.com/hubhike/OpenWrtNin1/actions/workflows/Rockchip-OpenWrt.yml/badge.svg)](https://github.com/hubhike/OpenWrtNin1/actions/workflows/Rockchip-OpenWrt.yml) | [![](https://img.shields.io/badge/编译-配置-orange.svg?logo=apache-spark)](https://github.com/hubhike/OpenWrtNin1/blob/main/configs/rockchip.config) | [![](https://img.shields.io/badge/下载-链接-blueviolet.svg?logo=hack-the-box)](https://github.com/hubhike/OpenWrtNin1/releases/tag/Rockchip) |
| [![](https://img.shields.io/badge/OpenWrt-树莓派_4B-32C955.svg?logo=openwrt)](https://github.com/hubhike/OpenWrtNin1/blob/main/.github/workflows/RaspberryPi4-OpenWrt.yml) | [![](https://github.com/hubhike/OpenWrtNin1/actions/workflows/RaspberryPi4-OpenWrt.yml/badge.svg)](https://github.com/hubhike/OpenWrtNin1/actions/workflows/RaspberryPi4-OpenWrt.yml) | [![](https://img.shields.io/badge/编译-配置-orange.svg?logo=apache-spark)](https://github.com/hubhike/OpenWrtNin1/blob/main/configs/rpi4.config) | [![](https://img.shields.io/badge/下载-链接-blueviolet.svg?logo=hack-the-box)](https://github.com/hubhike/OpenWrtNin1/releases/tag/RaspberryPi4) |
| [![](https://img.shields.io/badge/OpenWrt-树莓派_3B/3B+-32C955.svg?logo=openwrt)](https://github.com/hubhike/OpenWrtNin1/blob/main/.github/workflows/RaspberryPi3-OpenWrt.yml) | [![](https://github.com/hubhike/OpenWrtNin1/actions/workflows/RaspberryPi3-OpenWrt.yml/badge.svg)](https://github.com/hubhike/OpenWrtNin1/actions/workflows/RaspberryPi3-OpenWrt.yml) | [![](https://img.shields.io/badge/编译-配置-orange.svg?logo=apache-spark)](https://github.com/hubhike/OpenWrtNin1/blob/main/configs/rpi3.config) | [![](https://img.shields.io/badge/下载-链接-blueviolet.svg?logo=hack-the-box)](https://github.com/hubhike/OpenWrtNin1/releases/tag/RaspberryPi3) |


## 固件下载 https://github.com/haiibo/OpenWrt [![](https://img.shields.io/badge/-编译状态及下载链接-FFFFFF.svg)](#固件下载-)
点击下表中 [![](https://img.shields.io/badge/下载-链接-blueviolet.svg?style=flat&logo=hack-the-box)](https://github.com/haiibo/OpenWrt/releases) 即可跳转到该设备固件下载页面
| 平台+设备名称 | 固件编译状态 | 配置文件 | 固件下载 |
| :-------------: | :-------------: | :-------------: | :-------------: |
| [![](https://img.shields.io/badge/OpenWrt-X86_64位-32C955.svg?logo=openwrt)](https://github.com/haiibo/OpenWrt/blob/main/.github/workflows/X86_64-OpenWrt.yml) | [![](https://github.com/haiibo/OpenWrt/actions/workflows/X86_64-OpenWrt.yml/badge.svg)](https://github.com/haiibo/OpenWrt/actions/workflows/X86_64-OpenWrt.yml) | [![](https://img.shields.io/badge/编译-配置-orange.svg?logo=apache-spark)](https://github.com/haiibo/OpenWrt/blob/main/configs/x86_64.config) | [![](https://img.shields.io/badge/下载-链接-blueviolet.svg?logo=hack-the-box)](https://github.com/haiibo/OpenWrt/releases/tag/X86_64) |
| [![](https://img.shields.io/badge/OpenWrt-ARMv8_Mini-32C955.svg?logo=openwrt)](https://github.com/haiibo/OpenWrt/blob/main/.github/workflows/ARMv8-Mini-OpenWrt.yml) | [![](https://github.com/haiibo/OpenWrt/actions/workflows/ARMv8-Mini-OpenWrt.yml/badge.svg)](https://github.com/haiibo/OpenWrt/actions/workflows/ARMv8-Mini-OpenWrt.yml) | [![](https://img.shields.io/badge/编译-配置-orange.svg?logo=apache-spark)](https://github.com/haiibo/OpenWrt/blob/main/configs/armv8-mini.config) | [![](https://img.shields.io/badge/下载-链接-blueviolet.svg?logo=hack-the-box)](https://github.com/haiibo/OpenWrt/releases/tag/ARMv8_MINI) |
| [![](https://img.shields.io/badge/OpenWrt-ARMv8_Plus-32C955.svg?logo=openwrt)](https://github.com/haiibo/OpenWrt/blob/main/.github/workflows/ARMv8-Plus-OpenWrt.yml) | [![](https://github.com/haiibo/OpenWrt/actions/workflows/ARMv8-Plus-OpenWrt.yml/badge.svg)](https://github.com/haiibo/OpenWrt/actions/workflows/ARMv8-Plus-OpenWrt.yml) | [![](https://img.shields.io/badge/编译-配置-orange.svg?logo=apache-spark)](https://github.com/haiibo/OpenWrt/blob/main/configs/armv8-plus.config) | [![](https://img.shields.io/badge/下载-链接-blueviolet.svg?logo=hack-the-box)](https://github.com/haiibo/OpenWrt/releases/tag/ARMv8_PLUS) |
| [![](https://img.shields.io/badge/OpenWrt-Rockchip_平台-32C955.svg?logo=openwrt)](https://github.com/haiibo/OpenWrt/blob/main/.github/workflows/Rockchip-OpenWrt.yml) | [![](https://github.com/haiibo/OpenWrt/actions/workflows/Rockchip-OpenWrt.yml/badge.svg)](https://github.com/haiibo/OpenWrt/actions/workflows/Rockchip-OpenWrt.yml) | [![](https://img.shields.io/badge/编译-配置-orange.svg?logo=apache-spark)](https://github.com/haiibo/OpenWrt/blob/main/configs/rockchip.config) | [![](https://img.shields.io/badge/下载-链接-blueviolet.svg?logo=hack-the-box)](https://github.com/haiibo/OpenWrt/releases/tag/Rockchip) |
| [![](https://img.shields.io/badge/OpenWrt-树莓派_4B-32C955.svg?logo=openwrt)](https://github.com/haiibo/OpenWrt/blob/main/.github/workflows/RaspberryPi4-OpenWrt.yml) | [![](https://github.com/haiibo/OpenWrt/actions/workflows/RaspberryPi4-OpenWrt.yml/badge.svg)](https://github.com/haiibo/OpenWrt/actions/workflows/RaspberryPi4-OpenWrt.yml) | [![](https://img.shields.io/badge/编译-配置-orange.svg?logo=apache-spark)](https://github.com/haiibo/OpenWrt/blob/main/configs/rpi4.config) | [![](https://img.shields.io/badge/下载-链接-blueviolet.svg?logo=hack-the-box)](https://github.com/haiibo/OpenWrt/releases/tag/RaspberryPi4) |
| [![](https://img.shields.io/badge/OpenWrt-树莓派_3B/3B+-32C955.svg?logo=openwrt)](https://github.com/haiibo/OpenWrt/blob/main/.github/workflows/RaspberryPi3-OpenWrt.yml) | [![](https://github.com/haiibo/OpenWrt/actions/workflows/RaspberryPi3-OpenWrt.yml/badge.svg)](https://github.com/haiibo/OpenWrt/actions/workflows/RaspberryPi3-OpenWrt.yml) | [![](https://img.shields.io/badge/编译-配置-orange.svg?logo=apache-spark)](https://github.com/haiibo/OpenWrt/blob/main/configs/rpi3.config) | [![](https://img.shields.io/badge/下载-链接-blueviolet.svg?logo=hack-the-box)](https://github.com/haiibo/OpenWrt/releases/tag/RaspberryPi3) |

## 近期更新 [![](https://img.shields.io/badge/-近期固件更新-FFFFFF.svg)](#近期更新-)
🤣努力修复中……


## 插件预览 [![](https://img.shields.io/badge/-固件插件及功能预览-FFFFFF.svg)](#插件预览-)
<details>
<summary><b>&nbsp;ARMv8 盒子 Mini 精简版本插件预览</b></summary>
<br/>
<img src="https://cdn.jsdelivr.net/gh/hubhike/OpenWrtNin1/images/mini.png"/>
</details>

<details>
<summary><b>&nbsp;ARMv8 盒子 Plus 多功能版插件预览</b></summary>
<br/>
<img src="https://cdn.jsdelivr.net/gh/hubhike/OpenWrtNin1/images/plus.png"/>
</details>

<details>
<summary><b>&nbsp;X86、R2S、R4S 等软路由插件预览</b></summary>
<br/>
<details>
<summary><b>├── 状态</b></summary>
　├── 概况<br/>
　├── 防火墙<br/>
　├── 路由表<br/>
　├── 系统日志<br/>
　├── 内核日志<br/>
　├── 系统进程<br/>
　├── 实时信息<br/>
　├── 实时监控<br/>
　├── 在线用户<br/>
　├── WireGuard 状态<br/>
　├── 负载均衡<br/>
　└── 释放内存
</details>
<details>
<summary><b>├── 系统</b></summary>
　├── 系统<br/>
　├── 管理权<br/>
　├── TTYD 终端<br/>
　├── 软件包<br/>
　├── 启动项<br/>
　├── 计划任务<br/>
　├── 挂载点<br/>
　├── 磁盘管理<br/>
　├── 备份/升级<br/>
　├── 自定义命令<br/>
　├── 定时重启<br/>
　├── 文件传输<br/>
　├── Argon 主题设置<br/>
　├── 重启<br/>
　└── 关机
</details>
<details>
<summary><b>├── 服务</b></summary>
　├── PassWall<br/>
　├── PassWall2<br/>
　├── Hello World<br/>
　├── iKoolProxy 滤广告<br/>
　├── V2ray 服务器<br/>
　├── 广告屏蔽大师 Plus+<br/>
　├── ShadowSocksR Plus+<br/>
　├── AdGuard Home<br/>
　├── 应用过滤<br/>
　├── MosDNS<br/>
　├── 全能推送<br/>
　├── 微信推送<br/>
　├── 上网时间控制<br/>
　├── 解锁网易云灰色歌曲<br/>
　├── OpenClash<br/>
　├── 动态 DNS<br/>
　├── MultiSD_Lite<br/>
　├── SmartDNS<br/>
　├── 网络唤醒<br/>
　├── 迅雷快鸟<br/>
　├── Frps<br/>
　├── UU游戏加速器<br/>
　├── UPnP<br/>
　├── KMS 服务器<br/>
　├── AirPlay 2 音频接收<br/>
　├── udpxy<br/>
　├── Nps 内网穿透<br/>
　├── uHTTPd<br/>
　├── Frp 内网穿透<br/>
　└── MWAN3 分流助手
</details>
<details>
<summary><b>├── Docker</b></summary>
　├── 概览<br/>
　├── 容器<br/>
　├── 镜像<br/>
　├── 网络<br/>
　├── 存储卷<br/>
　├── 事件<br/>
　└── 设置
</details>
<details>
<summary><b>├── 网络存储</b></summary>
　├── 文件浏览器<br/>
　├── 可道云<br/>
　├── NFS 管理<br/>
　├── 微力同步<br/>
　├── Alist 文件列表<br/>
　├── qBittorrent<br/>
　├── USB 打印服务器<br/>
　├── 硬盘休眠<br/>
　├── 挂载 SMB 网络共享<br/>
　├── 网络共享<br/>
　├── FTP 服务器<br/>
　├── Rclone<br/>
　├── Aria2 配置<br/>
　├── miniDLNA<br/>
　└── Transmission
</details>
<details>
<summary><b>├── VPN</b></summary>
　├── N2N v2 VPN<br/>
　├── SoftEther VPN 服务器<br/>
　├── OpenVPN 服务器<br/>
　├── PPTP VPN 服务器<br/>
　├── IPSec VPN 服务器<br/>
　└── ZeroTier
</details>
<details>
<summary><b>├── 网络</b></summary>
　├── 接口<br/>
　├── DHCP/DNS<br/>
　├── 主机名<br/>
　├── IP/MAC 绑定<br/>
　├── 静态路由<br/>
　├── 防火墙<br/>
　├── 诊断<br/>
　├── Socat<br/>
　├── SQM QoS<br/>
　├── 网速控制<br/>
　├── 多线多拨<br/>
　├── 负载均衡<br/>
　└── Turbo ACC 网络加速
</details>
<details>
<summary><b>├── 带宽监控</b></summary>
　├── 显示<br/>
　├── 配置<br/>
　├── 备份<br/>
　├── 网速监控<br/>
　└── 实时流量监测
</details>
　└── <b>退出</b>
</details>


## 定制固件 [![](https://img.shields.io/badge/-项目基本编译教程-FFFFFF.svg)](#定制固件-)
1. 首先要登录 Gihub 账号，然后 Fork 此项目到你自己的 Github 仓库
2. 修改 `configs` 目录对应文件添加或删除插件，或者上传自己的 `xx.config` 配置文件
3. 插件对应名称及功能请参考恩山网友帖子：[Applications 添加插件应用说明](https://www.right.com.cn/forum/thread-3682029-1-1.html)
4. 如需修改默认 IP、添加或删除插件包以及一些其他设置请在 `diy-script.sh` 文件内修改
5. 添加或修改 `xx.yml` 文件，最后点击 `Actions` 运行要编译的 `workflow` 即可开始编译
6. 编译大概需要3-5小时，编译完成后在仓库主页 [Releases](https://github.com/hubhike/OpenWrtNin1/releases) 对应 Tag 标签内下载固件
<details>
<summary><b>&nbsp;如果你觉得修改 config 文件麻烦，那么你可以点击此处尝试本地提取</b></summary>

1. 首先装好 Linux 系统，推荐 Debian 11 或 Ubuntu LTS

2. 安装编译依赖环境

   ```bash
   sudo apt update -y
   sudo apt full-upgrade -y
   sudo apt install -y ack antlr3 asciidoc autoconf automake autopoint binutils bison build-essential \
   bzip2 ccache cmake cpio curl device-tree-compiler fastjar flex gawk gettext gcc-multilib g++-multilib \
   git gperf haveged help2man intltool libc6-dev-i386 libelf-dev libglib2.0-dev libgmp3-dev libltdl-dev \
   libmpc-dev libmpfr-dev libncurses5-dev libncursesw5-dev libreadline-dev libssl-dev libtool lrzsz \
   mkisofs msmtp nano ninja-build p7zip p7zip-full patch pkgconf python2.7 python3 python3-pyelftools \
   libpython3-dev qemu-utils rsync scons squashfs-tools subversion swig texinfo uglifyjs upx-ucl unzip \
   vim wget xmlto xxd zlib1g-dev
   ```

3. 下载源代码，更新 feeds 并安装到本地

   ```bash
   git clone https://github.com/coolsnowwolf/lede
   cd lede
   ./scripts/feeds update -a
   ./scripts/feeds install -a
   ```

4. 复制 diy-script.sh 文件内所有内容到命令行，添加自定义插件和自定义设置

5. 命令行输入 `make menuconfig` 选择配置，选好配置后导出差异部分到 seed.config 文件

   ```bash
   make defconfig
   ./scripts/diffconfig.sh > seed.config
   ```

7. 命令行输入 `cat seed.config` 查看这个文件，也可以用文本编辑器打开

8. 复制 seed.config 文件内所有内容到 configs 目录对应文件中覆盖就可以了

   **如果看不懂编译界面可以参考 YouTube 视频：[软路由固件 OpenWrt 编译界面设置](https://www.youtube.com/watch?v=jEE_J6-4E3Y&list=WL&index=7)**
</details>


## 特别提示 [![](https://img.shields.io/badge/-个人免责声明-FFFFFF.svg)](#特别提示-)

- **因精力有限不提供任何技术支持和教程等相关问题解答，不保证完全无 BUG！**

- **本人不对任何人因使用本固件所遭受的任何理论或实际的损失承担责任！**

- **本固件禁止用于任何商业用途，请务必严格遵守国家互联网使用相关法律规定！**


## 鸣谢 [![](https://img.shields.io/badge/-跪谢各大佬-FFFFFF.svg)](#鸣谢-)
| [ImmortalWrt](https://github.com/immortalwrt) | [coolsnowwolf](https://github.com/coolsnowwolf) | [P3TERX](https://github.com/P3TERX) | [Flippy](https://github.com/unifreq) |
| :-------------: | :-------------: | :-------------: | :-------------: |
| <img width="100" src="https://avatars.githubusercontent.com/u/53193414"/> | <img width="100" src="https://avatars.githubusercontent.com/u/31687149"/> | <img width="100" src="https://avatars.githubusercontent.com/u/25927179"/> | <img width="100" src="https://avatars.githubusercontent.com/u/39355261"/> |
| [Ophub](https://github.com/ophub) | [SuLingGG](https://github.com/SuLingGG) | [QiuSimons](https://github.com/QiuSimons) | [IvanSolis1989](https://github.com/IvanSolis1989) |
| <img width="100" src="https://avatars.githubusercontent.com/u/68696949"/> | <img width="100" src="https://avatars.githubusercontent.com/u/22287562"/> | <img width="100" src="https://avatars.githubusercontent.com/u/45143996"/> | <img width="100" src="https://avatars.githubusercontent.com/u/44228691"/> |

恩山网友帖子：[Applications 添加插件应用说明]([https://www.right.com.cn/forum/thread-3682029-1-1.html](https://www.right.com.cn/forum/thread-344825-1-1.html))
<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">OpenWrt 编译 LuCI ---&gt; Applications 添加插件应用说明 【人人为我，我为人人】&nbsp;</span>

<span style="background-color:#FFFFFF;">2022.11.28 更新 ！！！</span>

<br>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">make menuconfig&nbsp;进入定制界面</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">进入编译选项配置界面,.按照需要配置.( ‘*’ 代表编入固件，‘M’ 表示编译成模块或者IPK包， ‘空’不编译 )</span>

<br>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">非常感谢大佬”L有大雕“更正补充，20181121</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">大佬源码仓库：</span>

[https://github.com/coolsnowwolf/lede](<https://github.com/coolsnowwolf/lede>)<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">内容仅供参考，请根据个人实际情况使用，如果出现问题则后果自负。</span>

<br>

<br>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">选择LuCI 配置 添加插件应用：</span>

<br>

<span style="background-color:#FFFFFF;">注：应用后面标记 “</span>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;">” 为最近新添加；标记“&nbsp;</span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">!</span></span>

<span style="background-color:#FFFFFF;">&nbsp;”与其他插件依赖或冲突。</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">-------------------------------------------------------------------------------------------------------------------</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-accesscontrol&nbsp;#访问时间控制</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-acme&nbsp;#ACME自动化证书管理环境（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-adblock&nbsp;#ADB广告过滤</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-adbyby-plus&nbsp;#广告屏蔽大师Plus +</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-adbyby&nbsp;#广告过滤大师（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-adguardhome&nbsp;#AdGuard home广告过滤（Le库以外的插件）</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-adkill&nbsp;#广告过滤（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-advanced-reboot&nbsp;#Linksys高级重启</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-advancedsetting&nbsp;#系统高级设置（Le库以外的插件）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-ahcp&nbsp;#Ad-Hoc配置协议(AHCP) ipv6 and 双栈 自动配置协议</span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;"></span></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">!</span></span>

<span style="background-color:#FFFFFF;"></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-airplay2&nbsp;#Apple AirPlay2 AirPlay无损音乐推流(安卓+IOS)</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-aliddns&nbsp;#阿里DDNS客户端（丢弃，集成至ddns）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-aliyundrive-fuse&nbsp;#阿里云盘FUSE磁盘挂载</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-aliyundrive-webdav&nbsp;#阿里云盘 WebDAV 服务</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-amule&nbsp;#aMule下载工具</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">!</span></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;"></span></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-argon-config&nbsp;#Argon主题配置插件（Le库以外的插件）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-aria2 # Aria2下载工具</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-arpbind&nbsp;#IP/MAC绑定</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-asterisk&nbsp;#支持Asterisk电话服务器</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-attendedsysupgrade&nbsp;#固件更新升级相关</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-autoreboot&nbsp;#支持计划重启</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-baidupcs-web&nbsp;#百度网盘管理</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-bcp38&nbsp;#BCP38网络入口过滤（不确定）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-bird1-ipv4&nbsp;#对Bird1-ipv4的支持</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-bird1-ipv6&nbsp;#对Bird1-ipv6的支持</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-bird4&nbsp;#Bird 4（未知）（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-bird6&nbsp;#Bird 6（未知）（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-bmx6&nbsp;#BMX6路由协议</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-bmx7&nbsp;#BMX7路由协议（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-caldav&nbsp;#联系人（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-cifs-mount&nbsp;#CIFS/SMB挂载设置</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-cifsd&nbsp;#CIFS/SMB网络共享</span>

<span style="background-color:#FFFFFF;"></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-cjdns&nbsp;#加密IPV6网络相关</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-clamav&nbsp;#ClamAV杀毒软件</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-clash&nbsp;#Clash客户端（Le库以外的插件）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-commands&nbsp;#Shell命令模块</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-cshark&nbsp;#CloudShark捕获工具</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-dawn&nbsp;#分布式AP管理程序</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-ddns&nbsp;#动态域名 DNS（集成阿里DDNS客户端）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-diag-core&nbsp;#core诊断工具</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-diskman&nbsp;#磁盘管理工具</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> luci-app-diskman ---&gt; Include btrfs-progs&nbsp;#新型的写时复制 (COW)</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> luci-app-diskman ---&gt; Include lsblk&nbsp;#lsblk命令 用于列出所有可用块设备的信息</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> luci-app-diskman ---&gt; Include mdadm&nbsp;#mdadm命令 用于创建、管理、监控RAID设备的工具</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-diskman ---&gt; Include kmod-md-raid456&nbsp;#RAID 4,5,6 驱动程序模块（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-diskman ---&gt; Include kmod-md-linear&nbsp;#RAID 驱动程序模块（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-dnscrypt-proxy&nbsp;#DNSCrypt解决DNS污染</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-dnsfilter&nbsp;#DNSFilter基于DNS的广告过滤</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-dnsforwarder&nbsp;#DNSForwarder防DNS污染</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-dnspod&nbsp;#DNSPod动态域名解析（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-docker&nbsp;#Docker容器</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-dockerman&nbsp;#Dockerman容器</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-dump1090&nbsp;#民航无线频率（不确定）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-dynapoint&nbsp;#DynaPoint（未知）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-e2guardian&nbsp;#Web内容过滤器</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-easymesh&nbsp;#简单MESH(可有线+无线回程)</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-eqos&nbsp;#基于IP地址限速（Le库以外的插件）</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-familycloud&nbsp;#家庭云盘（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-fileassistant&nbsp;#文件管理助手（Le库以外的插件）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-filetransfer&nbsp;#文件传输（可web安装ipk包）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-firewall&nbsp;#添加防火墙</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-flowoffload&nbsp;#Turbo ACC网络加速（集成FLOW,BBR,NAT,DNS（丢弃，移至TurboACC）</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-freifunk-diagnostics&nbsp;#freifunk组件 诊断（未知）（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-freifunk-policyrouting&nbsp;#freifunk组件 策略路由（未知）（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-freifunk-widgets&nbsp;#freifunk组件 索引（未知）（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-frpc&nbsp;#内网穿透Frp客户端</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-frps&nbsp;#内网穿透Frp服务端</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-fwknopd&nbsp;#Firewall Knock Operator服务器</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-guest-wifi&nbsp;#WiFi访客网络</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-gfwlist&nbsp;#GFW域名列表（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-go-aliyundrive-webdav&nbsp;#阿里云盘webdav协议(文件管理/同步等) （丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-gost&nbsp;#隐蔽的https代理（Le库以外的插件）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-haproxy-tcp&nbsp;#HAProxy负载均衡-TCP</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-hd-idle&nbsp;#硬盘休眠</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-hnet&nbsp;#Homenet Status家庭网络控制协议</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-https-dns-proxy&nbsp;#通过HTTPS代理为DNS提供Web UI</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-ipsec-server&nbsp;#服务器 IPSec</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-ipsec-virtual**d&nbsp;#virtual**服务器 IPSec</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-jd-dailybonus&nbsp;#京东签到服务（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-kodexplorer&nbsp;#KOD可道云私人网盘</span>

<span style="background-color:#FFFFFF;">（与vnStat冲突&nbsp;</span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">!</span></span>

<span style="background-color:#FFFFFF;">&nbsp;）</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-kooldns&nbsp;#virtual**服务器 ddns替代方案（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-koolproxy&nbsp;#KP去广告（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-lxc&nbsp;#LXC容器管理</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-meshwizard #网络设置向导（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-minidlna&nbsp;#完全兼容DLNA / UPnP-AV客户端的服务器软件</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-mjpg-streamer&nbsp;#兼容Linux-UVC的摄像头程序</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-mosdns&nbsp;#MosDNS转发器</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-mtwifi&nbsp;#MTWiFi驱动的支持 （丢弃）</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-mmc-over-gpio&nbsp;#添加SD卡操作界面（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-multiwan&nbsp;#多拨虚拟网卡（丢弃，移至syncdial）</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-mwan&nbsp;#MWAN负载均衡（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-music-remote-center&nbsp;#PCHiFi 数字转盘遥控</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-mwan3&nbsp;#MWAN3负载均衡</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-mwan3helper&nbsp;#MWAN3分流助手</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-n2n_v2&nbsp;#N2N内网穿透 N2N v2 virtual**服务</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-netdata&nbsp;#Netdata实时监控（图形化）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-nfs&nbsp;#NFS网络共享</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-nft-qos&nbsp;#QOS流控 Nftables版</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-ngrokc&nbsp;#Ngrok 内网穿透（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-nlbwmon&nbsp;#网络带宽监视器</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-noddos&nbsp;#NodDOS Clients 阻止DDoS攻击</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-nps&nbsp;#内网穿透nps</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-ntpc&nbsp;#NTP时间同步服务器</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-ocserv&nbsp;#OpenConnect virtual**服务</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-olsr&nbsp;#OLSR配置和状态模块</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-olsr-services&nbsp;#OLSR服务器</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-olsr-viz&nbsp;#OLSR可视化</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-ocserv&nbsp;#OpenConnect virtual**服务（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-omcproxy&nbsp;#嵌入式IGMPv3和MLDv2组播代理</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-openclash&nbsp;#运行在OpenWrt上的Clash代理客户端（Le库以外的插件）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-openvirtual**&nbsp;#Openvirtual**客户端</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-openvirtual**-server&nbsp;#易于使用的Openvirtual**服务器 Web-UI</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-oscam&nbsp;#OSCAM服务器（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-p910nd&nbsp;#打印服务器模块</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-pagekitec&nbsp;#Pagekitec内网穿透客户端</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-“师夷长技以制夷”&nbsp;#“师夷长技以制夷”（Li大佬插件）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> Configuration ---&gt; Include Brook&nbsp;#Brook代理(跨平台强加密且不可检测代理)</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;">Configuration ---&gt; Include china-dns-NG&nbsp;#防污染DNS服务</span>

<br>

<span style="background-color:#FFFFFF;"> Configuration ---&gt; Include Haproxy&nbsp;#HAProxy&nbsp;#HAProxy负载均衡</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> Configuration ---&gt; Include Hysteria&nbsp;#Hysteria双边加速工具</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> Configuration ---&gt; Include Kcptun&nbsp;#Kcptun双边加速工具</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> Configuration ---&gt; Include NaiveProxy&nbsp;#NaiveProxy代理(Chrome网络堆栈伪装流量)</span>

<br>

<span style="background-color:#FFFFFF;"> Configuration ---&gt; Include PDNSD&nbsp;#DNS服务器</span>

<br>

<span style="background-color:#FFFFFF;"> Configuration ---&gt; Include SS Libev Client&nbsp;#SS Libev客户端(轻量级)</span>

<br>

<span style="background-color:#FFFFFF;"> Configuration ---&gt; Include SS Libev Server&nbsp;#SS Libev服务端(轻量级)</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> Configuration ---&gt; Include SS Rust Client&nbsp;#SS Rust客户端(负载均衡/探测延迟)</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;">&nbsp;Configuration ---&gt; Include “师夷长技以制夷” Libev Client&nbsp;#“师夷长技以制夷” Libev客户端(轻量级)</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> Configuration ---&gt; Include “师夷长技以制夷” Libev Server&nbsp;#“师夷长技以制夷” Libev服务端(轻量级)</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;">&nbsp;Configuration ---&gt; Include Simple-Obfs (SS plugin)&nbsp;#simple-Obfs简单混淆工具(Nginx)</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> Configuration ---&gt; Include Trojan_GO&nbsp;#Trojan_GO代理(直接模仿协议HTTPS)</span>

<br>

<span style="background-color:#FFFFFF;"> Configuration ---&gt; Include Trojan_Plus&nbsp;#Trojan_Plus代理(直接模仿协议HTTPS)</span>

<br>

<span style="background-color:#FFFFFF;"> Configuration ---&gt; Include “师夷长技以制夷”&nbsp;#“师夷长技以制夷”代理</span>

<br>

<span style="background-color:#FFFFFF;"> Configuration ---&gt; Include “师夷长技以制夷”-plugin (SS plugin)&nbsp;#SS “师夷长技以制夷”插件(WebSocket+TLS )</span>

<br>

<span style="background-color:#FFFFFF;"> Configuration ---&gt; Include Xray&nbsp;#Xray代理(XTLS)</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> Configuration ---&gt; Include Xray-Plugin (SS Plugin)&nbsp;#SS Xray插件(WebSocket+TLS )</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="background-color:#FFFFFF;"> Configuration ---&gt; Include Dns2socks&nbsp;#DNS服务器（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;"> Configuration ---&gt; Include “师夷长技以制夷”2&nbsp;#“师夷长技以制夷”2代理(透明TCP定向Socks/HTTPS代理服务器)（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;"> Configuration ---&gt; Include SS&nbsp;#SS代理（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;"> Configuration ---&gt; Include SS Server&nbsp;#SS服务器（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;"> Configuration ---&gt; Include SS Rust (AEAD ciphers only)&nbsp;#“师夷长技以制夷”UST代理(AEAD加密)（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;"> Configuration ---&gt; Include “师夷长技以制夷”&nbsp;#“师夷长技以制夷”代理（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;"> Configuration ---&gt; Include ShSR Server&nbsp;#“师夷长技以制夷”服务器（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;">&nbsp;Configuration ---&gt; Include Https DNS Proxy(DoH)&nbsp;#HttpsDNS服务（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-pgyvirtual**&nbsp;#蒲公英virtual**</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-phtunnel&nbsp;#花生壳PHTunnel内网穿透</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-polipo&nbsp;#Polipo代理(是一个小型且快速的网页缓存代理)</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-pppoe-relay&nbsp;#PPPoE NAT穿透 点对点协议（PPP）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-p p t p-server&nbsp;#virtual**服务器 p p t p</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-privoxy&nbsp;#Privoxy网络代理(带过滤无缓存)</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-ps3netsrv&nbsp;#PS3 NET服务器(用于加载蓝光/游戏ISO/PKG)</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-pushbot&nbsp;#全能推送(钉钉推送,企业微信推送,Bark,PushPlus推送)</span>

<span style="background-color:#FFFFFF;"></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-qbittorrent&nbsp;#BT下载工具(qBittorrent)</span>

<br>

<span style="background-color:#FFFFFF;"></span>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">Build Version Selection (Static Build)&nbsp;---&gt; Static Build&nbsp;#选择静态编译版本</span>

<br>

<span style="background-color:#FFFFFF;"></span>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">Build Version Selection (Static Build)&nbsp;---&gt; Dynamic Build&nbsp;#选择动态编译版本</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-qbittorrent-simple&nbsp;#BT下载工具(qBittorrent)简化版</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="background-color:#FFFFFF;"></span>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">Build Version Selection (Static Build)&nbsp;---&gt; Static Build&nbsp;#选择静态编译版本</span>

<br>

<span style="background-color:#FFFFFF;"></span>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">Build Version Selection (Static Build)&nbsp;---&gt; Dynamic Build&nbsp;#选择动态编译版本</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-qos&nbsp;#流量服务质量(QoS)流控</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-radicale&nbsp;#CalDAV/CardDAV同步工具</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-ramfree&nbsp;#释放内存</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-rclone&nbsp;#命令行云端同步工具</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> Include rclone-webui&nbsp;#Rclone界面</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> Include rclone-ng (another webui)&nbsp;#Rclone另一个界面</span>

<br>

<span style="background-color:#FFFFFF;"> Include fuse-utils (mount cloud storage)&nbsp;#fuse-utils（挂载云存储）（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-rp-pppoe-server&nbsp;#Roaring Penguin PPPoE Server 服务器</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-samba&nbsp;#网络共享（Samba）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-samba4&nbsp;#网络共享（Samba4）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-serverchan&nbsp;#微信/请不要发布这类群，谢谢推送的插件</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-sfe&nbsp;#Turbo ACC网络加速（丢弃，移至TurboACC）</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-“师夷长技以制夷”&nbsp;#SS“师夷长技以制夷”（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-“师夷长技以制夷”-libes&nbsp;#SS-libev服务端</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-shairplay&nbsp;#支持AirPlay功能</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-siitwizard&nbsp;#SIIT配置向导&nbsp;SIIT-Wizzard</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-simple-adblock&nbsp;#简单的广告拦截</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-smartdns&nbsp;#SmartDNS本地服务器（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-socat&nbsp;#Socat多功能的网络工具(端口转发)</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-softethervirtual**&nbsp;#SoftEther virtual**服务器&nbsp;NAT穿透</span>

<span style="background-color:#FFFFFF;"></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-splash&nbsp;#Client-Splash是无线MESH网络的一个热点认证系统</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-sqm&nbsp;#流量智能队列管理（QOS）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-squid&nbsp;#Squid代理服务器</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-“师夷长技以制夷”-plus&nbsp;#“师夷长技以制夷”“师夷长技以制夷”Plus+（Le大佬插件）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> SS Client Selection (SS-libev)&nbsp;---&gt; None&nbsp;#不选</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="background-color:#FFFFFF;"> SS Client Selection (SS-libev)&nbsp;---&gt; SS-libev&nbsp;#选择 SS Libev，C语言版(轻量级)</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> SS Client Selection (SS-libev)&nbsp;---&gt; “师夷长技以制夷”ust&nbsp;#选择 SS rust，Rust语言版(负载均衡/探测延迟)</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> SS Server Selection (SS-libev)&nbsp;---&gt; None&nbsp;#不选</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="background-color:#FFFFFF;"> SS Server Selection (SS-libev)&nbsp;---&gt; SS-libev&nbsp;#选择 SS Libev，C语言版(轻量级)&nbsp;</span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> SS Server Selection (SS-libev)&nbsp;---&gt; “师夷长技以制夷”ust&nbsp;#选择 SS rust，Rust语言版(负载均衡/探测延迟)</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> “师夷长技以制夷”-core Selection (Xray-core)&nbsp;---&gt; None&nbsp;#不选</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> “师夷长技以制夷”-core Selection (Xray-core)&nbsp;---&gt; “师夷长技以制夷”-core&nbsp;#“师夷长技以制夷”核心</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="background-color:#FFFFFF;"> “师夷长技以制夷”-core Selection (Xray-core)&nbsp;---&gt; Xray-core&nbsp;#Xray核心&nbsp;</span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> “师夷长技以制夷”-core Selection (Xray-core)&nbsp;---&gt; SagerNet-core&nbsp;#“师夷长技以制夷”核心增强版</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include Kcptun&nbsp;#Kcptun双边加速工具</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include Hysteria&nbsp;#轻量代理-专为恶劣网络环境进行优化的网络工具(双边加速)</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include IPT2Socks&nbsp;#IPT2Socks轻量代理</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include NaiveProxy&nbsp;#NaiveProxy代理(Chrome网络堆栈伪装流量)</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include “师夷长技以制夷”2&nbsp;#“师夷长技以制夷”2代理(透明TCP定向Socks/HTTPS代理服务器)</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include Simple-Obfs Plugin&nbsp;#SS Simple-Obfs混淆代理(Nginx)</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt;&nbsp;</span>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">Include SS “师夷长技以制夷” Plugin&nbsp;#SS “师夷长技以制夷”代理(WebSocket+TLS )</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include “师夷长技以制夷” Libev Client&nbsp;#“师夷长技以制夷” Libev客户端(轻量级)</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include “师夷长技以制夷” Libev Server&nbsp;#“师夷长技以制夷” Libev服务端(轻量级)</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include Trojan&nbsp;#Trojan代理(直接模仿协议HTTPS)</span>

<br>

<span style="background-color:#FFFFFF;"> Include libustream-ssl&nbsp;---&gt; Include libustream-wolfssl&nbsp;#选择wolfSSL库(传输层安全协议)</span>

<br>

<span style="background-color:#FFFFFF;"> Include libustream-ssl&nbsp;---&gt; Include libustream-openssl&nbsp;#选择OpenSSL库(传输层安全协议)</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include SS Libev Client&nbsp;#SS Libev客户端(轻量级)</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include SS Libev Server&nbsp;#SS Libev服务端(轻量级)</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include SS Rust Client&nbsp;#SS Rust客户端(负载均衡/探测延迟)</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include SS Rust Server&nbsp;#SS Rust服务端(负载均衡/探测延迟)</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include Xray&nbsp;#Xray代理(XTLS)</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include SS New Version&nbsp;#新SS代理（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;">&nbsp;luci-app-“师夷长技以制夷”-plus ---&gt; Include SS&nbsp;#SS代理（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include SS Rust (AEAD ciphers only)&nbsp;#“师夷长技以制夷”UST代理(AEAD密码)&nbsp;（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include “师夷长技以制夷”&nbsp;#“师夷长技以制夷”代理（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include Xray (“师夷长技以制夷”/Trojan-GO implemented)&nbsp;#Xray代理（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include Trojan-go&nbsp;#Trojan-go代理（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include SS Server&nbsp;#SS服务器（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include SS Rust Server&nbsp;#SS Rust服务器（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include “师夷长技以制夷” Server&nbsp;#“师夷长技以制夷”服务器（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include DNS2SOCKS&nbsp;#DNS服务器（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include “师夷长技以制夷” Socks and Tunnel（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;"> luci-app-“师夷长技以制夷”-plus ---&gt; Include Socks Server&nbsp;#socks代理服务器（丢弃）</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-“师夷长技以制夷”-pro&nbsp;#“师夷长技以制夷”-Pro（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-“师夷长技以制夷”server-python&nbsp;#“师夷长技以制夷”R Python服务器</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-statistics&nbsp;#流量监控工具</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-syncdial&nbsp;#多拨虚拟网卡（原macvlan）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-tinyproxy&nbsp;#Tinyproxy是 HTTP(S)代理服务器</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-transmission&nbsp;#BT下载工具</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-travelmate&nbsp;#旅行路由器</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-ttyd&nbsp;#网页终端命令行</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-turboacc&nbsp;#Turbo ACC 网络加速(支持 Fast Path 或者 硬件 NAT)</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> luci-app-turboacc ---&gt; Include Flow Offload&nbsp;#Flow Offload加速(提高路由转发效率)</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> luci-app-turboacc ---&gt; Include Shortcut-FE&nbsp;#Shortcut-FE 流量分载</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> luci-app-turboacc ---&gt; Include Shortcut-FE CM&nbsp;#Shortcut-FE 流量分载(高通芯片版)</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> luci-app-turboacc ---&gt; Include BBR CCA&nbsp;#BBR拥塞控制算法提升TCP网络性能</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> luci-app-turboacc ---&gt; Include Pdnsd&nbsp;#DNS防污染 Pdnsd</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="background-color:#FFFFFF;"></span>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">luci-app-turboacc ---&gt; Include DNSForwarder&nbsp;#DNS防污染 Forwarder</span>

<br>

<span style="background-color:#FFFFFF;"></span>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">luci-app-turboacc ---&gt; Include DNSProxy&nbsp;#DNS防污染 Proxy</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-udpxy&nbsp;#udpxy做组播服务器</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-uhttpd&nbsp;#uHTTPd Web服务器</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-unblockmusic&nbsp;#解锁网易云灰色歌曲3合1新版本</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> UnblockNeteaseMusic Golang Version&nbsp;#Golang版本</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> UnblockNeteaseMusic NodeJS Version&nbsp;#NodeJS版本</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-unblockneteasemusic-go&nbsp;#解除网易云音乐（合并）</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-unblockneteasemusic-mini&nbsp;#解除网易云音乐（合并）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-unbound&nbsp;#Unbound DNS解析器</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-upnp&nbsp;#通用即插即用UPnP（端口自动转发）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-usb-printer&nbsp;#USB 打印服务器</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-uugamebooster&nbsp;#UU网游加速器</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-“师夷长技以制夷”-server&nbsp;#“师夷长技以制夷” 服务器</span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-“师夷长技以制夷”-pro&nbsp;#“师夷长技以制夷”透明代理（丢弃，集成“师夷长技以制夷”）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-verysync&nbsp;#微力同步</span>

<span style="background-color:#FFFFFF;"></span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-vlmcsd&nbsp;#KMS服务器设置</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-vnstat&nbsp;#vnStat网络监控（图表）</span>

<span style="background-color:#FFFFFF;">（与kodexplorer冲突&nbsp;</span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">!</span></span>

<span style="background-color:#FFFFFF;">&nbsp;）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-virtual**bypass&nbsp;#virtual** BypassWebUI&nbsp;绕过virtual**设置</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-vsftpd&nbsp;#FTP服务器</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-v“师夷长技以制夷”&nbsp;#V“师夷长技以制夷”“师夷长技以制夷”（je大佬插件）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> luci-app-v“师夷长技以制夷” ---&gt; Include Xray&nbsp;#Xray代理(XTLS)</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> luci-app-v“师夷长技以制夷” ---&gt; Include Trojan&nbsp;#Trojan代理(直接模仿协议HTTPS)</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> luci-app-v“师夷长技以制夷” ---&gt; Include Kcptun&nbsp;#Kcptun双边加速工具</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> luci-app-v“师夷长技以制夷” ---&gt; Include “师夷长技以制夷” Xray Plugin&nbsp;#SS Xray代理</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;"> luci-app-v“师夷长技以制夷” ---&gt; Include “师夷长技以制夷”R Libev Server&nbsp;#“师夷长技以制夷” Libev服务端(轻量级)</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-watchcat&nbsp;#断网检测功能与定时重启</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-webadmin&nbsp;#Web管理页面设置</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-webdav&nbsp;#WebDAV阿里云盘</span>

<span style="background-color:#FFFFFF;"></span>

<span style="background-color:#FFFFFF;"><span style="font-weight:700;">*</span></span>

<br>

<span style="background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-webshell&nbsp;#网页命令行终端（丢弃）</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-wifischedule&nbsp;#WiFi 计划</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-wireguard&nbsp;#virtual**服务器 WireGuard状态</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-wirele“师夷长技以制夷”egdb&nbsp;#WiFi无线</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-wol&nbsp;#WOL网络唤醒</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-wrtbwmon&nbsp;#实时流量监测</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-xlnetacc&nbsp;#迅雷快鸟</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">LuCI ---&gt; Applications ---&gt; luci-app-zerotier&nbsp;#ZeroTier内网穿透</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">----------------------------------------------------------------------------------------</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">转载的时候请注明出处</span>

<br>

<br>

<br>

<br>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">支持 iPv6：</span>

<br>

<span style="background-color:#FFFFFF;">1</span>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">、Extra packages&nbsp;---&gt;&nbsp;ipv6helper&nbsp;（选定这个后下面几项自动选择了）</span>

<br>

<span style="background-color:#FFFFFF;">Network&nbsp;---&gt;&nbsp;odhcp6c<br> Network&nbsp;---&gt;&nbsp;odhcpd-ipv6only<br> LuCI&nbsp;---&gt;&nbsp;Protocols&nbsp;---&gt;&nbsp;luci-proto-ipv6<br> LuCI&nbsp;---&gt;&nbsp;Protocols&nbsp;---&gt;&nbsp;luci-proto-ppp</span>

<br>

<br>

<span style="background-color:#FFFFFF;">2</span>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">、打开适用于VMware的VM Tools</span>

<br>

<span style="background-color:#FFFFFF;">Utilities&nbsp;---&gt;&nbsp;open-vm-tools&nbsp;#打开适用于VMware的VM Tools</span>

<br>

<span style="background-color:#FFFFFF;">Utilities&nbsp;---&gt;&nbsp;open-vm-tools-fuse&nbsp;#打开适用于VMware的VM Tools</span>

<br>

<br>

<span style="background-color:#FFFFFF;">3</span>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">、</span>

<span style="background-color:#FFFFFF;">第二次编译</span>

<span style="background-color:#FFFFFF;">：</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">cd lede # 进入LEDE目录</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">git pull&nbsp;# 同步更新大雕源码</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">./scripts/feeds update -a &amp;&amp; ./scripts/feeds install -a&nbsp;# 更新Feeds</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">rm -rf ./tmp &amp;&amp; rm -rf .config&nbsp;# 清除编译配置和缓存</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">make menuconfig # 进入编译配置菜单</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">make -j</span>

<span style="background-color:#FFFFFF;">n</span>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">&nbsp;V=99&nbsp;# 开始编译&nbsp;</span>

<span style="background-color:#FFFFFF;">n</span>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">=线程数+1，例如4线程的I5填-j5</span>

<br>

<br>

<span style="background-color:#FFFFFF;">4</span>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">、编译丰富插件时，建议修改下面两项默认大小，留足插件空间。</span>

<span style="background-color:#FFFFFF;">（ x86/64 ）！！！</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">Target Images ---&gt; (</span>

<span style="background-color:#FFFFFF;">16</span>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">) Kernel partition size (in MB)&nbsp;#默认是 (</span>

<span style="background-color:#FFFFFF;">16</span>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">) 建议修改 (</span>

<span style="background-color:#FFFFFF;">256</span>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">)</span>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">Target Images ---&gt; (</span>

<span style="background-color:#FFFFFF;">400</span>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">) Root filesystem partition size (in MB)&nbsp;#默认是 (</span>

<span style="background-color:#FFFFFF;">400</span>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">) 建议修改 (</span>

<span style="background-color:#FFFFFF;">512</span>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">)</span>

<br>

<br>

<br>

<span style="color:#444444;font-family:Tahoma, Helvetica, &quot;font-size:14px;background-color:#FFFFFF;">另外有Excel文档方便修改查找：202211&nbsp;</span>

![](<https://www.right.com.cn/forum/static/image/filetype/zip.gif>)[OpenWRT编译LUCI插件说明2022.11.xlsx.zip](<https://www.right.com.cn/forum/forum.php?mod=misc&action=attachpay&aid=327014&tid=344825>)<span class="xg1" style="color:#666666;">(24.25 KB, 下载次数: 6943, 售价: 2 币恩山币)</span>




<a href="#readme">
<img src="https://img.shields.io/badge/-返回顶部-FFFFFF.svg" title="返回顶部" align="right"/>
</a>
