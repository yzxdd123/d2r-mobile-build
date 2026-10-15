# 小红书社区安装笔记（用户存档）

来源：2026-10-15 用户转发的小红书笔记（号 1035244391）  
对应 release 示例：上游 [jiayx/d2r-mobile-build v1.0.15](https://github.com/jiayx/d2r-mobile-build/releases/tag/v1.0.15)（Game 3.3.94012）

> **说明**  
> 这是社区简化操作备忘，**不是**本仓库官方流程。完整、更准确的用法见根目录 [README.zh-CN.md](../README.zh-CN.md)（签名推荐 Sideloadly / AltStore / SideStore 等；资源拷到「文件 → 我的 iPhone → D2R Mobile」）。  
> 游戏资源请自备正版；不要把游戏本体 / RomFS / 证书提交进 git。

---

## 一、到 GitHub 下载文件

打开 release（示例）：

https://github.com/jiayx/d2r-mobile-build/releases/tag/v1.0.15

笔记里写要下：

- `D2RMobile-v1.0.15.ipa`
- `D2R-Mobile-Resources.zip.001`
- `D2R-Mobile-Resources.zip.002`
- `D2R-Mobile-Resources.zip.003`

（本 fork 之后自己用 Actions 打出来的 IPA 文件名会带 build 编号，按 Release 页实际文件为准。）

## 二、解压资源

三个分卷拼好后解压，得到文件夹：`D2R Mobile Resources`

## 三、手机签名安装 IPA

1. 手机打开 `iosxb.cn`，安装签名软件（全能签）。
2. 把 IPA 拷到手机。
3. 签名后安装。

（官方 README 另推荐 Sideloadly、iloader、AltStore Classic、SideStore。）

## 四、拷贝资源进 App 目录

用电脑连手机，把整个 `D2R Mobile Resources` 文件夹拷进应用目录。  
笔记原文写「拷贝到 ipa 文件目录」；按官方说明更准确的位置是：

**文件 App → 我的 iPhone → D2R Mobile**

（或 Mac：Finder → 手机 → 文件 → 该应用。）

## 五、首次启动

打开已安装的 App，等待 **5–7 分钟** 后再正常游玩。  
（官方说明：若停在资源提示页，可点「重试」让应用重新检测资源。）

---

## 相关仓库

| 仓库 | 用途 |
|---|---|
| 本仓库 `yzxdd123/d2r-mobile-build` | Actions 构建 IPA / macOS 包 |
| [`yzxdd123/d2r-mobile`](https://github.com/yzxdd123/d2r-mobile) | 源码 fork（已有） |
| 上游模板 [`jiayx/d2r-mobile-build`](https://github.com/jiayx/d2r-mobile-build) | 构建工作流上游 |
