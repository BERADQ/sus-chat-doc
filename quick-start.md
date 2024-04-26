# 快速开始

### 条件

使用本插件需要自备 openai api。

### 环境

本插件用于 koishi，使用前请确保已有 koishi 环境并已安装本插件。

相关：

- [Koishi 机器人框架](https://koishi.chat/zh-CN/)
- [sus-chat](https://github.com/BERADQ/koishi-sus-chat)

### 初步配置

当你安装了本插件，并将其添加到 koishi 中。

你将会看到本插件的配置页面。

请先将准备好的 API 与 key 填入。

1. 如果你使用 openai 官方 API，它看起来应该是这样的：`https://api.openai.com/v1/chat/completions`。
2. 非官方 API 请于供应商提供的 API 尾部添加 `/v1/chat/completions`。
3. key 一般是 `sk-`开头的一段文本。
4. 请保证前后无空白字符。

当你配置好 API 与 key，请使用 sus 指令进行一次对话，测试是否成功对接 API。

例子：

- `sus 你好`。
- `你好，有什么可以帮助你的吗？`
