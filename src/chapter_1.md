# 場の理論

# 第1章 自由場

## 1.1 はじめに

物理の理論は、実験の結果を実験する前に計算で出す方法を示すものである。  
ここで、次の2つが重要になると考えられる。

・その理論はなぜ正しいと言えるのか。  
・具体的にどのように計算するのか。

前者は、計算方法の解釈の問題にもなる。  
「理由が完全に明確であるわけではないが、こう計算すると答がでる。
そして、その計算結果が実験と一致する」ということがあるのである。  
実際のところ、「ということがある」というより、「ここにこそ、物理学の重大な問題がある」と
言うこともできるだろう。  

しかし、この文章は後者に焦点をあて、「なるべくはやく計算方法（の流れ）を知る」ためのものとしたい。  
そのため、教科書で初めに書いてあるようなことを省略することもある。
また、多くの物理学者が正しいと考えているであろう解釈を、なるべく論評抜きで述べることにする。
しかし、物理の理論は完成したものではないため、それが絶対に正しいとは言えない。
したがって、どの解釈も、語尾に「このように解釈される。と多くの物理学者が考えている。と著者は思っている。しかし、どこかのステップで間違っている可能性はある」が省略されていると考えてほしい。

はじめに「実験結果を出す計算方法」と書いたが、本当の実験の結果を出すまでの計算方法を示すことはできない。「理論上の実験」レベルの話である。具体的には、散乱振幅（後述）の基本的な計算方法を示すということになる。

なお、この文章は予告なく変更することがあります。

## 1.2 場の理論

素粒子は、4次元時空の中で生成し、また消滅する。  
これを説明するのが場の理論である。素粒子が生成消滅する性質をもった時空を「場」とよんでいるのである。  

ここで、これから必要になる特殊相対性理論の内容を簡単に見ておく。  
4次元時空の座標は \\((x^0, x^1, x^2, x^3)\\) のように4つの実数で表される。\\(x^0\\) が時間である。
エネルギーと運動量は、\\((E, p^1, p^2, p^3)\\) のようにまとめられて4次元運動量となる。したがって、\\(E\\) を \\(p^0\\) とも書く。  
4次元の座標も運動量も4成分だが、多くの場合、1文字にまとめて \\(x , p \\) のようにあらわす。
4次元の内積も3次元のときと同様に「\\(\cdot\\)」であらわす。たとえば、\\(x \cdot p\\) は 

　　\\(x^0p^0 - x^1p^1 - x^2p^2 - x^3p^3\\) = \\(x^0p^0 - \mathbf{x}\cdot\mathbf{p}\\)

のことである。ただし、太字は3次元のベクトルを表し、その内積は通常のものである。  
質量 \\(m\\) の独立した粒子では、\\(p \cdot p = E^2 - \mathbf{p}\cdot\mathbf{p} = m^2 \\) が成り立つ。これは 

　　\\(E = \sqrt{\mathbf{p}\cdot\mathbf{p} + m^2}\\)

ということである。

場の理論に戻ろう。  
点 \\(x\\) に粒子を生成する演算子 \\(\phi(x)\\) があって、物理現象は、\\(\phi(x)\\) が真空 \\(|0>\\) に作用することで起こると考える。
この \\(\phi(x)\\) が「場を表す演算子」=「場の演算子」である。（実際には、光子の場の演算子、クォークの場の演算子、、、など複数種類ある。）
もちろん、真空に場の演算子がすでに作用している状態にさらに他の場の演算子が作用することもある。

具体的には、「真空に作用する場の演算子」を定義し、それらの作用の結果を計算するのが、場の理論ということになる。場の演算子は、特定の素粒子を生成消滅させる場を表すということを再度注意しておく。したがって、しばしば「この素粒子は〇〇の性質をもつ」と「この場は〇〇の性質をもつ」は同じ意味で使われる。また、以下では、素粒子を単に粒子と書く。実際、素粒子でなくとも、場の理論は有効である。


## 1.3 粒子の種類

空間の原点に点があるとする。座標軸を原点を中心に回転させても、「原点に点がある」という事実は変わらないし、見た目も変わらないだろう。次に、原点に矢印がある場合を考える。矢印を動かさずに座標軸を回転させると、「原点に矢印がある」という事実は変わらないが、矢印の座標軸から見た向きは変わってしまう。

