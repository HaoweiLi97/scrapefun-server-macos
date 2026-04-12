<div align="center">
  <img src="./docs/images/favicon.png" alt="ScrapeFun Logo" width="96" />
  <h1>ScrapeFun Desktop for macOS</h1>
  <p>为 macOS Desktop 使用场景设计的原生桌面版本</p>
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

ScrapeFun Desktop for macOS 是围绕 macOS 桌面使用场景整理出来的原生版本，重点不是“把网页包成 App”，而是把桌面常驻、窗口行为、本机托管、菜单栏入口和原生播放器协作这些体验真正做成桌面应用。

如果你更习惯在 Mac 上长期挂着一个媒体入口，而不是频繁打开浏览器标签页，这个版本会更适合你的使用方式。

## About

这个仓库用于发布 macOS 桌面版本的打包产物与使用说明。  
GitHub Releases 会提供可直接下载的 `.dmg` 安装包。

## 相关链接

- [ScrapeFun 主仓库](https://github.com/HaoweiLi97/ScrapeFun)
- [macOS 最新版本](https://github.com/HaoweiLi97/scrapefun-desktop-macos/releases/latest)
- [Docker 镜像](https://hub.docker.com/r/haoweil/scrapefun)

## 它适合谁

- 希望在 macOS 上直接使用 ScrapeFun，而不想每次都手动打开浏览器的人
- 希望把媒体库作为桌面常驻应用长期使用的个人用户
- 想在本机托管 ScrapeFun 服务并获得一体化体验的用户
- 需要菜单栏入口、开机启动、原生窗口行为的 macOS 用户
- 想在桌面端获得更顺手播放链路和更稳定日常体验的用户

## 核心能力

### 1. 菜单栏常驻与桌面入口

- 提供菜单栏常驻入口，适合日常长期挂在桌面环境中
- 不需要依赖浏览器书签或固定标签页
- 更符合 macOS 用户对常驻桌面工具的使用习惯
- 支持 Launch at Login，适合做个人设备上的长期入口

### 2. 本机托管与后台服务管理

- 桌面应用会在本机托管 ScrapeFun 服务
- 更适合一台 Mac 上把管理、浏览和使用链路集中起来
- 提供服务重启、数据目录查看、日志目录查看等桌面侧操作入口
- 更适合希望减少手工命令操作的桌面使用场景

### 3. 独立窗口与原生 WebView 体验

- 通过独立窗口承载应用，而不是单纯浏览器访问
- 使用原生 `WKWebView` 集成桌面端体验
- 更适合窗口切换、恢复、重开和长期停留
- 对桌面环境中的交互行为更友好

### 4. 面向 macOS 的本地目录与运行状态

- 数据、运行时和日志会落在 macOS 本地应用目录中
- 更符合桌面应用对本机状态管理的预期
- 更适合本机单用户长期使用和维护

### 5. 原生播放器协作能力

- 为桌面端播放链路预留了更自然的原生协作方式
- 更适合在 macOS 上做视频播放、字幕加载与播放列表更新
- 相比纯浏览器使用方式，更适合做面向桌面端的播放体验整合

### 6. 发布形态清晰

- 通过 GitHub Releases 分发 `.dmg`
- 安装路径和使用链路更适合普通 macOS 用户
- 适合做公开分发、版本管理和桌面端持续迭代

## 特性介绍

后续这里会结合截图重点介绍这些真正偏 macOS Desktop 的功能：

- 菜单栏入口与常驻方式
- 开机启动与桌面常驻体验
- 本机服务托管与日志/数据目录
- 独立窗口中的媒体库浏览
- 原生播放器协作链路
- 桌面端设置与日常使用路径

## 快速开始

### 方式一：直接下载 Release

1. 打开 [Latest Release](https://github.com/HaoweiLi97/scrapefun-desktop-macos/releases/latest)
2. 下载对应的 `.dmg`
3. 安装后启动应用

### 方式二：先准备主服务

如果你还没有可连接的 ScrapeFun 服务，可以先参考主仓库：

- [ScrapeFun 主仓库](https://github.com/HaoweiLi97/ScrapeFun)
- [Docker 镜像](https://hub.docker.com/r/haoweil/scrapefun)

## 使用建议

- 如果你主要在 Mac 上日常使用 ScrapeFun，这个版本会比纯浏览器方式更顺手
- 如果你希望媒体库以桌面常驻工具的方式存在，这个版本更合适
- 如果你重视菜单栏入口、本机服务管理和独立窗口体验，这个版本就是面向这类场景设计的

## 联系方式

- Product / Business: `lihaowei977@gmail.com`
