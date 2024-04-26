# sus.prom

### sus.prom

用于查看当前已有的提示词预设。

显示名词为提示词文件内的字段`name`。

### sus.prom.set

用于设定当前群聊/私聊上下文中使用的提示词预设。

参数：

- `name`：欲切换到的提示词预设的名称。

使用例：

`sus.prom.set 天凌钙`

设置成功将输出：`设置成功`

### sus.prom.exec

该指令用于渲染并输出指定提示词。

即将当前的提示词内`liquid`模板全部渲染后，以`yaml`形式输出。

参数：

- `name`：欲查看的提示词预设名称。

使用例：

`sus.prom.exec 天凌钙`

将输出：

```yaml
- role: system
  content: 
- role: system
  content: '与你进行对话的人类，昵称为 俗手'
- role: system
  content: |-
    用户所在时区当前时间为 2024-04-25 13:15:59
```

常用于调试提示词，相关指令有：sus.eval

### sus.prom.current

用于查看当前使用的提示词预设。

显示名词为提示词文件内的字段`name`。