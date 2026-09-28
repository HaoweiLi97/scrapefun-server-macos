# ScrapeFun Server for macOS

[简体中文](./README.md) · **English**

[Product overview](https://github.com/HaoweiLi97/ScrapeFun/blob/main/README.en.md) · [Stable downloads](https://github.com/HaoweiLi97/scrapefun-server-macos/releases/latest) · [All releases](https://github.com/HaoweiLi97/scrapefun-server-macos/releases) · [Online documentation](https://scrapefun.com/?lang=en#/docs)

> Updated: 2026-09-28. Versions and assets below are the stable releases checked on this date. Follow the corresponding Release for later changes.

A native macOS menu-bar host with the ScrapeFun Server runtime and a browser-based management interface. Manage movie, TV, comic, and remote WebDAV / AList libraries on your Mac, and let Clients on other devices connect.

## Downloads and environment

| Item | Current stable release |
| --- | --- |
| Version | [0.3.3](https://github.com/HaoweiLi97/scrapefun-server-macos/releases/tag/v0.3.3) |
| System | macOS 13 or later |
| Architecture | Apple Silicon / arm64, M1 or later |
| Package | `scrapefun-server-macos-arm64-0.3.3-stable.dmg` |
| Trust status | Ad-hoc integrity signature; not Apple Developer ID signed or notarized |

Download the DMG from the [stable download page](https://github.com/HaoweiLi97/scrapefun-server-macos/releases/latest). An Intel version is not currently provided.

## Installation and first launch

1. Open the official DMG and drag `ScrapeFun Server.app` into Applications.
2. For 0.3.3, run the command required by that release before first launch:

   ```bash
   xattr -dr com.apple.quarantine "/Applications/ScrapeFun Server.app"
   ```

3. Launch from Applications and configure the local port; the default is `8096`.
4. Follow the browser setup page to configure administrator credentials and libraries.

The command removes the download quarantine flag. It does not add an Apple signature or notarization. Follow each later release's first-launch requirements.

## Menu bar and network access

The menu bar provides actions to open the web interface, restart the service, view data and log directories, start at login, and check for updates. Before serving other devices, finish initialization, then enable LAN access as needed and check the firewall.

The default local address is `http://127.0.0.1:8096`. Other devices use this Mac's LAN IP address. Use the actual port if you changed it.

## Data and backups

Runtime directory:

```text
~/Library/Application Support/ScrapeFunDesktop/
```

Business data is in the `data` subdirectory and logs are in `logs`. Installing over the existing application normally retains these files. Deleting the runtime directory deletes instance data. Before upgrading, export a backup from the web settings and store it on another device.

## Updates

Check for updates through the menu bar or web settings, or install a newer DMG over the current version. In-app updates use Sparkle and support stable / beta channels. Updating restarts Server and interrupts playback and background tasks. Also back up before switching channels; older versions are not guaranteed to read newer data.

## Troubleshooting

If launch fails, check the system version, architecture, application location, and release-specific first-launch requirements. For service problems, open the log directory from the menu bar. Include Server version, port configuration, and logs with sensitive details removed in reports.

## Support and licensing

This repository provides platform installation instructions and official release assets. Submit usage questions and feature requests to the [main repository Issues](https://github.com/HaoweiLi97/ScrapeFun/issues). For accounts, activation, or private logs, contact `scrapefun@outlook.com`. Report security issues privately according to the [security instructions](./SECURITY.en.md).

See the new [commercial license statement](./LICENSE.en.txt) and full [software license agreement](./EULA.en.md). Ordinary personal, household, and internal organizational use is allowed. Pro requires a valid entitlement. Software redistribution, resale, customer delivery, and paid hosting require separate written authorization. The statement does not retroactively change existing licenses; existing assets follow their supplied licenses, and third-party components retain their own licenses.

[Releases and compatibility](https://github.com/HaoweiLi97/ScrapeFun/blob/main/RELEASE_POLICY.en.md) · [Third-party components](https://github.com/HaoweiLi97/ScrapeFun/blob/main/THIRD_PARTY_NOTICES.en.md) · [Support](./SUPPORT.en.md)
