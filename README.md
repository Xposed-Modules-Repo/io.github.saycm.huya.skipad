# 虎牙广告跳过模块

面向 LSPosed 的虎牙广告过滤模块，基于 libxposed API 102 开发，适配虎牙 **13.5.44**（versionCode `117129`）。

## 功能

- 拦截开屏广告。
- 过滤推荐列表中的广告卡片。
- 拦截自动推广弹窗和直播间外普通广告请求。
- 点击“看广告赚虎粮”等奖励广告入口时，直接完成原奖励完成、关闭和发奖流程。

## 兼容性

| 项目 | 版本或范围 |
| --- | --- |
| 目标应用 | 虎牙 13.5.44，versionCode `117129` |
| 模块版本 | 1.11，versionCode `12` |
| 模块包名 | `io.github.saycm.huya.skipad` |
| 作用域 | `com.duowan.kiwi` |
| Android | Android 10 及以上（API 29+） |
| 框架 | LSPosed，libxposed API 102 |

## 安装

1. 安装模块，并在 LSPosed 中启用。
2. 将作用域设置为虎牙 `com.duowan.kiwi`。
3. 强制停止虎牙并重新打开。

## 下载与源码

- [GitHub Releases](https://github.com/saycm/huya-ad-skip/releases)
- [源码仓库](https://github.com/saycm/huya-ad-skip)
- [完整变更记录](https://github.com/saycm/huya-ad-skip/blob/main/CHANGELOG.md)

## 版本变动

- 1.11：修复动态补丁加载后业务 Hook 未命中的问题，补充推荐广告回填、沉浸式推荐和列表写入时的广告过滤。
- 1.10：迁移至 libxposed API 102，使用现代模块元数据、包加载完成回调和拦截链接口。
- 1.9：更新 Application ID，适配虎牙 13.5.44，覆盖开屏、推荐列表、自动推广和奖励广告流程。
- 1.8：增加开屏广告、推荐列表广告和自动推广弹窗拦截。

## 许可证

本项目采用 [MIT License](LICENSE)。
