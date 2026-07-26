# ScrapeFun Server for macOS

> 最后更新：2026 年 7 月 26 日

ScrapeFun Server for macOS 将服务端、网页管理界面和桌面宿主整合在一个应用中，适合直接在 Mac 上管理媒体库。

## 下载

从 [Releases](https://github.com/HaoweiLi97/scrapefun-server-macos/releases/latest) 下载最新的 `macos-arm64` DMG。

当前版本支持 Apple Silicon（M1 及更新芯片）。

## 安装

1. 打开下载的 DMG。
2. 将 `ScrapeFun Server.app` 拖入“应用程序”。
3. 从“应用程序”启动 ScrapeFun Server。

如果某个版本需要额外的首次启动步骤，以该版本 Release 页面中的说明为准。

## 状态栏菜单

应用启动后会常驻 macOS 状态栏，可用于：

- 打开 ScrapeFun
- 在浏览器中打开
- 重启服务
- 查看数据目录和日志目录
- 设置登录时启动
- 开启或关闭局域网访问
- 检查 stable 或 beta 更新

## 数据与日志

所有运行数据都保存在：

```text
~/Library/Application Support/ScrapeFunDesktop/
```

数据库和持久化数据位于 `data` 子目录，日志位于 `logs` 子目录。更新应用不会删除该目录。

## 应用内更新

设置页可以检查新版本，并在 stable 与 beta 频道之间切换。选择 beta 后可以收到测试版本；切回 stable 后会继续跟随稳定版本。

## 相关链接

- [ScrapeFun 使用与 Docker 文档](https://github.com/HaoweiLi97/ScrapeFun)
- [Windows Server](https://github.com/HaoweiLi97/scrapefun-server-windows)
- [产品网站](https://scrapefun.com/)
