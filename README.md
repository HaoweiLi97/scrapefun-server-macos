<div align="center">
  <img src="./docs/images/favicon.png" alt="ScrapeFun Logo" width="96" />
  <h1>ScrapeFun Desktop for macOS</h1>
  <p>为 macOS Desktop 场景设计的原生桌面版本</p>
  <p>
    <a href="https://github.com/HaoweiLi97/scrapefun-desktop-macos/releases/latest">
      <img src="https://img.shields.io/github/v/release/HaoweiLi97/scrapefun-desktop-macos?label=macOS&logo=apple" alt="macOS Latest Release" />
    </a>
    <a href="https://github.com/HaoweiLi97/ScrapeFun">
      <img src="https://img.shields.io/badge/Main-Repository-111827" alt="Main Repository" />
    </a>
    <a href="https://hub.docker.com/r/haoweil/scrapefun/tags">
      <img src="https://img.shields.io/badge/Docker-latest-2496ED?logo=docker&logoColor=white" alt="Docker latest" />
    </a>
  </p>
</div>

ScrapeFun Desktop for macOS 不是单纯的网页壳，而是围绕 macOS 使用方式做的原生桌面宿主。

重点在这些桌面能力：

- 原生 Swift + AppKit / WebKit 框架
- 右上角状态栏图标与菜单
- Client Settings 中的服务器地址切换
- mpv 原生播放器接入

## 框架

桌面端采用原生 Swift 宿主，核心是：

- AppKit
- WebKit / `WKWebView`
- 原生 macOS 菜单与窗口行为
- 本机托管 ScrapeFun 服务

这也是它和纯浏览器访问最大的区别。

## 状态栏图标与菜单

应用会在 macOS 右上角状态栏提供常驻图标，并挂出常用菜单操作。

当前菜单能力包括：

- Open ScrapeFun
- Open in Browser
- Restart Service
- Show Data Directory
- Show Logs Directory
- Launch at Login
- Allow LAN Access
- Quit

这部分是桌面版本最重要的使用入口之一。

## Client Settings

客户端版本提供独立的 Settings 窗口，用来配置要连接的 ScrapeFun 服务器地址。

这里的重点不是部署，而是连接哪个服务实例。

适合这些场景：

- 在本机服务和远程服务之间切换
- 手动指定服务器地址
- 在桌面端长期固定使用某个实例

## mpv 接入

桌面端支持原生 `mpv` 播放器接入，而不是只停留在浏览器播放层。

当前这部分能力包括：

- 调起本地 `mpv`
- 字幕加载
- 播放列表更新
- 更适合桌面端的视频播放链路

## 特性介绍

后续这里可以结合截图重点展示：

- 状态栏图标与菜单
- Client Settings 中的服务器选择
- 桌面窗口界面
- mpv 播放链路

## 获取方式

直接从 [Latest Release](https://github.com/HaoweiLi97/scrapefun-desktop-macos/releases/latest) 下载 `.dmg` 即可。

## 相关链接

- [ScrapeFun 主仓库](https://github.com/HaoweiLi97/ScrapeFun)
- [macOS 最新版本](https://github.com/HaoweiLi97/scrapefun-desktop-macos/releases/latest)
- [Docker 镜像](https://hub.docker.com/r/haoweil/scrapefun)

## 联系方式

- Product / Business: `lihaowei977@gmail.com`
