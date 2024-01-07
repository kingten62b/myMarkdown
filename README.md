# MarkDown
- [MarkDown](#markdown)
  - [预备](#预备)
    - [编写环境](#编写环境)
    - [全角/半角标点](#全角半角标点)
  - [段落与换行](#段落与换行)
    - [分段](#分段)
    - [换行](#换行)
  - [分割线](#分割线)
  - [标题 \[数个 "#" + 空格\]](#标题-数个---空格)
  - [加粗 \[用 "\*\*" 或 "\_\_" 包围\]](#加粗-用--或-__-包围)
  - [斜体 \[用 "\*" 或 "\_" 包围\]](#斜体-用--或-_-包围)
  - [删除线 \[用 "~~" 包围\]](#删除线-用--包围)
  - [代码 \[用 "\`" 包围\]](#代码-用--包围)
  - [代码块 \[用 "\`\`\`" 包围\]](#代码块-用--包围)
  - [引用 \["\>" + 空格\]](#引用---空格)
  - [无序列表 \["-" 或 "+" + 空格\]](#无序列表---或---空格)
  - [有序列表 \[数字 + "." + 空格\]](#有序列表-数字----空格)
  - [链接 \[用 "\[ \]" + "( )" 分别包围文本与链接\]](#链接-用------分别包围文本与链接)
  - [任务列表 \["- \[ \]" + 空格\]](#任务列表------空格)
  - [表格](#表格)
  - [图片](#图片)
  - [Emoji 表情](#emoji-表情)
  - [内嵌HTML](#内嵌html)
  - [转义字符](#转义字符)
  - [目录生成](#目录生成)
  - [扩展语法](#扩展语法)

## 预备

### 编写环境

**vscode** + 插件 **Markdown All in One**  
或者使用 Typora

### 全角/半角标点

`Ctrl` + `.` 切换全角/半角标点

**全角/半角标点** 例如，和,  
~~或者你也可以直接安装Windows英文语言包，`win` + `空格`切换英文输入模式~~

## 段落与换行

### 分段

空白行将一行或多行文本进行分隔,即可分段

段落1

段落2

### 换行

行尾加两个或多个空格,即可换行  
也可以用另一种换行方式：HTML 的 `<br>` 标签换行

## 分割线

在单独一行上使用三个或多个`***`、`---`或`___` ，并且不能包含其他内容  
**为了兼容性，请在分隔线的前后均添加空白行**

____

我是分割线

___

## 标题 [数个 "#" + 空格]

```
# 一级标题
## 二级标题
### 三级标题
```

**为了不同的 Markdown 应用程序处理兼容考虑,最好在`#`后加空格**

## 加粗 [用 "**" 或 "__" 包围]

```
**加粗**
不加粗
```

**加粗**  
不加粗

也可选中文字后按下`Ctrl` + `B`

## 斜体 [用 "*" 或 "_" 包围]

```
*斜体*
不斜体
```

*斜体*  
不斜体

也可选中要加粗文字后按下`Ctrl` + `I`

## 删除线 [用 "~~" 包围]

```
~~删除~~
不删除
```

~~删除~~  
不删除

## 代码 [用 "`" 包围]

```
`sudo rm -rf /*`
```

`sudo rm -rf /*`  
~~清理Linux系统垃圾文件~~

## 代码块 [用 "```" 包围]

```
#include <stdio.h>
int mian() {
    print("Hello, world!\n");
    retrun O;
}
```

```c
#include <stdio.h>
int mian() {
    print("Hello, world!\n");
    retrun O;
}
```

使用` ``` `+ `对应语言`  
代码块里会根据语言来自动高亮各个语句

## 引用 [">" + 空格]

```
> 引用
>> 嵌套引用
```

> 引用
>> 嵌套引用

## 无序列表 ["-" 或 "+" + 空格]

```
+ 列表
  + 按`Tab`可以缩进一级
    + 按`Tab`可以缩进一级
```

+ 列表
  + 按`Tab`可以缩进一级
    + 按`Tab`可以缩进一级

## 有序列表 [数字 + "." + 空格]

```
1. 列表
2. 按`Enter`可以自动补全
   1. 按`Tab`可以缩进一级
```

1. 列表
2. 按`Enter`可以自动补全
   1. 按`Tab`可以缩进一级

## 链接 [用 "[ ]" + "( )" 分别包围文本与链接]

```
[bing](bing.com "鼠标悬停显示文字")
```
[bing](bing.com "鼠标悬停显示文字")

也可以使用尖括号可以把URL或者email地址变成可点击的  
<https://bing.com>

## 任务列表 ["- [ ]" + 空格]

```
- [ ] todo
- [x] finish
```

- [ ] toDo
- [x] finish

## 表格

```
| 学号 | 姓名 | 年龄 |
| :-------------: | :-------- | ---------------: |
| `-` 决定长度 | 1 |  2 |
| `:` 决定对齐方式 | 1 |  2 |
| 居中 | 靠左 |  靠右 |
```

| 学号 | 姓名 | 年龄 |
| :-------------: | :-------- | ---------------: |
| `-` 决定长度 | 1 |  2 |
| `:` 决定对齐方式 | 1 |  2 |
| 居中 | 靠左 |  靠右 |

## 图片

```
![替代文本](图片的位置 "鼠标悬停显示文字")
![替代文本](./picture/2d04a3af2edda3cc12291b9601e93901203f926d.png "鼠标悬停显示文字")
也可以配合图床
![理塘丁真](https://postimage.me/images/2024/01/04/2daeafec8a136327ef22e003d78fa0ec09fac7a0.jpeg)
```

!["鼠标悬停显示文字"](./picture/2d04a3af2edda3cc12291b9601e93901203f926d.png "鼠标悬停显示文字")

推荐一个好用的图床[postimage](https://postimage.me/)  
![2daeafec8a136327ef22e003d78fa0ec09fac7a0.jpeg](https://postimage.me/images/2024/01/04/2daeafec8a136327ef22e003d78fa0ec09fac7a0.jpeg)

## Emoji 表情

分享一个可以复制Emoji的网站:[传送门](https://emojipedia.org/)  
🤡 ~~天哪这简直就是我~~

## 内嵌HTML

直接用`<></>`包围就行

<div>
我来自HTML<br>
<a target="_blank" href="https://developer.mozilla.org/zh-CN/docs/Web/HTML"  style=""><strong>HTML</strong>（超文本标记语言） - MDN Web Docs</a>
</div>

还可以插入音乐 ~~敌在本能寺~~

<iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width=330 height=86 src="//music.163.com/outchain/player?type=2&id=1881994446&auto=1&height=66"></iframe>

## 转义字符

字符前加`\`,实现转义

例如`*\*nnn\**`,渲染效果 *\*nnn\**

## 目录生成

**Typora**可以使用`[toc]` *Table of Contents* 自动生成目录  
**vscode** + 插件 **Markdown All in One** 可以`Ctrl` + `shift` + `P` 在命令面板中输入`Create Table of Contents` 自动生成目录

## 扩展语法

大部分Markdown应用程序支持以上常用语法,扩展语法 *(不保证兼容性)* 可参阅 [markdown扩展语法](https://markdown.com.cn/extended-syntax/)