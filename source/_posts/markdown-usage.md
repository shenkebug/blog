---
title: Markdown 语法一揽子计划（超详细）
date: 2020-02-02 11:08:08
categories: [Markdown]
tags: [Markdown]
---

## 1. 标题

使用 `#`表示 1~6 级标题

<!-- more -->

> \# 一级标题  
> \## 二级标题  
> \### 三级标题  
> \#### 四级标题  
> \##### 五级标题  
> \###### 六级标题

效果：

> # 一级标题
> ## 二级标题
> ### 三级标题
> #### 四级标题
> ##### 五级标题
> ###### 六级标题

## 2. 文本样式

> \`标记`  
> \*斜体\*，\_斜体\_  
> \*\*粗体\*\*，\_\_粗体\_\_  
> \*\*\_斜体+粗体\_\*\*     
> \<u\>下划线\<\/u\>    
> \~\~删除线\~\~

效果：

`标记`  
_斜体_，_斜体_  
**粗体**，**粗体**  
**_斜体+粗体_**     
<u>下划线</u>   
~~删除线~~

### 2.1 字体大小和颜色

字体大小使用 `<font></font>` 标签，该标签下的 `size` 属性为字体大小，范围为 1~7，`color` 属性为字体颜色，如 red、blue 等

> <font size=1 color=red>size=1 color=red</font>  
> <font size=2 color=blue>size=2 color=blue</font>  
> <font size=3 color=yellow>size=3 color=yellow</font>  
> <font size=4 color=green>size=4 color=green</font>  
> <font size=5 color=orange>size=5 color=orange</font>  
> <font size=6 color=gray>size=6 color=gray</font>  
> <font size=7 color=purple>size=7 color=purple</font>

## 3. 链接

链接有两种形式：行内式和参考式

### 行内式 <!-- omit in toc -->

