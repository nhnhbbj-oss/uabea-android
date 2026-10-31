# UABEA Android

## Unity Asset Bundle Extractor 的 Android 移植版。

⚠️ 重要提示：本工具为个人修改版，非官方发布。操作前请务必备份原文件。因使用本工具造成的文件损坏或数据丢失，作者不承担责任。

## 作者与维护

· 作者：nhnhbbj-oss
· B站：https://b23.tv/xhTs9EN
· GitHub：https://github.com/nhnhbbj-oss
· 项目状态：个人维护，随缘更新
· 问题反馈：欢迎在 GitHub Issues 反馈

## 与上游的关系

本项目基于 ccss0101/uabea-android 1.6.0 版本修改。上游项目为 nesrak1/UABEA，Copyright (c) 2021 nesrak1，MIT License。

## 相对 1.6.0 的主要改动：

· UI 重构：列表改为 DataGrid，增加多选、列头全选、详情面板、操作栏布局调整。
· 性能与稳定性：加载/保存/批量操作改为后台线程 + 分阶段进度。
· 功能扩展：内置插件系统、贴图解码增强、音频预览与替换（外部 resS / 内嵌两种）、Mod 制作（.emip）。
· Bug 修复：保存功能、文件信息界面、类型过滤后选中状态、全选状态同步等。

## 功能

· 打开 AssetBundle / .assets 文件 / level 文件 / .unity3d 文件
· 查看、编辑、导出、导入资产
· 贴图预览与替换（支持大部分格式；不支持：BC6H、PVRTC、EAC、YUY2、ETC_RGB4_3DS、ETC_RGBA8_3DS、RGBA64/RGB48）
· 音频预览与替换（支持外部 resS 与内嵌资源两种方式）
· 批量导入/导出贴图、音频
· Mod 制作（.emip 补丁包）
· 3D 预览（Mesh，可旋转）
· 场景层级
· 合并 split 后缀文件（.split0、.split1 等，必须选择 .split0 后缀才会自动合并）
· 文件信息
· 新增资产
· 类型筛选、搜索资产、跳转资产
· 插件系统

## 下载与校验

从 Releases 页面下载最新 APK。

## 项目 内容
最新版本 【1.1】
发布日期 【2026/10/31】
APK SHA-256 【A4:0D:A8:0A:59:D1:70:CA:A9:50:CF:15:C1:8C:45:4D:47:A3:9B:26:98:9D:8B:64:0E:CD:74:5B:A7:1B:F5:DC】

## 权限说明

· 文件读写权限：用于读取和写入本地的 AssetBundle、.assets、图片、音频、.emip 等文件。
· 网络：应用本身不申请网络权限；仅“关于”页面通过系统 Intent 打开浏览器访问 B站/GitHub。
· FileProvider：音频预览通过 FileProvider 临时共享缓存文件给系统播放器，不对外暴露。

## 已知限制

· 贴图预览限制 4096×4096，超过则跳过预览。
· 不支持的纹理格式：BC6H、PVRTC、EAC、YUY2、ETC_RGB4_3DS、ETC_RGBA8_3DS、RGBA64/RGB48。
· 合并 split 文件时，必须选择 .split0 后缀的文件才会自动合并。
· 批量导出大文件操作可能较慢。
· 音频替换和 UABE 一样，可能不支持一些加密或特殊格式。
· 插件系统仅支持 UABE 格式 DLL。
· Mod Maker 需要先打开并修改 .assets 文件。
· 其他已知问题：欢迎在 Issues 反馈。

## 安全提示

· 操作前请备份原始文件。

## 许可证

本项目基于上游 MIT License 发布，保留原版权声明，完整许可证文本见 LICENSE。

上游项目：Copyright (c) 2021 nesrak1，MIT License。

## 更新记录

· 【1.1】（【2026/10/31】）：基于 ccss0101/uabea-android 1.6.0 修改，详见上文「与上游的关系」。

## 免责声明

本工具仅供学习与研究使用。使用本工具修改游戏资源请在使用前备份原始文件，作者不对因使用本工具造成的任何损失负责。使用本工具修改游戏资源可能违反相关游戏服务条款，存在账号封禁风险。

> 此仓库只发布构建产物。

---
