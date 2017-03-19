散射理论中常使用费曼图方法。费曼图方法对于中性和带电荷的自旋为0或1的玻色子以及带电荷的自旋二分之一的费米子很适用。而对于自旋为二分之一的中性费米子而言，这套方法尚未发展成熟。目前有关该问题的文章仅有三篇，而其中展示的方法过于复杂，且许多文章在描述Majorana中微子的相互作用时偏向于使用Wick定理。由于几种传播函数的区别、相关联费曼矩阵的多样和，不同费曼图对于同一幅度贡献的相对符号的问题，Majorana粒子的费曼规则与狄拉克费米子的费曼规则不同。这些差异和Majorana粒子的自共轭性有关。另一方面，Majorana中微子在很多被提出的标准模型的扩展中都有出现，因此提供对其适用的用于计算散射截面的简单费曼规则很为重要。参考文献3中所需的传播子数目以及费曼矩阵数已经被削减，但其费曼规则的应用依旧复杂。首先，该文作者通过格林函数中费米算子的阶给出了每个费曼图的确定的符号。参考文献1-3中使用了狄拉克$\gamma^\mu$矩阵与旋量的Majorana表述，因此难以分辨其简化是提出的方法抑或自旋表述的结果。

本文中会提出一种适用于Majorana中微子的费曼图方法，该方法与旋量的表述无关，而且不会对每一种费曼图提供一种规则。我们发现的是一种简单的方法，从而使得预料不同图间作用的符号可以预料，这在实际计算中至关重要。该方法非常简单，我们希望其能够在实际应用中得到利用。

下一章节会讨论Majorana中微子的相互作用，其中得到了费曼规则，章节3中会将该费曼规则展示出来。章节三的起始处会考虑一种简单的情况以说明即使旋转矩阵和传播子是多样的，明确的费曼规则依旧能够被写出。第四章节中会对我们的规则提供具体的例子。

## 2. Majorana中微子相互作用

在这里仅考虑规范场论中描述Majorana粒子-中微子相互作用的部分，其余部分的拉格朗日量对我们的需求来说不重要，且其费曼规则尽已世人皆知。这里以Majorana中微子$N$和带电荷的轻子$l$以及带电荷或不带电荷（$W^\pm$和$Z^0$）的规范玻色子的互作用为例，写成如下形式：

$L_{NW\pm}=\overline{N}\Gamma^\mu_l lW^+_\mu+\overline l\overline\Gamma^\mu_lNW^-_\mu$

$L_{NZ^0}=(\overline N\Gamma^\mu_N N+\overline l\Gamma^\mu_{lN}l)Z_\mu$

其中，

$\Gamma^\mu_{(x)}=\Gamma^\mu(P_LA_L^{(x)}+P_RA_R^{(x)}),\quad x=l,N,lN$

以及：

$\overline{\Gamma}^\mu_l\equiv\gamma_0\Gamma^{\mu\dagger}_l\gamma_0=\gamma^\mu(P_L{A^{(l)}_L}^*+P_R{A^{(l)}_R}^*)$

$P_{L(R)}=\frac{1}{2}(1\mp\gamma_5)$

参数$A^{(x)}_{L,R}$在$x=N,lN$的情况下为实数，而在$x=l$的时候一般为复数，取决于所考虑的理论。在不同代的粒子组合的情况下$A^{(x)}_{L,R}$是矩阵量，但这不会让我们的费曼规则变得复杂。

在一种类似的途径中，考虑Majorana中微子$N$与带电荷与不带电荷（$H^\pm$和$H^0$）的自旋为0希格斯粒子的相互作用：

$L_{NH^\pm}=\overline{N}\Gamma_llH^++\overline{l}\overline{\Gamma}_lNH^-$

$L_{NH^0}=(\overline{N}\Gamma_NN+\overline{l}\Gamma_{lN}l)H^0$

其中：

$\Gamma_{(x)}=P_LB_L^{(x)}+P_RB_R^{(x)}$		其中$x=l,N,lN$

$\overline{\Gamma}_l\equiv\gamma_0\Gamma^\dagger_l\gamma_0\equiv P_R{B_L^{(l)}}^*+P_L{B_R^{(l)}}^*$

以及：

$B_L^{(x)}={B_R^{(x)}}^*$	其中$x=N,lN$

如同之前的$A$，$B^{(x)}_{L(R)}$也是取决于具体理论的数或矩阵。Majorana场是自共轭场，有平面波展开形式：

$N_\alpha(x)=\sum\limits_{\lambda=\pm1/2}\int\frac{d^3k}{(2\pi)^32E}[u_\alpha(\vec{k},\lambda)a(\vec{k},\lambda)e^{-ikx}+u_\alpha(\vec{k},\lambda)a^\dagger(\vec{k},\lambda)e^{ikx}]$

$N^C_\alpha\equiv  CN_\alpha(x)C^{-1}=C_{\alpha\beta}[\overline{N}^T(x)]_\beta=N_\alpha(x)$

其中$C_{\alpha\beta}$是狄拉克空间中$4\times 4$电荷共轭矩阵

$C\gamma^\mu C^{-1}=-{\gamma^\mu}^T,\quad C^\dagger=C^{-1},\quad C^T=-C$

费曼矩阵可以用$\Gamma^\mu_{(x)}$或$\Gamma_{(x)}$矩阵和它们的电荷共轭来表示，

$\Gamma^\mu_{(x)C}\equiv C{\Gamma^\mu_{(x)}}^TC^{-1}=-\gamma^\mu(P_RA_L^{(x)}+P_LA_R^{(x)})$

及

$\Gamma_{(x)C}\equiv C\Gamma^T_{(x)}C^{-1}=\Gamma_{(x)}$

## 3. 费曼规则

我们会展示我们在(2.1)-(2.4)中展示的Majorana费米子的费曼规则。费曼图中狄拉克费米子用双重连续线表示，Majorana费米子用单重连续线表示，其余的粒子依旧用传统方式表示。

$<0|T[N_\alpha(x)\overline{N}_\beta(y)]|0>\equiv iS_{\alpha\beta}(x-y)=$

其中

$S(x-y)=i\int\frac{d^4 x}{(2\pi)^4}e^{-i(x-y)k}\frac{\hat{k}+m}{k^2-m^2+i\epsilon}$

描述在$y$处产生，在$x$湮灭的费米子，通过适用于Majorana粒子的关系$N^T=\overline{N}C^T$和$\overline{N}^T=C^{-1}N$，我们可以定义另外三种传播子：

$<0|T[N_\alpha(x)N_\beta(y)]|0>\equiv-i[S(x-y)C]_{\alpha\beta}=$

描述$x$和$y$点湮灭的Majorana中微子：

$<0|T[\overline{N}_\alpha(x)\overline{N}_\beta(y)]|0>\equiv i[C^{-1}S(x-y)]_{\alpha\beta}=$

其中的粒子在$x$和$y$点产生，最后

$<0|T[\overline{N}_\alpha(x)N_\beta(y)]|0>\equiv-i[C^{-1}S(x-y)C]_{\alpha\beta}=$

该规则描述