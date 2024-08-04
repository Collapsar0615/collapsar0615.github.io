---
layout: page
permalink: /blogs/qft/index.html
title: qft
---

---
puppeteer:
  displayHeaderFooter: true
  headerTemplate: '<span class="pageNumber"></span>'
  footerTemplate: '
    <div style="font-size: 15px; margin-left: 20px;">
    <span class="pageNumber"></span> / 
    <span class="totalPages"></span>
    </div>
    '
---
<style>
img{
    width: 60%;
    padding-left: 20%;
}
</style>

<font  face="仓耳明楷">

## 余钊焕《量子场论讲义》知识梳理 

> Collapsar,July 30,2024

---

## 第1章 预备知识

1. 组成物质的基本单元是**粒子**(particle).自然界存在的4种基本相互作用为
   - **引力相互作用**,gravitational interaction
   - **电磁相互作用**,electromagnetic interaction
   - **强相互作用**,strong interaction
   - **弱相互作用**,weak interaction
2. **基本粒子**是指尚未发现内部结构的粒子. 
    3代基本费米子(fermion)由带电轻子(lepton)+中微子(neutrino,中性轻子)+下型夸克+上型夸克构成,具体为

<div style="border: 2px solid blue; padding: 10px; display: inline-block;">

   - 1st:电子(e)+电子型中微子$(\nu_e)$+下夸克(d)+上夸克(u)
   - 2nd:$\mu$子$(\mu)+\mu$子型中微子$(\nu_\mu)$+奇夸克(s)+粲夸克(c)
   - 3rd:$\tau$子$(\tau)+\tau$子型中微子$(\nu_\tau)$+底夸克(b)+顶夸克(t)

</div>
<br>
某代某种费米子与它在另一代中相应的费米子具有相同量子数,但是质量不同.

夸克的种类从称为**味道**(flavor),6种味道的夸克具有不同的质量,每一味夸克都具有3种**颜色**,同味异色的夸克具有相同质量,严格构成颜色三重态,与描述强相互作用的量子色动力学有关.多个夸克通过强相互作用构成**强子**(hadron),如

<div style="border: 2px solid blue; padding: 10px; display: inline-block;">

- 介子(meson)=正夸克+反夸克
- 重子(baryon)=三个正夸克/三个反夸克
</div>
<br>
除了三代中微子以外的基本 费米子都有电荷,参与电磁相互作用,相应的理论称为**量子电动力学**.所有的基本费米子都参与弱相互作用,与电磁相互作用统一由**电弱规范理论**描述,电弱规范理论和量子色动力学构成**标准模型**(standard model).标准模型中费米子的相互作用由一些基本玻色子传递

<div style="border: 2px solid blue; padding: 10px; display: inline-block;">

- 胶子(gluon):传递夸克间强相互作用的规范玻色子
- 光子(photon):传递电磁相互作用的规范玻色子
- $W^{\pm},Z^0$玻色子:传递弱相互作用的规范玻色子
- $Higgs$玻色子:与电弱规范对称性的自发破缺以及基本粒子的质量起源有关
</div>
<br>

3. $Klein-Gordon$方程

Klein-Gordon方程用以描述单粒子的相对论性运动,它是第一个相对论性的波函数方程,形式为  
$$
   \boxed{-\hbar^2\dfrac{\partial^2}{\partial t^2}\Psi(\boldsymbol{x},t)=(-\hbar^2c^2\nabla^2+m^2c^4)\Psi(\boldsymbol{x},t).\tag{1}
   }$$


Klein-Gordon方程存在如下问题:
   - **负能量困难**.Klein-Gordon方程给出的自由粒子能量为
   $$
   E=\pm\sqrt{|\boldsymbol{p}|^2c^2+m^2c^4},\tag{2}
   $$
   其中$\boldsymbol{p}$为粒子动量,$m$为粒子静止质量.能量可以为正也可以为负.
   - **负概率困难**.通过Klein-Gordon方程构造的符合概率守恒的连续性方程要求粒子在空间中的概率密度为
   $$
   \rho=\dfrac{i\hbar}{2mc^2}\left(\Psi^*\dfrac{\partial \Psi}{\partial t}-\dfrac{\partial \Psi^*}{\partial t}\Psi\right),\tag{3}
   $$
   这样定义的概率密度并不总是正的.负概率问题的根源在于方程中含有波函数对时间的二阶导数.

