---
layout: page
permalink: /blogs/text/index.html
title: text
---
## Markdown 语法光速入门

#### 段落、字体
1. \#  这是一级标题 
2. \## 这是二级标题

  每写完一个段落要隔一行空行.

  就像这样， 隔了一行空行.

3. 用一前一后的\*\*围住用来**加粗**，使用一前一后的\*围住用来表示*斜体*.
   
4. 使用一前一后的\<u>和\</u>来表示<u> 下划线</u>

5. \<font color="red" size=3 face="仿宋">文字 \</font>
可以设置文字颜色为红色，字体为3号仿宋

6. 使用一前一后的\`围住文字用来`文字高亮`或者麻烦一点使用
\<span style="background-color:yellow">文字\</span>，后者可以设置用来文字高亮的颜色.

7. 一前一后的\~~用来表示~~删除线~~.

#### 插图

\![图片提示语]\(图片地址)，比如

![这是一脸懵冰](2024-01-21-12-43-36.png)


#### 数学公式

$$ 
\left\{
        \begin{aligned}
            \nabla \cdot \boldsymbol{E}&=\dfrac{\rho}{\varepsilon_0}\\
            \nabla \times \boldsymbol{E}&=-\dfrac{\partial \boldsymbol{B}}{\partial t}\\
            \nabla \cdot \boldsymbol{B}&=0\\
            \nabla \times \boldsymbol{B}&=\mu_0 \boldsymbol{j}+\varepsilon_0 \mu_0\dfrac{\partial \boldsymbol{E}}{\partial t}
        \end{aligned}
    \right.
$$


#### 代码环境
```LaTeX
\left\{
        \begin{aligned}
            \nabla \cdot \boldsymbol{E}&=\dfrac{\rho}{\varepsilon_0}\\
            \nabla \times \boldsymbol{E}&=-\dfrac{\partial
            \boldsymbol{B}}{\partial t}\\
            \nabla \cdot \boldsymbol{B}&=0\\
            \nabla \times \boldsymbol{B}&=\mu_0 \boldsymbol{j}
+\varepsilon_0 \mu_0\dfrac{\partial \boldsymbol{E}}{\partial t}
        \end{aligned}
    \right.
```
```Python
print("Hello world!")
```


#### 列表

* 无序列表
  * 嵌套无序列表
  * 嵌套无序列表
* 无序列表
* 无序列表

1. 有序列表 1
   1. 嵌套有序列表 1
   2. 嵌套有序列表 2
2. 有序列表 2
3. 有序列表 3

#### 引用文本:

> 引用别人说的话
> 就这样写
> By.Collapsar

---

这是 `行内代码` 语法.

代码块语法:

''' python
print("Hello， World!")
'''

请将 ' 替换成 `.

---

#### 表格:

| 表头 | 表头 |
| ---- | ---- |
| 内容 | 内容 |
| 内容 | 内容 |

---

#### 注释

\<!-- 理论上你看不见我 -->
