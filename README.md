# Software Releases

个人软件的统一下载与版本发布中心。每个产品独立编号，通过 GitHub Releases 分发安装包。

## 产品下载

| 产品 | 版本 | 平台 | 下载 | 官网 |
| --- | --- | --- | --- | --- |
| SnapNeo | 1.1.0 | macOS 14+ · Apple Silicon (arm64) | [下载安装包](https://github.com/zero-ljz/software-releases/releases/download/snapneo%2Fv1.1.0/SnapNeo-1.1.0-macos-arm64.dmg) · [发布说明](https://github.com/zero-ljz/software-releases/releases/tag/snapneo%2Fv1.1.0) | [snapneo.app](https://snapneo.app/) |

[查看所有版本](https://github.com/zero-ljz/software-releases/releases)

## 版本组织

- 每个产品使用独立的标签前缀：`<product>/v<version>`，例如 `snapneo/v1.1.0`。
- Release 标题采用“产品名 + 版本号”，例如 `SnapNeo 1.1.0`。
- 同一产品、同一版本的不同平台安装包放在同一个 Release 中。
- 新产品发布后，在上方下载表中增加对应入口；发布新版本时更新版本与下载链接。
- 安装包作为 Release 附件上传，不提交到 Git 历史。
- 自动更新应使用各产品自己的更新源，或按产品标签前缀筛选版本；仓库级 `/releases/latest` 不代表每个产品的最新版本。

## 校验下载

Release 提供 `SHA256SUMS.txt`，可与下载文件的 SHA-256 对照。

在 macOS 上运行：

```sh
shasum -a 256 SnapNeo-1.1.0-macos-arm64.dmg
```

## 产品授权

本仓库用于分发软件安装包与发布说明。各产品的使用与授权以其随附的许可条款为准。