4. $Dirac$方程与量子场论
   
Dirac方程克服了负概率问题,只包括对时间的一阶导数,且具有$Lorentz$协变性,用以描述自旋1/2的粒子,一开始是用来描述电子的. 

   Dirac方程能够保证概率密度正定和概率守恒,但负能量问题依旧存在.为此,Dirac提出:<span style="color:red;">真空(vacuum)是所有$E<0$的态都被填满而所有$E>0$的态都为空的状态.</span>如此,泡利不相容原理会阻止正能量的电子跃迁到负能量的态,因而激发态电子能量总是正的.如果负能海中缺少一个带有电荷-e和负能量的电子,即产生一个空穴(hole),则空穴的行为等价于一个带有电荷e和相应正能量的“反粒子”(antiparticle),称为**正电子**(positron).

   Dirac方程存在如下问题:
   - 并未观测到无穷多个负能电子具有的无穷大电荷密度所引起的电场.
   - Dirac方程一开始作为描述单粒子波函数方程提出来,但Dirac的解释包含了无穷多个粒子.
   - 整数自旋的玻色子不满足泡利不相容原理,空穴理论无法解释它们的负能量问题.
   - Dirac方程不能解决整数自旋粒子的负概率困难.

使用相对论性波函数方程描述单粒子遇到这么多困难,是因为在量子力学中时间与空间不平权,而狭义相对论中时间和空间则是完全对等的.
- 量子力学:时间$t$作为一个观测量并没有使用厄米算符描写,而空间$\boldsymbol{x}$则使用位置算符$\hat{x}$描写.
- 狭义相对论:$Lorentz$协变性将时空完全对等起来.

为此,存在以下两种解决方法
  - 将时间提升为一个厄米算符.(实际操作非常困难)
  - 将空间位置降格为一个参数,不再由厄米算符描述.具体来说是在每个空间点$\boldsymbol{x}$处定义一个算符$\hat{\phi}(\boldsymbol{x})$,所有这些算符的集合称为**量子场**.如此,<span style="color:red;">
  量子化的对象变成是由依赖于时空坐标的场组成的动力学系统, 
   </span>
   称为**量子场论**.

- 量子场论平等的描述正反粒子,由正反粒子产生和湮灭算符表达的哈密顿量是正定的,不再出现负能量困难.
- 不再将$\rho$解释为单粒子概率密度,而是解释为单位体积内正反粒子数目之差,不存在负概率困难.

5. 自然单位制

自然单位制取$\hbar=c=1$,而且
$$1\text{GeV}^{-1}=6.582\times 10^{-25}\text{s}=1.973\times 10^{-14}\text{cm},\tag{4}$$
自然单位制中,速度没有量纲;长度与时间的量纲相同,是能量量纲的倒数;能量、质量和动量具有相同的量纲.
在量子场论中,通常再取**真空介电常数**$\varepsilon_0=1$,这样精细结构常数(fine-structure constant)$\alpha$为
$$\alpha=\dfrac{e^2}{4\pi\varepsilon_0\hbar c}=\dfrac{e^2}{4\pi}\approx\dfrac{1}{137} \tag{5},$$
同时可得真空磁导率$\mu_0=(\varepsilon_0c^2)^{-1}=1$,
这样的单位制称为**有理化**的自然单位制.

6. $Lorentz$变换和$Lorentz$群&$Lorentz$张量
   
   略,参见梁灿彬《微分几何入门与广义相对论》上册前5章以及中册附录G相关内容.
7. 作用量原理
   
