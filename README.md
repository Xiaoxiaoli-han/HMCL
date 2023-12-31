# 🎮 Play Minecraft! Launcher 🎉

[![Build Status](https://github.com/xqzi/HMCL/actions/workflows/gradle.yml/badge.svg)](https://github.com/xqzi/HMCL/actions/workflows/gradle.yml)
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fxqzi%2FPMCL.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fxqzi%2FPMCL?ref=badge_shield)

## 简介

Play Minecraft Launcher (PMCL)是一款基于HMCL衍生的跨平台 Minecraft 启动器, 支持 Mod 管理, 游戏自定义, 游戏自动安装 (Forge, Fabric, Quilt, LiteLoader 与 OptiFine), 模组包创建, 界面自定义等功能.

PMCL 有着强大的跨平台能力. 它不仅支持 Windows、Linux、macOS 等常见的操作系统，同时也支持 x86、ARM、MIPS 和 LoongArch 等不同的 CPU 架构. 您可以使用 PMCL 在不同平台上轻松的游玩 Minecraft.

如果您想要了解 PMCL 对不同平台的支持程度，请参见[此表格](PLATFORM_cn.md).

> *PMCL 根据 HMCL - PR - huanghongxun/HMCL[#2617](https://github.com/huanghongxun/HMCL/pull/2617) 的官方指示依照HMCL开源协议独立自建.

## 下载

请从 [PMCL 官网](https://pmcl.fun/download) 下载最新版本的 PMCL.

你也可以在 [GitHub Releases](https://github.com/xqzi/PMCL/releases) 中下载最新版本的 PMCL.

虽然并不强制, 但仍建议通过 PMCL 官网下载启动器.

## 开源协议

该程序遵循 [HMCL 的开源协议](https://github.com/huanghongxun/HMCL/blob/javafx/LICENSE)的情况下发布, 同时附有额外的条款.

### 附加条款

在未得到仓库所有者([@xqzi](https://github.com/xqzi))的明确许可的情形下, 不得将本项目的“聚合”及“赦免”部分的源代码或非最终成品的二进制文件用于任何非授权用途。

## 发展决策

1.本项目采取委员会管理模式 (Committee Management Model), 由 [@xqzi](https://github.com/xqzi) 担任委员会常驻荣誉会长，拥有关键决策权，在涉及发展项目发展关键性决策或当票数持平时进行作用，其余时候按总票占比10%进行计算.

2.会长由上一年度仓库代码贡献排名前10名产生，贡献排名前3名作为会长，每人拥有总票占比10%的决策权，其余作为副会长，每人拥有总票占比3%的决策权.总票占比为48%。
> 2.1.该排名不包含[@xqzi](https://github.com/xqzi)。

> 2.2.每年统计截止为12月31日（含当日）。

> 2.3.根据统计结果确认下一年度的会长名额。

3.所有用户均为本委员会委员，在委员会发布提案时均可参与投票。总票占比为42%。

4.每个提案的公示期为7天，提案通过后，提案者有3天的时间进行修正和附加说明，提案者未在规定时间内修改的提案将被视为最终通过。

5.委员会决策结果以最终投票结果为参考，根据实际情况进行最终决策。

## 贡献

如果您想提交一个 Pull Request, 必须遵守如下要求:

* IDE: Intellij IDEA
* 编译器: Java 1.8
* **不要**修改 `gradle` 相关文件

### 编译

于项目根目录执行以下命令:

```bash
./gradlew clean build
```

请确保您至少安装了含有 JavaFX 8 的 Java. 建议使用 Liberica Full JDK 8 或更高版本.

## JVM 选项 (用于调试)

| 参数                                           | 简介                                                                                              |
|----------------------------------------------|-------------------------------------------------------------------------------------------------|
| `-Dhmcl.home=<path>`                         | 覆盖 HMCL 数据文件夹.                                                                                  |
| `-Dhmcl.self_integrity_check.disable=true`   | 检查更新时绕过本体完整性检查.                                                                                 |
| `-Dhmcl.bmclapi.override=<version>`          | 覆盖 BMCLAPI 的 API Root, 默认值为 `https://bmclapi2.bangbang93.com`. 例如 `https://download.mcbbs.net`. |
| `-Dhmcl.font.override=<font family>`         | 覆盖字族.                                                                                           |
| `-Dhmcl.version.override=<version>`          | 覆盖版本号.                                                                                          |
| `-Dhmcl.update_source.override=<url>`        | 覆盖更新源.                                                                                          |
| `-Dhmcl.authlibinjector.location=<path>`     | 使用指定的 authlib-injector (而非下载一个).                                                                |
| `-Dhmcl.openjfx.repo=<maven repository url>` | 添加用于下载 OpenJFX 的自定义 Maven 仓库                                                                    |
| `-Dhmcl.native.encoding=<encoding>`          | 覆盖原生编码.                                                                                         |
| `-Dhmcl.microsoft.auth.id=<App ID>`          | 覆盖 Microsoft OAuth App ID.                                                                      |
| `-Dhmcl.microsoft.auth.secret=<App Secret>`  | 覆盖 Microsoft OAuth App 密钥.                                                                      |


## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fxqzi%2FPMCL.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fxqzi%2FPMCL?ref=badge_large)