> \[Google\]\(https://www.google.com "谷歌搜索"\)

效果：

[Google](https://www.google.com "谷歌搜索")

### 参考式 <!-- omit in toc -->

> \[Google\]\[1\]  
> \[Baidu\]\[2\]
>
> \[1\]: https://www.google.com "谷歌搜索"  
> \[2\]: https://www.baidu.com "百度一下"

效果：

[Google][1]  
[Baidu][2]

[1]: https://www.google.com "谷歌搜索"
[2]: https://www.baidu.com "百度一下"

## 4. 图片

插入图片和插入链接类似，只是需要在链接的基础上前面加一个 `!`

> \!\[icon](https://gitee.com/tsund/data/raw/master/favicon/favicon-180x180.png "icon")

效果：

<center>

![icon](https://gitee.com/tsund/data/raw/master/favicon/favicon-180x180.png "icon")

</center>

**另**：使用 `<center></center>` 嵌套使图片居中：

> \<center\>
>
> \!\[](url)
>
> \</center\>

## 5. 区块引用

使用 `>` 表示引用

> \> 区块引用  
> \>\> 嵌套引用

效果：

> 区块引用
>> 嵌套引用

## 6. 代码区块

在每行加上 4 个空格或者一个制表符

public static void main(String args[]){  
&nbsp;&nbsp;&nbsp;&nbsp;System.out.println("Hello World");  
}

效果：

    public static void main(String args[])
    {
        System.out.println("Hello World");
    }

**注意**：此时需要与普通段落之间存在空行

**或者**，使用\`\`\`包裹代码（推荐），如下：

> \`\`\`java  
> public static void main(String args[])  
>  {  
> &nbsp;&nbsp;&nbsp;&nbsp;System.out.println("Hello World");  
>  }  
> \`\`\`

**注意**：\`\`\`后面紧跟展示代码所使用的语言，如 java、javascript、python、shell 等

## 7. 目录

Markdown 自动生成目录详见：<https://blog.csdn.net/sculpta/article/details/104173014>

## 8. 列表

### 8.1 无序列表

使用 `·` 、`+` 、或 `-` 标记无序列表，可嵌套

> \- 第一项  
> \- 第二项  
> \- 第三项

效果：

- 第一项
- 第二项
- 第三项

### 8.2 有序列表

有序列表的标记方式是序号后面加 `.`

> 1\. 第一项  
> 2\. 第二项  
> 3\. 第三项

效果：

1. 第一项
2. 第二项
3. 第三项

## 9. 复选框

> \- [ ] a  
> \- [x] b  
> \- [ ] c  
> \- [x] d

效果：

- [ ] a
- [x] b
- [ ] c
- [x] d

## 10. 表情 😏

### 10.1 Emoji

目前 Emoji 已经支持大部分文本输入场景，当然也适用于 Markdown😆

**注意**：Emoji 表情在不同设备、不同软件、不同浏览器显示会有所不同

随便附上几个（直接选中复制、粘贴就 OK），更多可以参考 [Emoji All](https://copy.emojiall.com/zh-hans/ "Emoji All")

😀 😃 😄 😁 😆 😅 😂 😋 😒 😏 🙃 🙂 😐 😑 ⭐ 🌟 ✨ 🔥

### 10.2 符号表情

山顶洞人用的表情包 ʕ •ᴥ•ʔ

( ´◔ ‸◔`)

⊙▂⊙ 　 ⊙ ０ ⊙ 　 ⊙︿⊙ 　 ⊙ω⊙ 　 ⊙﹏⊙ 　 ⊙△⊙ 　 ⊙▽⊙

∩▂∩ 　 ∩ ０ ∩ 　 ∩︿∩ 　 ∩ω∩ 　 ∩﹏∩ 　 ∩△∩ 　 ∩▽∩

●▂● 　　 ● ０ ● 　　 ●︿● 　　 ●ω● 　　 ●﹏● 　　 ●△● 　 ●▽●

∪▂∪ 　 ∪ ０ ∪ 　 ∪︿∪ 　 ∪ω∪ 　 ∪﹏∪ 　 ∪△∪ 　 ∪▽∪

≧▂≦ 　 ≧ ０ ≦ 　 ≧︿≦ 　 ≧ω≦ 　 ≧﹏≦ 　 ≧△≦ 　 ≧▽≦

＞ ▂ ＜　＞０＜　＞︿＜　＞ ω ＜　＞﹏＜　＞ △ ＜　＞ ▽ ＜

> 参考链接： [标点符号表情大全](https://www.douban.com/note/227408401/ "标点符号表情大全")

## 11. 分割线

使用三个或以上 `*` 、 `-` 、 `_`

效果：

---

## 12. 表格 😂

用 `|` 表示表格纵向边界，表头和表内容用 `-` 隔开，并可用 `:` 进行对齐设置——两边都有 `:` 则表示居中，若不加 `:` 则默认左对齐

> | 表头 | 内容 |  
> \| :----: | :----------------------: |  
> | Google | <https://www.google.com> |  
> | Baidu | <https://www.baidu.com> |

效果：

|  表头  |           内容           |
| :----: | :----------------------: |
| Google | <https://www.google.com> |
| Baidu  | <https://www.baidu.com>  |

## 13. 注脚

> 一个具有注脚的文本。\[^1\]
> 
> \[^1\]: 注脚的解释

效果：

一个具有注脚的文本。[^1]

[^1]: 注脚的解释


## 14. 折叠内容

> \<details>  
> \<summary>Title（点击展开隐藏内容）\</summary>
>
> content
>
> \</details>

效果：

<details>
<summary>Title（点击展开隐藏内容）</summary>

content

</details>

**注意**：部分场景（如 CSDN）可能不支持该语法，不过在 vs code、github 等场景可以正常显示

## 15. 数学公式 😉

> 详细数学公式语法，链接：[Markdown 语法之数学公式（from CSDN）](https://blog.csdn.net/sculpta/article/details/104142503)