对于具有$n$个自由度的系统,可以定义$n$个相互独立的**广义坐标**(generalized coordinate)$q_i$,它们的时间导数是**广义速度**(generalized velocity)$\dot{q}_i=\dfrac{\text{d}q_i}{\text{d}t}$,从而将拉格朗日量(Lagrangian)表达为广义坐标与广义速度的函数$L(q_i,\dot{q}_i)$.拉格朗日量的时间积分
$$\boxed{S=\int_{t_1}^{t_2}\text{d}tL[q_i(t),\dot{q}_i(t)]\tag{6},}$$
称为**作用量**.

最小作用量原理指出,<span style="color:red;">
作用量的变分极值($\delta S=0$)对应于系统的经典运动轨迹.
</span>
对式(6)进行变分,再令之为零,可得到**Euler-Lagrange方程**
$$\boxed{\dfrac{\text{d}}{\text{d}t}\dfrac{\partial L}{\partial\dot{q}_i}-\dfrac{\partial L}{\partial q_i}=0,i=1,\cdots,n.}\tag{7}$$

引入**广义动量**(generalized momentum)
$$
p_i\equiv\dfrac{\partial L}{\partial \dot{q}_i},i=1,\cdots,n.
\tag{8}$$
求解上述方程,将广义速度表示为$q_i,p_i$的函数$\dot{q}_i(q_i,p_i)$,通过Legendre变换定义**哈密顿量**(Hamiltonian)
$$H(q_i,p_i)\equiv p_i\dot{q}_i-L,\tag{9}$$
用$H$取代$L$来表示作用量$S$,取作用量的变分并令之为零,可得**Hamilton正则运动方程**
$$
\boxed{
\left\{
\begin{aligned}
\dot{q}_i&=\dfrac{\partial H}{\partial p_i}\\
\dot{p}_i&=-\dfrac{\partial H}{\partial q_i}\\
i&=1,\cdots,n
\end{aligned}
\right.
}
\tag{10}
$$

相当于用$2n$个一阶方程代替原来的$n$个二阶Euler-Lagrange方程(7).广义坐标$q_i$与广义动量$p_i$统称为**正则变量**.

场是时空坐标$x^\mu$的函数,在经典场论中,场$\phi(\boldsymbol{x},t)$是系统的广义坐标,每一空间点$\boldsymbol{x}$都是一个自由度,因此场论相当于具有无穷多个连续自由度的质点力学.局域场论中,拉格朗日量表达为
$$
L(t)=\int\text{d}^3x\mathcal{L}(x),\tag{11}
$$
其中$\mathcal{L}(x)$称为**拉格朗日量密度**,以下将简称为拉氏量.“局域”的含义是$\mathcal{L}(x)$只依赖于一个时空点$x^\mu$,不再依赖于其他时空点.设
$\mathcal{L}$是系统中$n$个场
$\phi_a(\boldsymbol{x},t),a=1,\cdots,n$及其时空导数
$\partial_a\phi_a$的函数,则**作用量**表达为
$$
\boxed{S=\int \text{d}tL=\int \text{d}^4x\mathcal{L}(\phi_a,\partial\mu\phi_a).}\tag{12}
$$
对上式取变分,令之为零可得**场的Euler-Lagrange方程**
$$\boxed{\partial_\mu\dfrac{\partial \mathcal{L}}{\partial(\partial_\mu\phi_a)}-\dfrac{\partial\mathcal{L}}{\partial \phi_a}=0,a=1,\cdots,n,}\tag{13}$$
它给出场的经典运动方程.场的**共轭动量密度**(conjugate momentum density)或者正则共轭场定义为
$$
\pi_a(\boldsymbol{x},t)\equiv\dfrac{\partial \mathcal{L}}{\partial \dot{\phi}_a},\tag{14}
$$
用Legendre变换将哈密顿量定义为
$$
H\equiv\int \text{d}^3x \pi_a\dot{\phi}_a-L\equiv\int \text{d}^3x\mathcal{H},\tag{15}
$$
其中$\mathcal{H}(\phi_a,\pi_a,\nabla\phi_a)=\pi_a\dot{\phi}_a-L$是**哈密顿量密度**.以$\mathcal{H}$代替$\mathcal{L}$,改写作用量,然后对作用量取变分再取为零,得到**场的正则运动方程**
$$
\boxed{
\left\{
\begin{aligned}
\dot{\phi}_a&=\dfrac{\partial \mathcal{H}}{\partial t},\\
\dot{\pi}_a&=-\dfrac{\partial \mathcal{H}}{\partial \phi_a}+\nabla\cdot\dfrac{\partial\mathcal{H}}{\partial(\nabla\phi_a)}.
\end{aligned}
\right.}
\tag{16}$$
场$\phi_a$和它的共轭动量密度$\pi_a$是系统的正则变量.

8. Noether定理、对称性与守恒律

连续变换对应的对称性称为**连续对称性**.Noether定理指出,
<span style="color:red;">
如果系统具有一种连续对称性,就必然存在一条对应的守恒定律.
</span>
它适用于所有物理行为由作用量原理决定的系统.

**Noether守恒流**(conserved current)定义为
$$j^\mu\equiv \dfrac{\partial \mathcal{L}}{\partial(\partial_\mu\phi_a)}\overline{\delta}\phi_a+\mathcal{L}\delta x^\mu,\tag{17}$$
**守恒流方程**为
$$\partial_\mu j^\mu=0,\tag{18}$$

方程(18)两边对空间区域$\tilde{R}$积分,应用Gauss定理,有
$$
\dfrac{\text{d}}{\text{d}t}\int_{\tilde{R}}\text{d}^3x j^0+\int_{\tilde{S}}\boldsymbol{j}\cdot \text{d}\boldsymbol{\sigma}=0,\tag{19}
$$
其中,$\text{d}\boldsymbol{\sigma}$是边界面$\tilde{S}$上的定向面元.引入**守恒荷**(conserved charge)$\displaystyle Q\equiv\int_{\tilde{R}}\text{d}^3xj^0$,上式改写为
$$\dfrac{\text{d}Q}{\text{d}t}=-\int_{\tilde{S}}\boldsymbol{j}\cdot \text{d}\boldsymbol{\sigma},\tag{20}$$
即<span style="color:red;">区域$\tilde{R}$中的守恒荷减少率(增加率)等于从边界面$\tilde{S}$出来(进入)的流.
</span>
$j^0$是守恒荷的空间密度.

对于三维空间,边界面$\tilde{S}$位于无穷远处,通常假设$\phi_a$在无穷远处消失,从而无穷远处$\boldsymbol{j}\to 0$,于是**全空间的守恒荷**
$$Q=\int \text{d}^3xj^0.\tag{21}$$


场论中,<span style="color:blue;">若系统具有某种连续对称性,则存在相应的守恒流(17),满足守恒流方程(18),而全空间的守恒荷(21)不随时间变化,对应着一条守恒定律.
</span>

- 时空平移对称性 
  - 保持线元平方$\text{d}s^2$不变的变换称为庞加莱变换或者非齐次洛伦兹变换.所有庞加莱变换组成的集合称为庞加莱群,它是闵氏时空的等距群,记作$\text{ISO}(1,3)$.时空坐标的庞加莱变换表示为
  $$
  x^{\prime\mu}=\Lambda^\mu{}_{\nu}x^\nu+a^\mu
  ,\tag{22}
  $$
  即任意庞加莱变换可以表示为洛伦兹变换和时空平移变换的组合.
  - 场的**能动张量**(energy-momentum tensor)为
  $$
  T^{\mu\nu}\equiv \dfrac{\partial \mathcal{L}}{\partial(\partial_\mu\phi_a)}\partial^\nu\phi_a-g^{\mu\nu}\mathcal{L},\tag{23}
  $$
满足$$
\partial_\mu T^{\mu\nu}=0.\tag{24}
$$
  - 时间平移对称性对应于能量守恒定律,空间平移对称性对应于动量守恒定律.

- 洛伦兹对称性
  
  - 空间旋转对称性对应于角动量守恒定律. 

- $U(1)$整体对称性

  - 一种$U(1)$整体对称性对应于一条荷数守恒定律.  

## 第2章 量子标量场