場の理論で考える粒子は大きさを持たないという意味で点である。しかし、このような回転（やその拡張としてのローレンツ変換）に対して、見え方が変わるかもしれない。そこで、ただの点のように変化しない粒子をスカラー粒子、矢印のように見た目が変わるものをベクトル粒子などという。  
このような粒子の分類には、「ローレンツ群の表現」という数学的な道具が使える。それによれば、粒子はスピンという数で分類できる。たとえば、スカラー粒子はスピン0、ベクトル粒子をスピン1である。素粒子の世界では、ヒグス粒子がスカラーで、光子（光の粒子）がベクトルである。また、通常の場の理論では扱えないが重力の粒子はスピン2と考えられている。

実は、スピンが1/2などという半整数の粒子もある。実際、クォークやニュートリノはスピン1/2の粒子である。スピン3/2の「素」粒子はまだ見つかっていない。

スピンが整数の粒子をボソン、スピンが半整数の粒子をフェルミオンという。


## 1.4 自由スカラー場

粒子はなんらかの相互作用をしているはずだが、最初は相互作用を一切しない粒子を考え、それを自由粒子、自由場の粒子、自由場などとよぶ。相互作用は、自由場からの「わずかなずれ」と考えるのである。  

ここでは、自由スカラー場の説明をする。  
自由スカラー場の演算子は

　　\\(\phi(x) = \displaystyle{\int} \frac{d^3p}{(2\pi)^3}\frac{1}{\sqrt{2E_{\mathbf{p}}}}(a_{\mathbf{p}}e^{-ip\cdot x} + a_{\mathbf{p}}^{+}e^{ip\cdot x})\\)

と書かれる。ただし、\\(p\\) は4次元の運動量で、\\(p^0 = E_{\mathbf{p}} = \sqrt{\mathbf{p}\cdot\mathbf{p} + m^2}\\) とする。 
また、\\(a_{\mathbf{p}} , a_{\mathbf{p}}^{+}\\) は

