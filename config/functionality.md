# 功能性

### 消息记录持久化

启用后，将会于存储中记录消息而不是内存。

最直接的影响是：

- 重启 koishi 消息记录（记忆）不会消失。
- 重启插件同理。

### 随机回复

随机回复仅为娱乐性功能，未知其用途请不要开启。

#### 随机回复概率

随机回复的概率。

#### 是否影响关键词匹配

如果启用，随机回复的概率将会影响关键词匹配的概率。

关键词将不会 100% 响应，而是符合随机响应的概率。

本功能暂无用途（都随机回复了，关键词再随机不就没意义了吗？）。

### 关键词触发

#### 触发关键词

填写关键词。当用户提及关键词，会触发 AI 回复。

注意事项：
- 不要留有空白关键词，否则 AI 将会响应每条消息。
- 前后空白字符也会被匹配。

#### 关键词是否使用正则表达式

开启后，关键词将具备正则表达式匹配的能力。