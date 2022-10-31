# BluePrint Separable Convolutions

作者提出一种“蓝图分离卷积”(blueprint separable convolutions, BSConv)作为高效CNN的构建模块。受启发于预训练模型的核属性的量化分析：深度方向的强相关性。

 基于该发现，作者构建了一套理论基础并用于推导如何采用标准OP进行高效实现。更进一步，所提方法为深度分离卷积的应用(深度分离卷积已成为当前主流网络架构的核心模块)提供了系统的理论推导、可解释性以及原因分析。最后，作者揭示了基于深度分离卷积的网络架构(如MobileNet)隐式的依赖于跨核相关性；而所提BSConv则基于核内相关性，故可以为常规卷积提供一种更有效的拆分。

 作者通过充分的实验(大尺度分类与细粒度分类)验证了所提BSConv可以明显的提升MobileNet以及其他基于深度分离卷积的架构的性能，而不会引入额外的复杂度。对于细粒度问题，所提方法取得13.7%的性能提升；在ImageNet分类任务，BSConv在ResNet的“即插即用”取得了9.5%的性能提升。



[深度卷积重思考｜BSConv - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/142147021)

[知乎](https://zhuanlan.zhihu.com/p/166736637#:~:text=3.3%20Blueprint%20Separable%20Convolution%20%5B6%5D)