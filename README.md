# ScrapeFun Server for macOS

**简体中文** · [English](./README.en.md)

[产品主页](https://github.com/HaoweiLi97/ScrapeFun) · [稳定版下载](https://github.com/HaoweiLi97/scrapefun-server-macos/releases/latest) · [全部发行](https://github.com/HaoweiLi97/scrapefun-server-macos/releases) · [在线文档](https://scrapefun.com/#/docs)

> 文档更新：2026-09-28。下列版本和资产为核对当日的稳定版；后续以对应 Release 为准。

macOS 原生菜单栏宿主，内置 ScrapeFun Server 运行时，并通过浏览器提供管理界面。可在 Mac 上管理影视、漫画与 WebDAV / AList 远程媒体库，也可供其他设备的 Client 连接。

## 下载与系统环境

| 项目 | 当前稳定版 |
| --- | --- |
| 版本 | [0.3.3](https://github.com/HaoweiLi97/scrapefun-server-macos/releases/tag/v0.3.3) |
| 系统 | macOS 13 或更新版本 |
| 架构 | Apple Silicon / arm64，M1 及更新芯片 |
| 安装包 | `scrapefun-server-macos-arm64-0.3.3-stable.dmg` |
| 信任状态 | ad-hoc 完整性签名，未经 Apple Developer ID 签名或公证 |

从[稳定版下载页](https://github.com/HaoweiLi97/scrapefun-server-macos/releases/latest)获取 DMG。当前不提供 Intel 版本。

## 安装与首次启动

1. 打开官方 DMG，将 `ScrapeFun Server.app` 拖入“应用程序”。
2. 对 0.3.3，在首次启动前运行该版本要求的命令：

   ```bash
   xattr -dr com.apple.quarantine "/Applications/ScrapeFun Server.app"
   ```

3. 从“应用程序”启动，配置本地端口，默认 `8096`。
4. 在浏览器初始化页面按提示设置管理员凭据并配置媒体库。

上述命令移除下载隔离标记，不会给应用增加 Apple 签名或公证。后续版本的首次启动要求以其 Release 为准。

## 菜单栏与网络访问

菜单栏提供打开网页、重启服务、查看数据与日志目录、登录时启动和更新检查等入口。向其他设备提供服务时，先完成初始化，再按需要启用局域网访问并检查防火墙。

本机默认访问 `http://127.0.0.1:8096`。其他设备使用这台 Mac 的局域网 IP；端口已修改时使用实际端口。

## 数据与备份

运行目录：

```text
~/Library/Application Support/ScrapeFunDesktop/
```

业务数据在 `data` 子目录，日志在 `logs` 子目录。覆盖安装应用通常保留这些数据；主动删除运行目录会删除实例数据。升级前在网页设置中导出备份，并把备份保存在另一设备。

## 更新

通过菜单栏或网页设置检查更新，或下载新版 DMG 覆盖安装。应用内更新采用 Sparkle，支持 stable / beta 频道。更新会重启 Server，中断播放与后台任务；切换频道前也应备份，旧版本不保证能读取较新版本的数据。

## 故障排查

启动失败时检查系统版本、架构、应用位置及 Release 的首次启动要求。服务异常时通过菜单栏查看日志目录，反馈时提供 Server 版本、端口配置和脱敏日志。

## 支持与授权

本仓库提供平台安装说明和官方发行资产。使用问题与功能建议请提交到[主仓库 Issues](https://github.com/HaoweiLi97/ScrapeFun/issues)；账号、激活或私密日志请联系 `scrapefun@outlook.com`。报告安全问题请按[安全说明](./SECURITY.md)私密提交。

新的商业许可声明见 [LICENSE](./LICENSE)，完整条款见[软件使用许可协议](./EULA.md)。个人、家庭及组织内部可正常使用；Pro 需有效授权，软件再分发、转售、客户交付和收费托管须单独书面授权。该声明不追溯改变既有授权；现有资产以其随包许可为准，第三方组件继续适用各自许可证。

[发行与兼容性说明](https://github.com/HaoweiLi97/ScrapeFun/blob/main/RELEASE_POLICY.md) · [第三方组件说明](https://github.com/HaoweiLi97/ScrapeFun/blob/main/THIRD_PARTY_NOTICES.md) · [支持流程](./SUPPORT.md)
