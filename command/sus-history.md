# sus.history

### sus.history

该命令用于查看当前群聊/私聊上下文中，当前提示词的对话历史记录。

历史记录将以 YAML 格式输出，它看起来应该是这样的：

```yaml
- role: user
  content: 你好
- content: 你好！有什么可以帮助你的吗？
  role: assistant
```

### sus.history.clean

该指令用于清空当前群聊/私聊上下文中，当前提示词的对话历史记录。

清空成功将输出：`清空成功`