---
layout: page
permalink: /blogs/text/index.html
title: text
---

#这是一级标题
Ctrl+b用来**加粗**,Ctrl+i用来 *斜体*

1.+空格用来表示有序列表
1. 这是个有序列表
2. ...
<u>下划线是这样子的</u>

<font color="red" size=3 face="仿宋">设置文字颜色为红色,字体为3号仿宋</font>
`文字高亮是这样子的`或者麻烦一点
<span style="background-color:yellow">这是一段高亮的文字</span>

##这是二级标题
可以直接识别$\LaTeX$语法,编辑公式相当简单.让我们来写一个经典的 **Maxwell方程组**:
\[ \left\{
        \begin{aligned}
            \nabla \cdot \boldsymbol{E}&=\dfrac{\rho}{\varepsilon_0}\\
            \nabla \times \boldsymbol{E}&=-\dfrac{\partial \boldsymbol{B}}{\partial t}\\
            \nabla \cdot \boldsymbol{B}&=0\\
            \nabla \times \boldsymbol{B}&=\mu_0 \boldsymbol{j}+\varepsilon_0 \mu_0\dfrac{\partial \boldsymbol{E}}{\partial t}
        \end{aligned}
    \right.\]
###这是三级标题
插图:Copy图片,然后Ctrl+Alt+V即可粘贴:
![这是一脸懵冰](2024-01-21-12-43-36.png)


## code
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

