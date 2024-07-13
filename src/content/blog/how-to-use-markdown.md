---
title: Markdown语法
author: Motues
pubDatetime: 2024-07-10T20:14:00Z
slug: how-to-use-markdown
featured: true
draft: false
tags:
  - 其他
ogImage: ""
description: Motues的第一篇文章。
canonicalURL: https://motues.top/posts
---

## 目录

## 标题

一般来使用1-6个井号`#`来表示标题，例如：

```markdown
# 这是一级标题

## 这是二级标题

### 这是三级标题

#### 这是四级标题

#### 这是五级标题
```

显示如下：
![heading](/image/how-to-use-markdown/heading.png)

## 段落

### 段落

段落之间用空行开，段落前不使用空格或者缩进。

```markdown
这是第一段

这是第二段
```

### 换行

在行尾添加两个及以上的空格表示换行。

```markdown
这是第一行  
这是第二行
```

## 着重

### 粗体

在单词或短语的前后添加两个星号`**`或下划线`__`表示加粗。

```markdown
我喜欢**听歌**、**旅游**......
```

显示如下:  
我喜欢**听歌**、**旅游**......

### 斜体

在单词或短语的前后添加一个星号`*`或下划线`_`表示斜体。

```markdown
我喜欢*听歌*、_旅游_......
```

显示如下:  
我喜欢*听歌*、_旅游_......

### 粗体和斜体

在单词或短语的前后添加三个星号`***`**或**下划线`___`表示同时为粗体和斜体。

```markdown
我喜欢**_听歌_**、**_旅游_**......
```

显示如下:  
我喜欢**_听歌_**、**_旅游_**......

## 块引用

### 块引用

将单词或短语用右箭头`>`开头表示为块引用，需要用空格隔开。

```markdown
> 念念不忘，必有回响！
```

显示如下:

> 念念不忘，必有回响！

### 嵌套块引用

在段落前面添加一个双右箭头`>>`表示嵌套引用。

```markdown
> 念念不忘
>
> > 必有回响
```

显示如下:

> 念念不忘
>
> > 必有回响

## 代码

### 代码

将单词或者短语用勾号``括起来表示为代码。

```
在C++中，使用`cout`打印Hello World!
```

显示如下  
在C++中，使用`cout`打印Hello World!

### 代码块

代码块之前和之后的行上使用三个刻度线（```）或三个波浪号（~~~），并在第一行后面加入语言类型实现语法高亮。

````
```c++
#include <iostream>
using namespace std;

int main() {
  cout<<"Hello World!"<<endl;
  return 0;
}
```
````

结果如下所示

```c++
#include <iostream>
using namespace std;

int main() {
  cout<<"Hello World!"<<endl;
  return 0;
}
```

## 列表

### 有序列表

在段落前中添加数字和句点`.`表示有序列表。数字不必按数字顺序排列，但列表以数字开头显示。

```markdown
1. 第一项
1. 第二项
1. 第三项
```

显示如下:

1. 第一项
2. 第二项
3. 第三项

### 无序列表

在段落前添加一个星号`*`或减号`-`或圆点`.`表示无序列表。

```markdown
- 第一项

* 第二项
  . 第三项
```

显示如下:

- 第一项
- 第二项
- 第三项

### 在列表中添加元素

在列表中添加另一个元素（段落、块引用等），需要把该元素缩进四个空格或一个制表符。

```markdown
1. 第一项
   > 早睡早起
2. 第二项
```

显示如下:

1. 第一项
   > 早睡早起
2. 第二项

## 链接

### 链接

将文本括在方括号（例如[Motues]）中，然后在后面的括号加入URL表示链接。

```markdown
欢迎访问Motues的[Blog](https://motues.top)！
```

显示如下:  
欢迎访问Motues的[Blog](https://motues.top)！

### 链接标题

在URL后面的括号中添加标题，当用户将鼠标悬停在链接上时，这将显示提示。

```markdown
欢迎访问Motues的[Blog](https://motues.top "Motues's Blog")！
```

显示如下:  
欢迎访问Motues的[Blog](https://motues.top "Motues's Blog")！

## 图片

先感叹号（!），然后在括号中添加替代文本，并在括号中添加图像资源的路径或URL，也可以选择在括号中的URL之后添加标题。

```markdown
![Motues](/image/how-to-use-markdown/Motues.png "这是我的头像")
```

显示如下:  
<img src="/image/how-to-use-markdown/Motues.png" alt="Motues" title="这是我的头像" width="256" height="256">

## 表格

### 表格

要添加表，请使用三个或多个连字符（`---`）创建每列的标题，并使用竖线（`|`）分隔每列（每行每列不需要对齐）。

```markdown
| 水果   | 颜色 | 口感 |
| ------ | ---- | ---- |
| 西瓜🍉 | 绿色 | 甜   |
| 葡萄🍇 | 紫色 | 酸   |
```

显示如下:
| 水果 | 颜色 | 口感 |
| ---------- | ---------| ----|
| 西瓜🍉 | 绿色 | 甜 |
| 葡萄🍇 | 紫色 | 酸 |

### 对齐

可以通过在标题行内的连字符的左侧，右侧或两侧添加一个冒号`:`，以使列中的文本左，右或居中对齐。

```markdown
| 水果   | 颜色 | 口感 |
| :----- | :--: | ---: |
| 西瓜🍉 | 绿色 |   甜 |
| 葡萄🍇 | 紫色 |   酸 |
```

显示如下:
| 水果 | 颜色 | 口感 |
| :------ | :-----:| ----:|
| 西瓜🍉 | 绿色 | 甜 |
| 葡萄🍇 | 紫色 | 酸 |

### 转义字符

使用表格的HTML字符代码`&#124;`在表中显示竖线`|`字符

## 任务清单

任务列表项前需要添加破折号`-`和方括号`[]`，并在之间插入一个空格。如果要选择一个复选框，需要在方括号之间添加`x`。

```markdown
- [x] 吃饭
- [ ] 睡觉
- [ ] 打豆豆
```

- [x] 吃饭
- [ ] 睡觉
- [ ] 打豆豆

## 其他

### 删除线

在单词或短语的前后添加两个波浪线`~~`表示删除线。

```markdown
我不喜欢吃~~葡萄~~
```

显示如下:  
我不喜欢吃~~葡萄~~

### 水平线

在一行上使用三个或更多的星号（`***`），减号（`---`）或下划线（`___`）创建水平线。

```markdown
---
---

---
```

显示如下:

---

---

---