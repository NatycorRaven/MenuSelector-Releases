# MenuSelector 安装包

此公开仓库仅分发 Android APK、校验和、安装说明及更新索引，不包含应用源代码、用户数据或签名密钥。

## 0.3.0 开发预览版

新增菜单购物清单：按日期及餐次汇总已确认菜单的食材，保留各菜用量与来源，支持采购勾选、重启保留及备份恢复。

- [版本说明与附件](https://github.com/NatycorRaven/MenuSelector-Releases/releases/tag/v0.3.0-dev)
- [直接下载 APK](https://github.com/NatycorRaven/MenuSelector-Releases/releases/download/v0.3.0-dev/MenuSelector-0.3.0-dev.apk)
- [SHA-256 校验文件](https://github.com/NatycorRaven/MenuSelector-Releases/releases/download/v0.3.0-dev/sha256.txt)
- [所有历史版本](https://github.com/NatycorRaven/MenuSelector-Releases/releases)

最低 Android 8.0 / API 26。当前为开发预览，Android 36 ARM64 模拟器已验证；真实手机和最低系统仍需对应设备验收。手机需允许浏览器/文件管理器安装未知来源应用；系统会要求用户确认。

## 0.2.0 用户先备份，再重新安装

**0.3.0 使用新的 V2 签名，不能直接覆盖安装 0.2.0。不要在备份前卸载旧版。**

1. 在旧版“设置 → 数据备份 → 导出备份”导出 JSON，存放在应用目录外，确认文件存在且可读，建议另存副本。
2. 备份不含 API Key 和模型配置。先确认自己可以重新取得模型配置和密钥；0.2.0 的聊天记录仅在内存中，也不包含在备份内。
3. 卸载旧版，再从上述链接下载并安装 0.3.0。
4. 在新版设置导入 JSON，核对菜谱和历史，再重新配置模型及主题。旧备份没有采购勾选，新清单首次为未购。

首次新安装可直接下载。后续保持 V2 签名的版本支持“设置 → 应用更新”；普通应用不能静默安装。手机需要能访问 GitHub。

## 更新渠道和校验

0.3.0 及后续 V2 使用 [latest-v2.json](https://raw.githubusercontent.com/NatycorRaven/MenuSelector-Releases/main/latest-v2.json)。旧版 [latest.json](https://raw.githubusercontent.com/NatycorRaven/MenuSelector-Releases/main/latest.json) 保留 0.2.0，不向旧版推送无法覆盖的新签名包。JSON 是 App 的版本索引，不是安装包。

0.3.0 APK SHA-256：`e0ecae09d3b7e8bf98c7b51195a1a7090e51ddecef45bcbe70453ea34e64efaf`。

请从此仓库的 Release 附件下载，先核对安装说明及校验值。开发预发布不保证出现在 GitHub `/releases/latest`，建议收藏全部版本页。
