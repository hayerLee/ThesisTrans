</style><script type="text/javascript" src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
<script>MathJax.Hub.Config({
  config: ["MMLorHTML.js"],
  extensions: ["tex2jax.js"],
  jax: ["input/TeX"],
  tex2jax: {
    inlineMath: [ ['$','$'], ["\\(","\\)"] ],
    displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
    processEscapes: false
  },
  TeX: {
    extensions: ["AMSmath.js", "AMSsymbols.js"],
    TagSide: "right",
    TagIndent: ".8em",
    MultLineWidth: "85%",
    equationNumbers: {
      autoNumber: "AMS",
    },
    unicode: {
      fonts: "STIXGeneral,'Arial Unicode MS'"
    }
  },
  showProcessingMessages: false
});
</script>

## Majorana费米子的?费曼规则

> 摘要：本文展示出一种适用Majorana粒子费曼规则的简单算法。通过在费米子线上穿过费曼图的费米子流，我们只需要熟悉的狄拉克传播函数和定点，而不需要显式的C变换矩阵。甚至，在狄拉克费米子的情况下我们会得到正确的____

超对称规范场论中包括Majorana费米子。Majorana场的自共轭性表明其不同于狄拉克场，存在场间Wick收缩现象。这和费米场的反对易性一同使作用的费曼图中的方向变得模糊。
Majrana费米子的费曼规则在（参考文献）中已经被给出，但是，这些费曼规则看上去不是不必要地复杂就是不允许

我们推导出了Majorana费米子的费曼规则，该规则和狄拉克粒子的费曼规则相近。因为费米子流中粒子数存在破缺，我们引入了一种连续的费米子流，例如每条费米子线的方向？基于这个费米子流我们得到狄拉克矩阵链，并且得以决定相关联的费曼图之间的关联符号。这里我们仅需众所周知的适用于一切费米子的传播函数，而对于每个顶点总体而言需要引入两个解析的表述，这依旧少于通常的处理方法所需。

具体而言，考虑典型的连结$\mathcal{L}_I = \overline{\chi}\Gamma\chi$，其中$\chi$可以是狄拉克或Majorana费米子，而$\Gamma$表示一般的费米子相互作用，其中包括狄拉克矩阵、互作用常数$h^i_{abc}$和玻色子场：
$$\overline{\chi}\Gamma\chi = h^i_{abc}\overline{\chi}_a\Gamma_i\chi_b\Phi_c$$
其中$\Phi$表示标量和矢量场的叠加，$\Gamma_i = 1,i\gamma_5,\gamma_\mu\gamma_5,\gamma_\mu,\sigma_{\mu\nu}$.

为了能够在费米子线段上跟随这条引入的费米子流，有必要将$\mathcal{L}_I$重写为等效的反转形式：
$$\mathcal{L}_I = \overline{\tilde{\chi}}\Gamma'\tilde{\chi}$$
其中电荷共轭场：
$$\tilde{\chi}=C\overline{\chi}^T,\overline{\tilde{\chi}}=-\chi^TC^{\dagger}$$
以及

$\Gamma' = C\Gamma^TC^\dagger$

利用电荷共轭矩阵$C$的性质（其中i不予求和）：

$C^\dagger=C^{-1},\quad C^T=-C,\quad C\Gamma^T_iC^{-1}=\eta_i\Gamma_i$

以及

$\eta_i = \begin{cases} 1\quad \Gamma_i=1,i\gamma_5,\gamma_\mu\gamma_5\\-1\quad\Gamma_i=\gamma_\mu,\sigma_{\mu\nu}\end{cases}$

得到：

$$\overline{\tilde{\chi}}\Gamma'\tilde{\chi}=h^i_{abc}\eta_i\overline{\tilde{\chi}}_b\Gamma_i\tilde{\chi}_a\Phi_c$$

方程 (7) 表明，在两个$\chi$都是Majorana费米子的情况下，对于所有指数$i$有$\eta_ih^i_{abc}=h^i_{abc}$，类似结论包括$\Gamma=\Gamma'$.

对于旋量，有

$v(p,s)=C\overline{u}^T(p,s)$

其中$p$和$s$分别表示动量和极化，对于传播函数$S(p)$

$CS(p)C^{-1}=S(-p)$

参考文献 [5] 中包括其详细的表达式，更完整的例子以及与参考文献 [1, 2, 3, 4] 的对比，其中我们也会表明我们的费曼规则对于含有明确的电荷共轭费米子场的理论有着天生的适用。

由此，费曼规则可以写出：

费米子用实线标示。对于狄拉克费米子来说，每条线都带有一个箭头以标示费米子数目流，Majorana粒子线没有箭头。

费米子顶点仍旧可以从拉格朗日量中读出，但对每个含有费米子的顶点需要两个表达式，直接的$\Gamma$和反转$\Gamma'$. 纯Majorana粒子顶点由于$\Gamma = \Gamma'$只需一个表达式。

与狄拉克费米子数流对应，正常的传播函数$S(p)$和反转传播函数$S'(-p)=S(-p)$以及旋转子和其对应的反向算符也是存在的。对于Majorana费米子而言只存在通常的传播函数、旋转子，而没有反转的对应项。其费米子流中的反转项和通常项相同，故只有通常项。

根据这些规则，费曼幅可按如下方法取得：

1. 画出给定过程中的所有费曼图；
2. 对每条费米子链，修正其方向；
3. 从一条外部的连线开始，写下其与选定的方向相反的狄拉克矩阵；
4. 对于每项内部的传播函数，外部的连线和顶点，如图1，2，3在其中加入合适的对应费米子流的解析表达式。显然，如果其方向和费米子数流相反，则需使用反转矩阵$\Gamma'$、传播子$S(-p)$和对应的旋转子；
5. 每个闭合的环乘上因子-1；
6. 对获取的解析表达式，乘上其旋转子的宇称；
7. 就结合因素的作用项而言，Majorana费米子的表征和实标量或矢量场相同。

注意上面的分析性表述和选定的起源之间不相互依赖。

在这里我们通过给出案例的方式演示我们的费曼规则的使用方法：考虑其在$\psi\psi\to\Phi\Phi$通过图4中Majorana交换中的贡献，该变换给出拉格朗日量$\mathcal{L}_I=h^i_{abc}\overline{\lambda_a}\Gamma_i\psi_b\Phi_c$，其中$\lambda_a$和$\psi_b$分别表示Majorana和狄拉克费米子。

得力于我们的费曼规则，随机费米子流幅值的表达式可以立刻写出。对于图4b中的始源，得到：

$$i\mathcal{M}=-i\overline{v}_a\Gamma'_iS(p_c-p_a)\Gamma_ju_bh^i_{eac}h^j_{ebd}$$

$$i\mathcal{M}'=(-1)(-i)\overline{v}_b\Gamma'_jS(p_a-p_c)\Gamma_iu_ah^i_{eac}h^j_{ebd}=i\mathcal{M}$$

其正负符号由旋转子的排列宇称按顺序给出，其参考顺序在10b中会为其加上参数$(-1)$. 上述两式的等效关系可轻易看出。

如上的费曼规则对任意阶的激发理论适用，注意由两个Majorana费米子组成的自能量环对于特殊的粒子有$\frac{1}{2}$的结合常数。

总而言之，我们给出的基于完整定义的费米子流的费米子流的费曼规则是简单而算术可行的。该规则和通常用于狄拉克费米子的规则形似，其中不显含电荷变换矩阵。符号的不确定由此消失，相作用的费曼图被明确定义，正如狄拉克费米子中的情况。这套规则使得可行的计算可以进行，可被轻易地转化为符号运算中费曼图生成子。