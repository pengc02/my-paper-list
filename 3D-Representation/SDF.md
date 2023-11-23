
参考这里学一下：
[Rendering (Signed) Distance Function - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/345227118)



图形学上的表示：
$$|f(x)|=\inf _{y \in \Omega}\|x-y\|, x \in \mathbb{R}^{\mathrm{n}}$$
点 x 在表面内部时取负，在外部时取正


Neus 中提出用SDF作为表达来进行3D重建


第一步：
构造从3D模型到图像的渲染方法 (吐槽: 在传统图形学大概可称为光栅化)。

定义两个函数:
* $f: \mathbb{R}^3 \rightarrow \mathbb{R}$ 空间中一点到表面的符号距离 (signed distance) 值;
* $c: \mathbb{R}^3 \times \mathbb{S}^2 \rightarrow \mathbb{R}^3$ 空间中一点到某个视角方向的颜色值   （为什么是到某一个视角？跟光照有关吗）

两个函数都通过MLP编码。待重构的表面则可以被表示为 $S D F$ 的零级集合: $\mathcal{S}=\left\{x \in \mathbb{R}^3 \mid f(x)=0\right\}$

第二步是构造体积渲染训练SDF网络，先定义概率密度函数 $\phi_{\mathcal{S}}(f(x))$ ，称为S密度。其中 $f(x)$是SDF，外层是logistic密度分布 : 
$$
\phi_s(x)=s e^{-s x} /\left(1+e^{-s x}\right)^2
$$










