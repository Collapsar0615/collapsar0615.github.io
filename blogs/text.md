---
layout: page
permalink: /blogs/text/index.html
title: text
---
## Markdown 语法光速入门

#### 段落、字体

\# 这是一级标题

\## 这是二级标题

...

Ctrl+b或者用两个** 围住用来**加粗**字,Ctrl+i或者一个* 围住用来*斜体*.
   
使用头尾的\<u>和\</u>来表示<u> 下划线</u>

\<font color="red" size=3 face="仿宋">文字 \</font>
可以设置文字颜色为红色,字体为3号仿宋

两个\`围住\用来`文字高亮`或者麻烦一点使用
\<span style="background-color:yellow">文字\</span>

#### 列表环境

有序列表:
1.+空格用来表示有序列表

1. 这是个有序列表
2. ...
   
无序列表:

- 第一项
- 第二项


#### 插图

Copy图片,然后Ctrl+Alt+V即可粘贴:

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

