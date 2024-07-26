---
layout: page
permalink: /blogs/dd/index.html
title: dd
---

## 刘川《电动力学》知识梳理

---
1. **经典电动力学基础**
- 真空中的麦克斯韦方程组
$$
\begin{align}
&\nabla \cdot \boldsymbol{E}=\dfrac{\rho}{\varepsilon_0}\\
&\nabla \times \boldsymbol{B}=\varepsilon_0\mu_0\dfrac{\partial \boldsymbol{E}}{\partial t}+\mu_0\boldsymbol{J}\\
&\nabla \times \boldsymbol{E}=-\dfrac{\partial \boldsymbol{B}}{\partial t}\\
&\nabla \cdot \boldsymbol{B}=0
\end{align}
$$
其中,(1)反映了高斯定律,它源自于库仑定律;(2)是安培环路定律加上麦克斯韦的位移电流假设,称为安培-麦克斯韦定律;(3)是法拉第电磁感应定律;(4)是磁的高斯定律.
  - 线性,意味着经典电磁场满足线性叠加原理
  - 洛伦兹协变性(**连续对称性**),体现了电磁场在时空变换下的性质:麦克斯韦方程组在不同惯性参考系之间的洛伦兹变换下保持形式不变
  - 规范对称性(**连续对称性**)
    存在两套(实际上是无数套)不同的电磁势$(\Phi,\boldsymbol{A})$和$(\Phi^\prime,\boldsymbol{A'})$对应于相同的电磁场$\boldsymbol{E},\boldsymbol{B}$.这两套电磁势是相互关联的.若任意选取一个标量场$\Lambda$,则只需要使得$$\boldsymbol{A'}=\boldsymbol{A}+\nabla \Lambda,\Phi^\prime=\Phi-\dfrac{\partial \Lambda}{\partial t}$$  
电磁场具有的这种对称性(不变性)称为规范对称性.上式描写的两套等价的电磁势之间的变换称为规范变换.规范变换表明,电磁势具有一定的不确定性,在经典范畴内并不是可以直接测量的物理量.必须给定相应的规范条件.
   - 洛伦茨规范(协变规范):$\nabla \cdot \boldsymbol{A}+\dfrac{1}{c^2}\dfrac{\partial \Phi}{\partial t}=0$.
   - 库伦规范(辐射规范、横规范)$\nabla \cdot \boldsymbol{A}=0$.
 在洛伦茨规范下,真空麦克斯韦方程组可以化为相互独立的标势和矢势的波动方程,预示着电磁势从而电磁场具有波动形式的解:$$
\nabla^2\phi-\dfrac{1}{c^2}\dfrac{\partial^2\phi}{\partial t^2}=-\dfrac{\rho}{\varepsilon_0},\nabla^2\boldsymbol{A}=-\dfrac{1}{c^2}\dfrac{\partial^2\boldsymbol{A}}{\partial t^2}=-\mu_0\boldsymbol{J}$$ 
- 空间反射与时间反演(**分立对称性**) 
     **空间反射变换**(宇称变换)就是将所有的空间坐标都改变一个符号,即$x\to -x$.该变换下电荷密度不变,电流密度改变一个符号.真空中麦克斯韦方程组形式在如下的空间反射变换下不变:$$\boldsymbol{E}\to \boldsymbol{-E},\boldsymbol{B}\to \boldsymbol{B}$$
    - 极矢量:具有电场或者坐标这样变换性质(即在空间反射下变号)的三维矢量;
    - 轴矢量:像磁场这类在空间反射下不变的矢量.
     
     **时间反演变换**相当于将时间反号,即$t \to -t$的变换.该变换下电流密度会变号.要保证麦克斯韦方程组在该变换下不变,相应的电磁场应当在时间反演时满足$$\boldsymbol{E}\to \boldsymbol{E},\boldsymbol{B}\to -\boldsymbol{B}$$ 
- 洛伦兹力
若带电粒子处于外加电磁场$(\boldsymbol{E},\boldsymbol{B})$之中,会受到电磁场对它的电磁相互作用,作用力大小由于洛伦兹力公式给出.假设空间存在电荷密度和电流密度分布$(\rho,\boldsymbol{J})$,则这些电荷以及电流分布在单位体积感受的力(力密度)为$\boldsymbol{f}=\rho \boldsymbol{E}+\boldsymbol{J}\times \boldsymbol{B}$.
2. 即两种介质的交界面处磁感应强度的法向分量连续,电位移矢量的法向分量存在跃变.介质中的麦克斯韦方程组
$$
\begin{aligned}
&\nabla \cdot \boldsymbol{D}=\rho\\
&\nabla \times \boldsymbol{H}=\dfrac{\partial \boldsymbol{D}}{\partial t}+\boldsymbol{J}\\
&\nabla \times \boldsymbol{E}=-\dfrac{\partial \boldsymbol{B}}{\partial t}\\
&\nabla \cdot \boldsymbol{B}=0
\end{aligned}
$$

其中,$\boldsymbol{D}=\varepsilon_0\boldsymbol{E}+\boldsymbol{P},\boldsymbol{H}=\dfrac{1}{\mu_0}\boldsymbol{B}-\boldsymbol{M}$.$\boldsymbol{P}$是电极化强度,是介质单位体积中平均电偶极矩,$\boldsymbol{M}$是介质的极化强度,是介质单位体积中的平均磁偶极矩.
3. **介质交界面处的边界条件** 
设$\sigma$是两个交界面处的自由电荷面密度,$\boldsymbol{n}$是由介质1指向2的单位矢量,$\boldsymbol{K}$是交界面处的自由面电流密度.则两个电介质交界面的边界条件为 
- $\boldsymbol{n}\cdot(\boldsymbol{D}_2-\boldsymbol{D}_1)=\sigma$
- $\boldsymbol{n}\cdot(\boldsymbol{B}_2-\boldsymbol{B}_1)=0$
  即两种介质的交界面处磁感应强度的法向分量连续,电位移矢量的法向分量存在跃变.
-  $\boldsymbol{n}\times(\boldsymbol{E}_2-\boldsymbol{E}_1)=0$
-  $\boldsymbol{n}\times(\boldsymbol{H}_2-\boldsymbol{H}_1)=\boldsymbol{K}$
即两种介质的交界面处电场强度的切向分量连续,磁场强度的切向分量存在跃变.  
4. **电磁规律中的守恒律**
- 电荷守恒定律为$\dfrac{\partial\rho}{\partial t}+\nabla \cdot \boldsymbol{J}=0$
- 电磁场能量守恒:考虑在电磁场$(\boldsymbol{E},\boldsymbol{B})$中的一个电荷为$q$,速度为$\boldsymbol{v}$的运动的带电粒子.定义电磁场能量密度为$u=\dfrac{1}{2}(\boldsymbol{E}\cdot \boldsymbol{D}+\boldsymbol{B}\cdot \boldsymbol{H})$,能流密度或者坡印亭矢量$\boldsymbol{S}=\boldsymbol{E}\times \boldsymbol{H}$,则对于非耗散的线性介质,电流密度对电磁场做功的功率为$$\int_Vd^3\boldsymbol{x}\left(\dfrac{\partial u}{\partial t}+\nabla \cdot \boldsymbol{S}\right)=-\int_V d^3\boldsymbol{x}\boldsymbol{J}\cdot \boldsymbol{E}$$ 
即单位时间内任意一个体积$V$内的带电粒子能量的下降,一部分转换为电磁场能量的上升,另一部分由电磁场能流通过体积的边界流出.
- 电磁场动量守恒:考虑任意选定的空间区域$V$,该区域内的带电粒子(源)的总动量为$\boldsymbol{P}^{src}$,区域内电磁场的总动量为$$\boldsymbol{P}^{(field)}=\int_Vd^3\boldsymbol{xg}$$其中电磁场的动量密度(单位体积内电磁场的动量)定义为$$\boldsymbol{g}=\varepsilon_0(\boldsymbol{E}\times \boldsymbol{B})=\varepsilon_0\mu_0\boldsymbol{S}$$
定义电磁场的应力张量,即麦克斯韦应力张量为
$$T_{ij}=\varepsilon_0\left[E_iE_j+c^2B_iB_j-\dfrac{1}{2}(\boldsymbol{E}\cdot\boldsymbol{E}+c^2\boldsymbol{B}\cdot \boldsymbol{B})\delta_{ij}\right]$$ 
则有
$$\dfrac{d}{dt}\left[ P_i^{(src)}+P_i^{(field)}\right]=\int_V d^3\boldsymbol{x} \partial_i T_{ij}=\oint _{\partial V}d S_iT_{ij}$$
利用高斯定理,上式右边可以化为麦克斯韦应力张量在边界面上的积分,则上式的物理意义为
在单位时间中任意区域内的带电粒子(源)动量的下降,等于该区域内电磁场能量的上升,加上通过该区域边界$\partial V$净流出去的场对外界作用的动量变化率,而场对外界作用的动量变化率等于麦克斯韦应力张量在边界面上面积分的负值.
- 电磁场角动量守恒:若空间同时存在电磁场,那么空间任意一点就存在电磁场的动量密度$\boldsymbol{g}=\dfrac{(\boldsymbol{E}\times \boldsymbol{H})}{c^2}$,则相对原点来说电磁场就具有叫动量密度$$\boldsymbol{M}=\boldsymbol{x}\times \boldsymbol{g}=\boldsymbol{x}\times \dfrac{(\boldsymbol{E}\times\boldsymbol{H})}{{c^2}} $$
将之对空间积分,即可得到某区域中的电磁场携带的角动量.
---
5. 静电势$\Phi$满足的泊松方程:$\nabla^2 \Phi(\boldsymbol{x})=-\dfrac{\rho(\boldsymbol{x})}{\varepsilon} $,$\rho(\boldsymbol{x})=0$时满足拉普拉斯方程.

静电势在边界$S$上满足的边界条件有:
- **Dirichlet边界条件**:已知静电势本身在边界$S$上的取值
- **Neumann边界条件**:已知静电势在边界$S$上法向偏微商的取值
在这两类边界条件下,静电边值问题的解是唯一的.具体而言,唯一性定理可以表述为:
设空间某个区域$V$的边界为$S$,那么在该区域内满足泊松方程且在边界$S$上满足狄利克雷或者诺伊曼边界条件的解$\Phi(\boldsymbol{x})$是唯一的.
6.静电学中
- 导体内部的电场强度恒等于0;
- 导体表面是一个等电势面;
- 导体上所有的自由电荷只可能分布在导体的表面.实际上导体就是用来实现狄利克雷边界条件的物体.  
- 静电势在导体表面的法向偏微商是与该处自由电荷面密度联系在一起的:$$\varepsilon\dfrac{\partial \Phi}{\partial n}=-\sigma$$
其中假设导体外部是介电常数为$\varepsilon$的各向同性、均匀线性电介质.方向定义为从导体的内部指向外部.
7. **镜像法的思想**
   试图用用一个或者多个点电荷(称之为镜像电荷)来替代所有导体球表面产生的面电荷分布效应.如此,导体球外空间的静电势就是原先点电荷与镜像电荷产生的静电势的简单叠加.由于点电荷叠加出来的静电势自动满足拉普拉斯方程,镜像电荷的带电量以及位置只需要使得叠加后的静电势满足边界条件,即在导体球表面为0.
8. **求解拉普拉斯方程$\nabla^2\Phi=0$的分离变量法**
  - 直角坐标系中:设$\Phi(\boldsymbol{x})=X(x)Y(y)Z(z)$,其中$$X(x)\propto e^{k_1x},Y(y)\propto e^{k_2y},Z(z)\propto e^{k_3z},k_1^2+k_2^2+k_3^2=0$$
  若某个方向的边界条件是在一个有限区间内,该方向相应的$k_i$往往取分立的纯虚数值(形成驻波);如果某个方向的边界条件是在无穷区间上,相应的$k_i^2$取连续的值. 
  - 柱坐标系中:设$\Phi(\boldsymbol{x})=Z(z)\Phi(\phi)R(r)$,其中$r=\sqrt{x^2+y^2}$表示空间任意一点到$z$轴的距离.方程解为$$Z(z)\propto e^{\pm kz},\Phi(\phi)\propto e^{\pm im\phi},R(r)\propto J_m(kr),N_m(kr)$$
  为确保静电势的单值性,参数$m$必须为整数,参数$k$有如下两种选择:
    - $k$为实数.此时静电势在$z$方向为指数函数.径向函数$R(r)$就是标准的Bessel函数(振荡柱面波解)$J_m(kr)$和$N_m(kr)$的组合.
    - $k$为纯虚数.静电势在$z$方向为振荡的三角函数(由于该方向有限区间所加的边界条件引起的).径向函数为虚宗量贝塞尔函数(指数型)$I_m(|k|r)$和$K_m(|k|r)$.
  - 球坐标系中,拉普拉斯方程的一般解可以写为:
  $$\Phi(r,\boldsymbol{n})=\sum\limits_{l=0}^\infty\sum\limits_{m=-l}^l\left(A_{lm}r^l+\dfrac{B_{lm}}{r^{l+1}}\right)Y_{lm}(\boldsymbol{n})$$
一个典型的例子就是均匀场中的介质球,静电势在球内对应于一个均匀电场,在球外对应于原先存在的均匀外电场与极化的电偶极矩产生的电偶极场的叠加.
---
9. **静磁学与静电学的区别**
    自然界中没有单一的磁荷,静磁场不会是由作为基本粒子的点磁荷(磁单极)产生的,产生磁场的可以是运动电荷(电流),或者是自发磁化的铁磁体中的等效磁荷(本质是电子自旋).磁力线一定是闭合的曲线,磁感应强度一定是一个无源场.
10. 电流分布$\boldsymbol{J}$对应的磁偶极矩(简称磁矩)定义为$$
\boldsymbol{m}=\dfrac{1}{2}\int d^3 \boldsymbol{x'}[\boldsymbol{x'}\times \boldsymbol{J(x')}]=IS\boldsymbol{n}_0$$
后面的等号仅仅在电流分布是位于一个平面内的电流圈(不一定是环形)时成立,$S,I$分别是该平面内电流圈所包围的面积和电流强度,$\boldsymbol{n}_0$是沿着右手法则所确定的平面电流圈的法向单位矢量.
11. **电流在外场中的能量**
一个外场中的磁偶极子的势能表达为:$U=-\boldsymbol{m}\cdot \boldsymbol{B}$.
塞曼效应:电子的磁矩与外加磁场相互作用引起的.由于量子力学中电子的磁矩与它的角动量成正比,而后者是量子化的.当原子处于外磁场中时由于转动不变性而简并的能级会发生劈裂.
12. **磁标势**
    若研究的空间区域中没有自由电流分布,则磁场强度$\boldsymbol{H}$为一个无旋矢量场,可以引入磁标势$\Phi_M(\boldsymbol{x})$,满足$$\boldsymbol{H}(x)=-\nabla \Phi_M(\boldsymbol{x})\Rightarrow \nabla^2 \Phi_M(\boldsymbol{x})=-(-\nabla \cdot \boldsymbol{M})$$
  ---
  13. **电磁波的波动方程**
  在没有电荷与电流分布的介质中,电场强度和磁感应强度满足同样的波动方程:
  $$\nabla^2\boldsymbol{E}-\varepsilon\mu\dfrac{\partial^2 \boldsymbol{E}}{\partial t^2}=0,\nabla^2\boldsymbol{B}-\varepsilon\mu\dfrac{\partial^2 \boldsymbol{B}}{\partial t^2}=0$$
  基本解为均匀平面电磁波:$$\boldsymbol{E}=\boldsymbol{E}_0e^{i\boldsymbol{k\cdot x}-i\omega t},\boldsymbol{B}=\boldsymbol{B}_0e^{i\boldsymbol{k\cdot x}-i\omega t}$$
  均匀平面电磁波的波矢、电场强度和磁感应强度构成相互垂直的一个坐标架.
  平面波在介质中传播的速度——相速度或者说平面波中相位保持相同的点在空间移动的速度为$$v=\dfrac{\omega}{k}=\dfrac{1}{\sqrt{\mu \varepsilon}}=\dfrac{c}{n},n=\sqrt{\dfrac{\mu \varepsilon}{\mu_0\varepsilon_0}}$$
  其中$n$为介质的折射率.
  设波矢量为$\boldsymbol{k}=k\boldsymbol{e_3}$,另外两个在垂直于$\boldsymbol{k}$的平面内的单位矢量为$\boldsymbol{e_1},\boldsymbol{e_2}$,满足$\boldsymbol{e_1}\times \boldsymbol{e_2}=\boldsymbol{e_3}$.电场强度的复振幅可以用$\boldsymbol{e_1},\boldsymbol{e_2}$展开:
  $$\boldsymbol{E}(\boldsymbol{x},t)=(E_1\boldsymbol{e_1}+E_2\boldsymbol{e_2})e^{i\boldsymbol{k\cdot x}-i\omega t}$$
  $E_1,E_2$决定了电磁波的不同偏振状态:
  - $E_1,E_2$的复相角相同,则称为线偏振
  - $\dfrac{E_2}{E_1}=i$,称为左旋或者右旋偏振
  - 一般情况,称为椭圆偏振.
**能流**:坡印亭矢量的时间平均值代表了在一个周期中平均通过的能流:
$$\boldsymbol{S}=\dfrac{1}{2}\boldsymbol{E}\times \boldsymbol{H^*}=\dfrac{1}{2}\sqrt{\dfrac{\varepsilon}{\mu}}|\boldsymbol{E_0}|^2\boldsymbol{n}$$
即电磁波传播的时间平均的效果是有静能流沿着波矢$\boldsymbol{k}$的方向传播.
14. **电磁波在介质表面的折射与反射**
    考虑两种均匀、各向同性的线性介质,介电常数和磁导率分别是$\varepsilon,\mu$和$\varepsilon',\mu'$,分别填充于$z<0,z>0$的空间.
    **Snell定律**:设$i,r$分别表示入射角与折射角,则有
    $$\dfrac{\sin i}{\sin r}=\dfrac{k'}{k}=\dfrac{n'}{n}$$
    **布儒斯特角**:非磁性材料中,布儒斯特角满足$$i_B=\arctan \left(\dfrac{n'}{n}\right) $$对于反射波的振幅来说,如果入射波的入射角正好等于布儒斯特角时,反射波的电场平行分量为0,从而反射波的偏振方向就会完全垂直于入射面.即使入射角不正好等于布儒斯特角,在反射波中的电场平行于入射面的分量也会被较大幅度地减小.(自然光经过反射后往往具有较高偏振度.)
    **全反射**:电磁波从较大折射率的介质(光密介质)入射到较小折射率的介质(光疏介质)表面时($n>n'$),折射角$r=90\degree$,折射波沿着交界面传播的现象.此时的入射角$i_0$满足$$i_0=\arcsin\left(\dfrac{n'}{n}\right)$$
    若入射角继续增大,则折射角的余弦将会变成纯虚数,折射波的相因子会出现沿着$z$方向指数衰减的因子,折射波在该方向上指数衰减.
  15. **电磁波在导电介质中的传播**
    假设研究的导电介质均匀、各向同性,满足欧姆定律$\boldsymbol{J}=\sigma\boldsymbol{E}$.对电磁波而言,导电介质与非导电介质的区别就是电磁波在导电介质中会引起自由电流从而出现耗散,电磁能量会转换为导电介质中的焦耳热.
    定义复介电常数:$\varepsilon(\omega)=\varepsilon_b(\omega)+i\dfrac{\sigma(\omega)}{\omega}$,若场具有平面波的形式,则波矢平方满足
    $$k^2=\mu\varepsilon(\omega)\omega^2=\mu\varepsilon_b\omega^2\left(1+i\dfrac{\sigma}{\omega\varepsilon_b}\right)\xlongequal{\text{良导体，}\dfrac{\sigma}{\omega\varepsilon_b}\gg1}(1+i)\sqrt{\dfrac{\omega\mu\sigma}{2}}=\dfrac{1+i}{\delta}$$
    其中$\delta=\sqrt{\dfrac{2}{\omega\mu\sigma}}$为导体中的趋肤深度,代表了电磁波能够进入导体内的一个特征长度.它明显依赖于电磁波的频率.频率越高的电磁波越不容易穿透良导体.
  - 初始时刻导体中存在某个真实电磁场分布,这时频率$\omega$必为复数,频率的虚部代表了导体中电磁场是随着时间指数衰减的.由于存在欧姆损耗,初始时刻存在的电磁场以及与之相对应的能量随时间不断转换为焦耳热,导致导体中的电磁场振幅随时间指数衰减.
  - 外界有电磁波入射到导体的情形,此时导体内的场是由于外界能量注入的受迫振动,其时间依赖是不衰减的简谐振荡,即$\omega$为实数.此时电磁波的波矢$k$必须为复数.尽管能量仍然会转化为焦耳热,但由于外面入射的电磁波源源不断带来能量,所以导体内任意一点电磁场随着时间仍然可以维持不衰减的简谐振荡.
  - 对良导体而言,磁场与电场的相位差几乎为$\frac{\pi}{4}$.
  - **导体的准静态近似**:导体中的传导电流远大于位移电流的贡献,可以完全忽略位移电流.
16. **介质色散的经典模型**
  Drude模型:$\sigma(\omega)=\dfrac{f_0Ne^2}{m(\gamma_0-i\omega)}$
  其中$f_0$为具有频率$\omega_0$的电子的振子强度,$e,m$分别是电子的电荷与质量,$\gamma_0$为阻尼系数.
 - 低频极限:略去分母中的虚部,电导$\sigma(\omega)$基本上为实的.
 - 高频极限下有$$\dfrac{\varepsilon(\omega)}{\varepsilon_0}\approx 1-\dfrac{\omega^2_p}{\omega^2},\omega_p^2=\dfrac{NZe^2}{\varepsilon_0m}$$ 
   - 地球上频率不太高的电磁波信号可以经过电离层反射而传递很远,但高频电磁波是可以穿透电离层的.
   - 普通金属的等离子体频率处于紫外到X射线波段,虽然多数金属对于可见光是不透明的,但对于紫外线会逐步变为透明的. 
   - 水对于电磁波的吸收系数在多数频率范围内一直很大,仅仅在一个非常狭小的频率窗口之内,水的吸收系数陡然变小,这个窗口对应的光波长恰为可见光波段。亦即,当且仅当电磁波波长在可见光波段时,水才是透明的.
17. **波导与谐振腔**
假定在波导管中电磁波沿着该波导管的平移对称轴(取为$z$轴)在介质中传播.
- 若电场的纵向分量恒为零,即$E_z=0$,这种波导管中传播的电磁波称为横电波,或者TE波、横电模式、TE模式.
- 如果磁场的纵向分量恒为零,这种波称为横磁波、TM波、横磁模式、TM模式.
- 若电场和磁场的纵向分量都为零,这种模式就称为恒电磁波或者TEM波、横电磁模式、TEM模式.
横电磁模式的波的波数与频率之间的关系和无边界空间中平面波的波数与频率之间的关系完全相同,即$$k_{TEM}^2=\mu \varepsilon\omega^2\Rightarrow k_{TEM}=k_0=\sqrt{\mu \varepsilon}\omega$$ 
横电磁模式的横向波矢$k_\perp=0$,电磁波的相速度与无边界空间中传播的平面波完全相同,等于该介质中的光速.
  
对于金属波导,横电模式和横磁模式是完全分离的,互相没有干扰,它们各自由自己的边界条件所完全确定. 对于一般的横电或者横磁模式,波导管中的电磁波的相速度总是大于无边界空间光速.这并不与狭义相对论矛盾,因为金属波导中能量的平均传输速度应当用群速度而不是相速度描写.

---
18. **电磁波的辐射**
    经典电动力学中的电磁波的辐射都可以归因为带电粒子变速运动导致的辐射,从具体机制出发分为两类:
    - 由宏观天线中电流的周期振荡产生的
    - 由微观带电粒子做变速运动产生的.这类辐射大量出现在快速粒子穿过物质时或者人造的各种加速器中.
通常将电磁波绕过障碍物传播的现象称为衍射,而如果障碍物受到电磁波影响然后自身发射电磁波则称为散射.
- 电偶极辐射的辐射功率与辐射频率的4次方成正比,其角分布与观测点处的位置矢量与电偶极矩夹角的正弦的平方成正比.
- 电四级辐射的辐射功率与辐射频率的6次方成正比.
19. **电磁波的散射**
    如果散射体的尺度远大于电磁波的波长,散射体对电磁波的影响基本上可以利用几何光学近似处理.若散射体的尺度远小于电磁波的波长或者与之相当,那么电磁波的波动性就会十分显著. 
- 散射截面:如果入射波的方向是$\boldsymbol{n_0}$,其偏振方向为给定的$\boldsymbol{e_0}$的入射能流密度为
 $S_0=\dfrac{|\boldsymbol{e_0}^*\cdot\boldsymbol{E}_{inc}|^2}{2Z_0}$,那么单位入射能流产生的散射波在方向$\boldsymbol{n}$的立体角$d\Omega_n$中且具有指定偏振方向$\boldsymbol{e}$的辐射波功率称为相应散射体的微分散射截面:
 $$\dfrac{d\sigma}{d\Omega}(\boldsymbol{n},\boldsymbol{e};\boldsymbol{n_0},\boldsymbol{e_0})=\left.\dfrac{r^2 \dfrac{1}{2Z_0}|\boldsymbol{e}^*\cdot\boldsymbol{E}_{sc}|^2}{\dfrac{1}{2Z_0}|\boldsymbol{e_0}^*\cdot\boldsymbol{E}_{inc}|^2}\right|_{r\to \infty}$$
散射微分截面具有面积的量纲.在空间某个方向以及某个特定偏振的微分散射截面的大小体现了散射体将入射电磁波散射到该指定方向角和偏振的概率大小.
- 长波散射和偶极散射的特性:微分散射截面正比于频率的4次方,同时散射波的偏振方向具有完全确定的特性.
- 对于可见光波段来说电磁波的波长远大于气体分子的尺度,因此长波偶极辐射理论可以很好解释阳光的散射问题.偶极散射截面公式表明,频率较高的光将比较多的被散射掉,这就是为什么白天看到的晴天呈现蓝色.
20. **狭义相对论的基本假设及其验证**
  - 惯性系:如果一个不受外力的经典物体在该参照系中满足牛顿第一定律,即保持匀速直线运动,那么就称这个参照系为惯性参考系.如果一个参照系是惯性参照系,那么相对于该惯性系做匀速直线运动的参照系也是一个惯性系.
  - 狭义相对论的基本假设:
    - 相对性原理:所有的惯性系在物理上都是等价的.
    - 光速不变原理:所有惯性系中信号的最大可能传播速度是真空中的光速$c$. 
  - 迈克耳孙-莫雷实验:利用光的干涉条纹的移动试图测量地球相对于一个绝对静止惯性系-以太的速度.实验结果是在精度之内没有测到任何地球相对于以太的速度,若以太真实存在则任何时刻地球在其中都是静止的.
21. **洛伦兹变换**
  构造两个时空点之间的不变间隔的平方$$\Delta s^2\equiv c^2(t_2-t_1)^2-(\boldsymbol{x_2}-\boldsymbol{x_1})^2=c^2\Delta t^2-\Delta \boldsymbol{x}^2=0$$ 
  对于光信号联系的事件,其不变间隔平方一定等于零.而不同惯性系坐标变换时,任意两个事件之间或者说四维时空中任意两个时空点之间的不变间隔平方不变.该四维时空称为闵可夫斯基时空,简称闵氏时空.
  - $\Delta s^2>0$,称两个时空点的间隔是类时的;
  - $\Delta s^2<0$,称两个时空点间隔是类空的;
  - $\Delta s^2=0$,称两个时空点间隔是类光的.
闵氏时空中任意一点可以按照它与原点之间的不变间隔$\Delta s$分为类空、类时和类光三种可能.所有类光的点在四维闵氏时空中构成所谓的光锥 
>*闵氏时空的光锥.光锥的分界面由所有与原点的不变间隔为类光的点构成.一个粒子在$t=0$时处于原点.它的时空轨迹称为世界线,一定穿过原点且完全位于类时区域.*

在不同惯性系之间维持其不变间隔不变的线性坐标变换统一称为洛伦兹变换,可以看成闵氏时空的一个“转动”:
- 只涉及空间坐标之间的转动:$x-y,x-z,y-z$平面内的转动,刻画$K'$系的三个坐标架相对于$K$系的三个坐标架之间的相对取向,由一个三维转动刻画.
- 涉及一个空间坐标与一个时间坐标之间的变换,称为“推促”:$x-t,y-t,z-t$,反映了$K'$系的原点在$K$系中的运动方向,由速度$\boldsymbol{v}$刻画.

若惯性系$K'$相对于惯性系$K$的速度为$\boldsymbol{v}$,那么空间坐标中与$\boldsymbol{v}$垂直的分量在变换下不变,而平行的分量应当与时间混合,具体的变换为:
$$ct'=\gamma(ct-\boldsymbol{\beta\cdot x}),\boldsymbol{x'}=\boldsymbol{x}+\dfrac{\gamma-1}{\boldsymbol{\beta}^2}(\boldsymbol{\beta}\cdot\boldsymbol{x})\boldsymbol{\beta}-\gamma\boldsymbol{\beta}ct.$$
洛伦兹变换将会导致长度收缩、时钟变慢等有违经验的结论.这些现象只是一种运动学的测量效应,构成尺子或者钟表的物质本身并未发生任何物理上的变化.
两个事件的不变间隔只有是类时的,才可能存在因果联系. 
1.  **洛伦兹标量与四矢量、洛伦兹变换的数学性质**
  - 洛伦兹标量:在任意洛伦兹变换下都不变的物理量,如闵氏时空中两个事件之间的不变间隔平方$\Delta s^2$以及闵氏时空中的四维体积元$d^4x$.
  - 洛伦兹四矢量:将闵氏时空中的时空坐标这样的物理量用一个四维空间的坐标矢量来标记:
  $$x^0=ct,x^1=x,x^2=y,x^3=z$$
  统一用逆变四矢量$x^\mu=(x^0,\boldsymbol{x})$标记.协变四矢量为空间部分反号的四矢量$x_\mu=(x^0,-\boldsymbol{x}).$
  引入闵氏空间的度规张量$\eta_{\mu \nu}$,满足$\eta_{\mu \beta}\eta^{\beta\nu}=\delta_{\nu}^{\mu}$,则闵氏空间中两个无限接近的点之间的不变间隔平方$ds^2$可以写为:
  $$ds^2=dx^\mu dx_\mu=\eta_{\mu \nu}dx^\mu dx^\nu=\eta^{\mu\nu}dx_\mu dx_\nu$$
  如果在任意洛伦兹变换$\Lambda^\mu{}_\nu$下,物理量$A^\mu$按照与四维坐标$x^\mu$相同的形式变换$$A^{'\mu}=\Lambda^\mu{}_\nu A^\nu$$称该物理量为逆变四矢量.利用度规张量降低指标,可以得到相应的协变四矢量$A_\mu$.将任意一个协变四矢量$A_\mu$与任意一个逆变四矢量$B^\mu$相乘并且缩并它们的指标,就得到一个洛伦兹标量,称为两个四矢量的内积:
  $$A\cdot B=A^\mu B_\mu=A_\mu B^\mu$$
  事实上,任意两个矢量的内积都是洛伦兹变换下的不变量.

  电磁波的波矢四矢量构成一个逆变四矢量:$$\phi=k\cdot x=k^\mu x_\mu,k^\mu=(\omega/c,\boldsymbol{k})$$
  电磁波的频率与波矢构成四矢量意味着$k^\mu$在洛伦兹变换下按照与时空坐标类似的变换.因此电磁波的频率在坐标变换下会发生变化,这个现象就是光的多普勒效应.

  定义一个四矢量梯度算符$\partial_\mu$,其作用于闵氏空间中的标量函数的规则为:
  $$\partial_\mu f(x)\equiv \dfrac{\partial f(x)}{\partial x^\mu}$$
显然它作用于一个标量场后产生一个协变四矢量.将具有协变指标和逆变指标的两个四维梯度缩并,会得到一个标量算符,称之为达朗贝尔算符:
$$-\square =\partial^\mu\partial_\mu=\dfrac{1}{c^2}\dfrac{\partial^2}{\partial t^2}-\nabla^2$$
闵氏空间中,各阶张量是唯一的在洛伦兹变换下具有确定变换性质的数学对象.因此如果一个物理理论要符合狭义相对论的要求,那么表述它的数学方程一定是用正确的张量形式写出的.只有这样该方程描述的物理规律才可能在不同参照系下普遍成立,而这一点恰恰是相对性原理的要求.如果一个方程满足上述条件,称这个方程在洛伦兹变换下是协变的.如果一个物理理论中的所有方程都是协变的,称这个物理理论是协变的,具有协变性.
所有的洛伦兹变换的集合在数学上构成一个称为洛伦兹群的结构.

---
23. **相对论性电动力学**