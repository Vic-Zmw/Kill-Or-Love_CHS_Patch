# 识渡汉化组Kill Or Love汉化补丁 / °Know Team Kill Or Love Simplified Chinese localization patch

适用于 Steam 版 *Kill or Love*（Ren'Py 7.3.5，游戏目录为 `Steam\steamapps\common\Kill or Love`）。

## 安装

适用系统：Windows

运行方式：解压至游戏目录下覆盖原文件即可。

1. 下载本仓库：右上角 `Code → Download ZIP`（或从 [Releases](../../releases) 下载打包版）；
2. 解压后得到 `Kill-Or-Love_CHS_Patch-main/game/`；
3. 把其中的 `game` 文件夹拖进游戏根目录（与 `KillOrLove.exe` 同级），选择覆盖。

语言切换：启动游戏后进入「设置 → Language → 简体中文」。首次启动会重新编译脚本，比平时慢几秒属正常现象。

若游戏仍是英文界面，说明旧编译产物被优先加载了：删除 `game/gui.rpyc`、`game/screens.rpyc`、`game/tl/chinese/script.rpyc` 以及 `game/cache/*.rpyb` 后重启即可。

字体：Noto Sans SC（已随包附带 game/NotoSansSC-Regular.otf，无需另行安装）

## 本修订版说明（2026-11）

- 修复 `tl/chinese/options.rpy` 第 10 行的双重转义（反斜杠引号多写了一层），原版会报 `Could not parse string` 导致游戏无法启动。
- 随包补上缺失的 `game/NotoSansSC-Regular.otf`。原版只在 `gui.rpy` 里引用该字体却未附带文件，覆盖后会报 `Could not find font`。
- 补全原版未翻译的 1798 条对话；对原有译文逐条复核英文原文，修正错行、误译与人名串位。
- 全篇人名统一为英文原名（Jack / Anna / Grace / Buddy / Don / Mr. Friday），中英文混排统一加空格。
- 文中的「设置 → Language」入口由 `screens.rpy` 提供，若界面仍是英文，说明 `screens.rpy` 未生效，请确认覆盖完整。

## 致谢

感谢以下成员的贡献

LeanderLin(监制)

YEE(翻译)

Yolen(审校)

Heguang1112(翻译)

Kalakala(审校)

如果有署名有问题，可以随时提出修改。

**最后感谢使用本汉化的你。**

## 声明

本补丁为民间汉化，仅供学习交流使用，请支持正版。游戏本体版权归原作者 Andy Church 所有，本仓库不包含任何游戏资源文件。字体 Noto Sans SC 以 SIL Open Font License 1.1 授权，详见 [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md)。
