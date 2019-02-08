# ASF 简体中文翻译规范/说明

## 中文翻译的通用规则

* 遵守官方的本地化规则
* 避免错别字，注意用字用词规范（“的地得”的区别，“其他”而非“其它”等）
* 指代用户的 `you` 尽量翻译成“您”而非“你”，但是“你们”不可以写成“您们”（这条只是为了全文的一致）

## 术语

* 注意不要翻译一些虽然不在代码块中，但是尚未有通用译文或者不应该翻译的词汇，例如：`Docker`（一种软件）、`Master`（用户权限相关的属性值）、`Generic`（ASF 的一种包），不过如果它们出现在正文中，可以按情况考虑是否加括号说明
* 有下划线的术语，需要根据实际情况选择翻译（例如 `bot` 通常应翻译为“机器人”而不是保留原文，又例 `issue` 在“本地化”中应按照术语提示译为“议题”，但其他情况应该按照情况翻译）

## 标点符号与空白

* 除特殊情况外，应将普通标点符号转换标准的中文全角符号（特殊情况：一些文本以英文冒号和一个空格结尾，表示这里需要用户输入，则保持原符号不动）
* 引号`“”`、省略号`……`、破折号`——`等规范使用，将英文中表示并列部分的逗号妥当改为顿号`、`
* 斜线 `/`、竖线 `|` 等全角形式不常用的标点符号仍用半角形式
* 通常全角文本与半角文本之间应加入一个空格，例如 `正在启动 IPC 服务……`，但是一般全角标点符号与半角字符之间无需再加空格（因为全角标点通常自带空白），例如 `这包括 ASF-WebConfigGenerator（配置生成器）`
* 目前斜线 `/` 两侧都不加空格，竖线 `|` 两侧各有一个空白（空格或全角符号自带的空白皆可）

## 其他

* 引用文本优先直接使用被引用方提供的中文文本，如果没有中文再自行翻译，涉及到 Steam 协议、软件许可等法律文件，应保留英文原文，并在括号内提供参考译文
* 如果实在不确定应该如何翻译，可以在 Comment 中讨论
* 其他情况可以先参考已通过审批的译文，保持格式的一致性，并在讨论区中展开讨论
* 目前的审批过程仅仅是为了修正过去的错误翻译，以及明确规范，不代表不可更改，欢迎您继续提供更好的翻译建议（一般所有新翻译我都会看，不需要发 issue）

# 一些 Wiki 相关的说明（坑）

* Wiki 页面的翻译结果，实际上每句话之间有一个空格，显然是之前 Crowdin 分割留下的，不影响效果，有空格就有空格吧
* 由于发现 GitHub 对于强调+链接的语法渲染有点奇怪（`示例**[链接](http://xxxxx)**示例` 中的强调会失效，但强调两侧有空格则正常），所以我会在这样的地方插入零宽空格以保证排版较好的情况下正确渲染：`示例&#8203;<strong><a href="http://xxxxx">链接</a></strong>&#8203;示例`
