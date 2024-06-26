# 提示词

### 基础提示词

当你未开启**高阶提示词**时，基础提示词会被使用。

基础提示词往往是一句话，是一条`system`消息，指定 AI 需要遵守的行为。

基础提示词也是一个`liquid`模板，你可以在其中使用`{{ value }}`来使用变量。

常用的变量有：

- `{{ session }}`：当前会话。
  - `{{ session.user }}`：用户
    - `{{ session.user.name }}`：用户名
    - `{{ session.user.id }}`：用户 ID
  - `{{ session.channel }}`：频道
    - `{{ session.channel.id }}`：频道 ID
  - `{{ session.guild }}`：群组
    - `{{ session.guild.id }}`：群组 ID

你还可以在其中使用标签或过滤器等`liquid`语法，详见[文档](https://liquid.bootcss.com/)。

### 高阶提示词

欲使用高阶提示词，请先开启高阶提示词。

开启高阶提示词后，基础提示词将不会被使用。

#### 提示词文件所在目录

用于存放高阶提示词文件的目录。

本项为必填项，默认为 koishi 实例目录下的`sus-chat`。

请进行下列操作：

1. 在任意位置创建一个文件夹用于存放提示词文件。
2. 将插件设置中的提示词文件所在目录选择为刚刚创建的文件夹。

注意事项：

- 目录路径及其名称不存在任何非法字符。
- 目录下必须包含一个以上的提示词文件。
- 提示词文件必须合法，如果出现扩展名为`.yml`但格式不正确的提示词文件，会导致插件不可用。
- 目录下的提示词文件的`name`条目必须唯一。
- 如果没有任何报错，但`sus.prom`查看不到想要的提示词，请确认文件扩展名是否为`.yml`。
- 如果没有`sus.prom`及其相关指令，请确认使用高阶提示词配置项已启用。

#### 默认提示词

默认提示词项目应填写提示词文件的`name`条目。

可以进行如下操作完成配置：

1. 将提示词文件以文本文档打开，查看其`name: `后的内容。
2. 将查看到的`name`填入默认提示词中。

注意事项：

- 请务必保证默认提示词存在。
- 请务必保证默认提示词合法。
- 如果默认提示词无法被加载，会导致插件不可用。
