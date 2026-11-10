# Software Releases

软件下载与版本发布。

## 产品下载

| 产品 | 版本 | 平台 | 下载 | 官网 |
| --- | --- | --- | --- | --- |
| SnapNeo | 1.1.0 | Windows x64 / macOS 14+ arm64 | [Windows 便携版](https://github.com/zero-ljz/software-releases/releases/download/snapneo%2Fv1.1.0/SnapNeo-1.1.0-windows-x64-portable.7z) · [macOS](https://github.com/zero-ljz/software-releases/releases/download/snapneo%2Fv1.1.0/SnapNeo-1.1.0-macos-arm64.dmg) · [发布说明](https://github.com/zero-ljz/software-releases/releases/tag/snapneo%2Fv1.1.0) | [snapneo.app](https://snapneo.app/) |

[查看所有版本](https://github.com/zero-ljz/software-releases/releases)

## 校验下载

将软件包与同名的 `.sha256` 文件下载到同一目录。

Windows（PowerShell，输出 `True` 表示匹配）：

```powershell
$package = 'SnapNeo-1.1.0-windows-x64-portable.7z'
(Get-FileHash $package -Algorithm SHA256).Hash -eq (Get-Content "$package.sha256").Split()[0]
```

macOS：

```sh
shasum -a 256 -c SnapNeo-1.1.0-macos-arm64.dmg.sha256
```

## 产品授权

各产品的使用与授权以其随附的许可条款为准。

[发布维护](PUBLISHING.md)