　　\\([a_{\mathbf{p}} , a_{\mathbf{p}'}^{+}] = (2\pi)^3\delta^{(3)}(\mathbf{p} - \mathbf{p}')\\) 

をみたす演算子と考える。ただし、ここで、\\([A , B]\\) は \\(AB - BA\\) という意味で、交換子などという。他の組み合わせの交換子は \\(0\\) とする。

これら \\(a_{\mathbf{p}} , a_{\mathbf{p}}^{+}\\) が真空 \\(\|0>\\) に作用するのである。  
特に、

　　\\(a_{\mathbf{p}}\|0> = 0\\)

とする。

　　\\(a_{\mathbf{p}}^{+}\|0>\\)

はゼロではない。これは「運動量が \\(\mathbf{p}\\) の粒子が1つある状態」と解釈される。このような「状態」の前の係数は、重要な意味を持つが、「これは1粒子状態である」などという性質は、係数の大きさにはよらない。  

　　\\(\phi(\mathbf{x} , t)\|0>\\)

では、\\(a_{\mathbf{p}}\\) の項はすべて消え、\\(a_{\mathbf{p}}^{+}\\) の項はすべて残る。これは、無数の運動量の状態の重ね合わさった状態（次節を参照）と考えることができる。

\\(a_{\mathbf{p}}^{+}\\) を真空に作用させると1粒子状態になるので、これを生成演算子とよび、1粒子状態に \\(a_{\mathbf{p}}\\) を作用させると真空に戻るので、これを消滅演算子とよぶ。  
よって、たとえば、\\(a_{\mathbf{p}}^{+}a_{\mathbf{p}'}^{+}\|0>\\) は、「真空から2つの粒子（運動量が、\\(\mathbf{p} , \mathbf{p}'\\)）が生成された状態」「2粒子状態」と解釈される。より多くの粒子の状態も同様である。

場の演算子は、運動方程式とよばれる方程式をみたす。自由スカラー場の運動方程式は Klein-Gorodn方程式とよばれる。  
\\(\frac{\partial}{\partial x^\mu}\\) を \\(\partial_\mu\\) と書くと、Klein-Gordon方程式は次のように書ける。

　　\\((\partial\cdot\partial + m^2)\phi = 0\\)

上の \\(\phi(\mathbf{x} , t)\\) がKlein-Gordon方程式をみたすことは、微分して容易に示すことができる。  
自由スカラー場はこの式で特徴づけられるので、Klein-Gordon場ともいう。  

「自由スカラー場は、なぜKlein-Gordon方程式をみたすと考えられるのか」はここでは述べない。（多くの教科書では最小作用の原理から導出する。）ただ、次の事実を指摘しておく。  
量子力学（粒子の生成消滅までは考えない理論）は、その適用範囲内で大きな成果を得た。量子力学では粒子は波動方程式をみたす波動関数であらわされる。  
波動方程式は、非相対論的なエネルギーの式 \\(E = \frac{1}{2 m} p^2 + U\\) で、\\(E , p^1 , p^2 , p^3\\) を \\(i \frac{\partial}{\partial t} , -i \frac{\partial}{\partial x^1} , -i \frac{\partial}{\partial x^2} , -i \frac{\partial}{\partial x^3}\\) に置き換えて得られるものだった。
Klein-Gordon方程式は、その対応を相対論的なエネルギーの式 \\(p \cdot p = m^2 \\) にあてはめたものである。  

## 1.5 Dirac場

スピン1/2の自由フェルミオンはDirac場などとよばれる。  
Dirac場を説明するために、ガンマ行列というものが必要になる。それは4つの4×4の行列 \\(\gamma^\mu (\mu = 0 ～ 3)\\) で、次の関係式をみたすものである。

　　\\(\lbrace \gamma^\mu , \gamma^\nu \rbrace = 2g^{\mu\nu}\\)

ただし、ここで \\(\lbrace A , B \rbrace\\) は \\(AB + BA\\) という意味で、反交換子などという。また、\\(g^{\mu\nu}\\) は、\\(\mu = \nu = 0\\) のとき \\(1\\)、\\(\mu = \nu = 1 , 2, 3\\) のとき \\(-1\\) 、それ以外は \\(0\\) の行列（テンソル）である。
ガンマ行列は「上の関係をみたすもの」なので、いろいろな選び方がありうるが、ここでは特定しないでおく。

Dirac場の演算子は次のように書かれる。

\\(\psi(x) = \displaystyle{\int} \frac{d^3p}{(2\pi)^3}\frac{1}{\sqrt{2E_{\mathbf{p}}}}\Sigma_s(a_{\mathbf{p}}^su^s(p)e^{-ip\cdot x} + b_{\mathbf{p}}^{s+}v^s(p)e^{ip\cdot x})\\)  
\\(\bar{\psi}(x) = \displaystyle{\int} \frac{d^3p}{(2\pi)^3}\frac{1}{\sqrt{2E_{\mathbf{p}}}}\Sigma_s(b_{\mathbf{p}}^s\bar{v}^s(p)e^{-ip\cdot x} + a_{\mathbf{p}}^{s+}\bar{u}^s(p)e^{ip\cdot x})\\)

ここで、\\(s\\) は \\(1\\) か \\(2\\) であり、\\(u^s(p) , v^s(p)\\) は、（ガンマ行列を掛けることができる）4成分のもので、それぞれ

　　\\((\gamma\cdot p - m)u(p) = 0\\)  
　　\\((\gamma\cdot p + m)v(p) = 0\\)

の2つずつの独立した解たちである。
その具体的な形をここで見ても普通の人は絶望的な気分になるだけなので省略する。まずは、そういう解があると思えば良いと思う。  
これらは、Dirac場がDirac方程式とよばれる運動方程式

　　\\((i\gamma\cdot\partial - m)\psi(x) = 0\\)

の解になるように定められている。  
また \\(\bar{u}\\) のように上にバーがついたものは \\(u^{+}\gamma^0\\) （この \\(+\\) は複素共役をとって転置）という意味である。  
そして、「演算子パート」の \\(a_{\mathbf{p}}^s\\) たちは

　　\\(\lbrace a_{\mathbf{p}}^r , a_{\mathbf{q}}^{s+} \rbrace = \lbrace b_{\mathbf{p}}^r , s_{\mathbf{q}}^{s+} \rbrace = (2\pi)^3\delta^{(3)}(\mathbf{p} - \mathbf{q})\delta^{rs}\\)

をみたす。また、他の組み合わせの反交換子は \\(0\\) とする。


「なぜ、Dirac方程式が導入されたのか」また「それはどのように解かれるのか」は、物理に興味があるなら知りたいところだと思う。実際、Klein-Gordon方程式から出発する面白いストーリーがある。（Dirac方程式は、Klein-Gordon方程式の平方のようなものである。）さらに、数学的な見地からも興味深く、実践的な計算をするならぜひ慣れておくべきものでもあるだろう。しかし、かなり長い考察と計算がありそれを乗り切らなければ場の理論がわからないということでもないと思う。

Dirac場の場合、真空 \\(|0>\\) は次のように定義される。

　　\\(a_{\mathbf{p}}^s|0> = b_{\mathbf{p}}^s|0> = 0\\)

スカラー場の場合と同様に、\\(a_{\mathbf{p}}^{s+}\\) と \\(b_{\mathbf{p}}^{s+}\\) が生成演算子であり、\\(a_{\mathbf{p}}^{s}\\) と \\(b_{\mathbf{p}}^{s}\\) が消滅演算子である。

ここまでスカラー場とほとんど同じに見えるが、大きな違いがある。
フェルミオンの場合、\\(a_{\mathbf{p}}^{s+}\\) や \\(b_{\mathbf{p}}^{s+}\\) の自分自身との交換子（つまり、2乗）が \\(0\\) になる。つまり、\\((a_{\mathbf{p}}^{s+})^2 = 0\\)、\\((b_{\mathbf{p}}^{s+})^2 = 0\\) である。そのため、同じ状態の「2粒子状態」は存在しないことになる。


## 1.6 Feynmanプロパゲータ

粒子の状態は「多くの状態の重ね合わせ」であることが多い。「多くの状態が重ね合わさった状態」というのは、「そのなかの状態たちのどれにも実現される可能性がありながら、そのどれも実現されていない状態」のことである。このような「重ね合わさった状態」を観測すると、どれかの状態が実現されるのであるが、「含まれている割合が大きいもの」ほど実現される可能性が高いことになる。

たとえば、自由スカラー場で、状態 \\(|X>\\) が

　　\\(|X> = C a_{\mathbf{p}}^{+}|0> + \cdots\\)

のように展開されるとき、\\(a_{\mathbf{p}}^{+}|0>\\) の実現確率は \\(C\\) の絶対値の二乗に比例するのである。  
「どうしてそうなるのか？」に明快に答えられる人はいないと思う。ただ、これまでの物理学の発展の中でそう考えられるようになり、実際、実験によって確かめられている事実なのである。この \\(C\\) のようなものを確率振幅という。

確率振幅をうまく計算する方法として、

　　\\(<0|\\)

を定義する。
これは

　　\\(<0|0> = 1\\)  
　　\\(<0|a_{\mathbf{p}}^{+} = 0\\)

となるものとする。

そうすると、\\(<0|a_{\mathbf{p}'}a_{\mathbf{p}}^{+}|0> = (2\pi)^3\delta^{(3)}(\mathbf{p}' - \mathbf{p})\\) より、\\(<0|a_{\mathbf{p}'}|X>\\) を計算すれば \\(C\\) がわかることになる。

ここで、後の議論で重要になるスカラー場のFeynmanプロパゲータ（ファインマンの伝搬関数）を紹介する。  
まず、Tという演算子を導入する。これは、「場の演算子の積に作用し、場の演算子の時間が前のものを右にもっていく」というものである。たとえば、場の演算子2つに対しては、

　　\\(T\phi(x)\phi(y)\\)  
　　　　\\( = \phi(x)\phi(y)　（x^0 > y^0のとき）\\)  
　　　　\\( = \phi(y)\phi(x)　（x^0 < y^0のとき） \\)

となる。

\\(<0|T\phi(x)\phi(y)|0>\\) をスカラー場のFeynmanプロパゲータという。
Feynmanプロパゲータは、その形から、\\(x^0 > y^0\\) のときは、\\(y\\) に置かれた粒子が \\(x\\) まで伝搬する確率振幅、\\(x^0 < y^0\\) のときは、\\(x\\) に置かれた粒子が \\(y\\) まで伝搬する確率振幅を表すものに見える。ただし、今の段階では「そのように見える」程度だと思う。これを使って実際の計算をし、実験結果と一致する結果を出せることはあとで見る。

計算すると個別の \\(x , y \\) ではなく \\(x - y\\) に依存することがわかるので、\\(D_F(x - y)\\) と書く。実際、少々の計算ののち次のように書かれる。

　　\\(D_F(x - y) = \displaystyle{\int} \frac{d^4p}{(2\pi)^4}\frac{i}{p^2 - m^2 + i\epsilon}e^{-ip\cdot(x - y)}\\)

ここで、\\(\epsilon\\) は「無限に小さい正の数」を意味する。（すなわち、積分計算後、正の方向から 0 に近づけた極限をとる。）  

Dirac場のTも定義される。

　　\\(T\psi(x)\bar{\psi}(y)\\)  
　　　　\\( = \psi(x)\bar{\psi}(y)　（x^0 > y^0のとき）\\)  
　　　　\\( = -\bar{\psi}(y)\psi(x)　（x^0 < y^0のとき） \\)

フェルミオンは基本的に前後を変えると－符号がつく。  
Feynmanプロパゲータは次のようになる。

　　\\(S_F(x - y) = <0|T\psi(x)\bar{\psi}(y)|0>\\)  
　　　　　　\\( = \displaystyle{\int} \frac{d^4p}{(2\pi)^4}\frac{i(\gamma\cdot p + m)}{p^2 - m^2 + i\epsilon}e^{-ip\cdot(x - y)}\\)
