# UABEA Android

Unity Asset Bundle Extractor 的 Android 移植版。

## 作者

- B站：https://b23.tv/xhTs9EN
- GitHub：https://github.com/nhnhbbj-oss

## 功能

- 打开 AssetBundle / .assets 文件
- 查看、编辑、导出、导入资产
- 贴图预览与替换（支持 RGBA32、BGRA32、ARGB32、RGB24、Alpha8、R8、ARGB4444、RGBA4444、RGB565、DXT1/BC1、DXT5/BC3、BC4、BC5、BC7、ETC_RGB4、ETC2_RGB4、ETC2_RGBA8、ASTC 4x4~12x12 LDR/HDR；Crunch 降级为基础格式）
- 音频预览与替换（支持 FSB、wav、ogg、mp3 等，不检查格式，游戏能否播放取决于游戏本身）
- 批量导入/导出贴图、音频
- Mod 制作（.emip 补丁包）

## 下载

从 [Releases](https://github.com/你的用户名/新仓库/releases) 页面下载最新 APK。

## 来源

- 基于 [ccss0101/uabea-android](https://github.com/ccss0101/uabea-android) 修改
- 上游项目：[nesrak1/UABEA](https://github.com/nesrak1/UABEA)，Copyright (c) 2021 nesrak1，MIT License
- 完整许可证文本见 [LICENSE](LICENSE)

## 已知限制

- PVRTC、EAC、YUY2、ETC2_RGBA1、BC6H 不支持
- Crunch 贴图替换时降级为基础格式，文件体积会变大
- 音频替换不检查格式，非 FSB 格式能否播放取决于游戏
