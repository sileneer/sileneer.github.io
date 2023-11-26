---
layout: post
title:  "How to bypass the firewall in some regions (via airports)"
date:   2023-11-11 23:30:00 +0800
categories: Network
---


**Table of content:**
- [Before continuing...](#before-continuing)
- [原理](#原理)
  - [一些名词](#一些名词)
  - [如何使用](#如何使用)
- [机场推荐](#机场推荐)
  - [省流](#省流)
    - [SKY VPN](#sky-vpn)
    - [OuO Network](#ouo-network)
  - [机场比较](#机场比较)
- [安装与配置](#安装与配置)
  - [\[Recommended\] Clash Verge (For Linux, macOS and Windows)](#recommended-clash-verge-for-linux-macos-and-windows)
  - [Windows: Clash for Windows](#windows-clash-for-windows)
  - [macOS: ClashX](#macos-clashx)
  - [Android / HarmonyOS](#android--harmonyos)
  - [iOS](#ios)
  - [Router](#router)
- [Troubleshot](#troubleshot)
  - [Windows](#windows)
  - [macOS](#macos)

## Before continuing... 

Please follow the laws and regulations of the country and region you are in now. DO NOT use the contents and resources for illegal or immoral purposes. 

<ins>If you are to conduct interviews or important activities, it is highly recommended to use your own roaming data or eSIM plans (on iPhone or Android phone with eSIM supported).</ins>

## 原理

### 一些名词

> 机场：机场指的是一些提供代理服务的网站，用户可以通过购买套餐来使用代理服务。

> Clash, v2ray: 跨平台的基于规则的代理工具

> Clash for Windows / Clash Verge: Clash for Windows 是基于 Clash 的一个 GUI 客户端，可以通过图形界面来配置代理规则

### 如何使用

Clash 客户端是用来配置代理规则的，它可以通过订阅链接来获取代理规则。机场一般是个人在境外组建的服务器，他们提供订阅链接，然后我们用 Clash 的时候，就可以通过他们的服务器代理访问境外的网站。

1. 选择一个机场，购买一个套餐，获取订阅链接
2. 下载并安装 Clash 的客户端
3. 配置 Clash 的客户端，将订阅链接添加到 Clash 的客户端中
4. 启动 Clash 的客户端，选择一个节点
5. 配置系统代理

## 机场推荐

### 省流

#### SKY VPN

我正在使用的是 [SKY VPN](https://skyvpn.one)，这个机场的套餐主要有以下几个，速度和稳定度都还行，算是我能找到便宜有好用的机场了。

> From SKY VPN: 域名被墙给污染了，国内可以使用 yun.skyvpn.one 进行访问，订阅链接可以重新复制或者将sub2.skyvpn.one替换成sub3.skyvpn.one

⚠️ 网速换算：1Mbps = 0.125MB/s, 1MB/s = 8Mbps

⚠️ 流量是按照流入流出总和计算的，所以如果你的流量是 30G，那么你的流入流出总和是 30G，而不是 60G。

| 流量 | 时长 | 价格 | 速度 | 同时在线设备 | 推荐 |
| --- | --- | --- | --- | --- | --- |
| 30G | 30天 | ￥0.5/月 | 30Mbps | 2 | ✅ |
| 200G | 30天 | ￥4/月 | 100Mbps | 2 |
| 200G | 30天 | ￥6/月 | unlimited | 2 | ✅ |
| 1000G | 30天 | ￥8/月 | unlimited | 6 |

#### OuO Network

[OuO Network](https://ouonetwork.b-cdn.net)

（我没怎么用过这个机场，但是听说挺快挺稳的。下面这个code可以享受6块钱一个月100G的优惠，还是挺划算的，可以试一试）

Referal code: DUANG114514

### 机场比较

关于其他的机场，这个网站上有详细的机场比较：[付费机场推荐/SSR-v2ray专线机场评测（2023.11.7更新）](https://sites.google.com/view/honven/%E9%A6%96%E9%A1%B5/%E6%9C%BA%E5%9C%BA%E6%8E%A8%E8%8D%90)，但是我的建议是，这种机场长期来看都不是太稳定，不要给机场充太多钱，一般来说，一个月的套餐就够了。

## 安装与配置

### [Recommended] Clash Verge (For Linux, macOS and Windows)

**Please go to [Troubleshot](#troubleshot) if you encounter any problems.**

Download from [release](https://github.com/wonfen/clash-verge-rev/releases). Supports Windows x64, Linux x86_64 and macOS 11+

- [Windows x64](https://github.com/wonfen/clash-verge-rev/releases/download/v1.4.0/Clash.Verge_1.4.0_x64_zh-CN.msi)
- [macOS intel](https://github.com/wonfen/clash-verge-rev/releases/download/v1.4.0/Clash.Verge_1.4.0_x64.dmg)
- [macOS arm](https://github.com/wonfen/clash-verge-rev/releases/download/v1.4.0/Clash.Verge_1.4.0_aarch64.dmg)
- [Linux AppImage](https://github.com/wonfen/clash-verge-rev/releases/download/v1.4.0/clash-verge_1.4.0_amd64.AppImage)
- [Linux deb](https://github.com/wonfen/clash-verge-rev/releases/download/v1.4.0/clash-verge_1.4.0_amd64.deb)

安装配置教程：

<iframe width="560" height="315" src="https://www.youtube.com/embed/C_q8Cv0A_cc?si=amLxFRkkwWEVD2Pl" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

### Windows: Clash for Windows

**Please go to [Troubleshot](#troubleshot) if you encounter any problems.**

1. 下载 Clash for Windows：
   1. x64: [https://archive.org/download/clash_for_windows_pkg/Clash.for.Windows.Setup.0.20.39.arm64.exe](https://archive.org/download/clash_for_windows_pkg/Clash.for.Windows.Setup.0.20.39.arm64.exe)
   2. x86: [https://archive.org/download/clash_for_windows_pkg/Clash.for.Windows.Setup.0.20.39.ia32.exe](https://archive.org/download/clash_for_windows_pkg/Clash.for.Windows.Setup.0.20.39.ia32.exe)
   3. Other versions: [https://archive.org/download/clash_for_windows_pkg](https://archive.org/download/clash_for_windows_pkg)


2. 安装 Clash for Windows


3. 在机场购买套餐，获取订阅链接


   ![Alt text](/assets/image-1.png)


4. 添加订阅：
   1. 如果是使用订阅链接：粘贴订阅链接——然后点击download——提示 Success 


   ![Alt text](/assets/image.png)


    2. 或者点击机场添加链接的地方，一键导入订阅链接


5. 设置系统代理
   点击左边 General —— 点击 System proxy （可以设置开机自启：点击 Start with Windows）


   ![Alt text](/assets/image-2.png)


6. 点击Proxies，再点Proxy


   ![Alt text](/assets/image-3.png)


7. 点击⚡检测延迟


   ![Alt text](/assets/image-4.png)


8. 选择一个延迟低的节点，点击确定


   ![Alt text](/assets/image-5.png)


注意事项：
1. 所示按钮为更新托管地址


   ![Alt text](/assets/image-6.png)


2. 如果是使用订阅链接的可以设置自动定时更新订阅（可选）：点击 Profiles -- 点击 change information 按钮 - 随便输入名称 - 输入定时更新的时间（小时整数，24就挺好）


   ![Alt text](/assets/image-8.png)
   ![Alt text](/assets/image-7.png)

### macOS: ClashX

下载地址：

Download from [gh-pages -> assets/Clash.img](https://github.com/sileneer/sileneer.github.io/blob/gh-pages/assets/ClashX.dmg)

安装配置教程：

<iframe width="560" height="315" src="https://www.youtube.com/embed/zTLOdZh6g08?si=d0vGDi5swwUJ-d3u" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

### Android / HarmonyOS

Download the apk from [release](

### iOS

1. 下载 Shadowrocket. 注意，要切换到非国区的 Apple ID 才能下载 Shadowrocket. 美区价格是2.99美元。

2. 点击软件主界面左上角 ➕ 按钮，在弹出窗口进入添加节点界面，类型选择 `Shadowsocks` 后，出现 `Shadowsocks` 配置界面。
   
   ![Alt text](/assets/image-12.png)

如果你不想付费购买，可以使用共享账号。

**<span style="color:red;">注意，登录时选择-其他选项，不要开启双重验证</span>**

**<span style="color:red;">千万别拿别人的苹果账号登录iCloud，只登录应用商店Apple Store这个软件，进去apple store,点击右上角-拉到最后-退出登录</span>**

**<span style="color:red;font-size:30px;">禁止设置中登录<br>禁止登录iCloud<br>未按要求操作所产生的一切后果自负</span>**

1. 打开设备上的 App Store，点击右上角的头像按钮，然后在弹出的界面中滑动到最底部，点击 "登出" 以退出当前帐号。

2. 选择下方的账号登录 App Store。在弹出的 Apple ID 安全界面中点击 "其他选项 -> 不升级"，切勿开启双重认证！

3. 登录后在 App Store 搜索关键词「Shadowrocket」并下载。下载完成后立即「退出账号」，以避免各类问题。

4. 共享账号地址：https://appleid.zijieyunti.com/share/pDzoeuTjqK

![Alt text](/assets/image-10.png)
![Alt text](/assets/image-11.png)

### Router

[OpenClash](https://github.com/vernesong/OpenClash)

参考：
1. [小米 AX1800 安装 ShellClash](https://zhuanlan.zhihu.com/p/458905777)
2. [Github: juewuy/ShellCrash](https://github.com/juewuy/ShellCrash/releases)

## Troubleshot

### Windows

1. 如果重启电脑后发现连不上网，记得去设置里看一下是不是上次代理忘记关了，重置一下代理设置。

2. If you could not start the app on Windows when you are installing Clash Verge, please check that you have [Webview2](https://developer.microsoft.com/en-us/microsoft-edge/webview2/#download-section) installed.

### macOS

If you encounter the following on macOS:

![Alt text](/assets/image-9.png)

Please run the following command in the terminal:

```bash
xattr -d com.apple.quarantine /Applications/Clash\ Verge.app
```

Replace the `/Applications/Clash\ Verge.app` with the path of your Clash Verge app, if necessary

`sudo` if required.