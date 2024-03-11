# HDU PHOENIX 战队 2025 赛季视觉组第一轮考核

本次任务**5选3**，多做不加分。

**重要：请在 linux 环境下完成所有考核**  
**不要虚拟机**  
**不要虚拟机**  
**不要虚拟机**

本 `README` 仅有任务的简要描述，具体要求请查看子文件夹的 `README`。

## 任务1：OpenCV

使用 `cpp` 完成以下任务，提交代码和运行结果。

+ 不使用 `cv` 提供的库函数，用三种方式实现图像的二值化（提示：遍历 `cv::Mat` 有几种方式？）
+ 使用 `canny` 算子实现图像的边缘检测
+ 对给定图片上的回形针进行计数
+ 将给定图片进行腐蚀、膨胀、开运算、闭运算，调整算子形状和大小，观察运算结果
+ 将一张 `RGB` 图片转换为 `HSV` 图片，调整 `HSV` 图片的 `H`、`S`、`V` 通道，观察运算结果
+ 开启摄像头，实时显示摄像头画面。
  + 选做：如何使用手机摄像头？（提示：互联网通信）
+ 对给定图片进行伽马矫正
+ 提取口罩

选做：曼德博集合

使用任一开源图形图像库，画出 `math` 中 `README` 中的函数图像。  
可选语言有： Python、C、C++  
可使用 matlab 或 mathematica 研究函数性质，但不可使用 matlab 或 mathematica 画图 : )

## 任务2：DeepLearning

本任务建议在学过python和opencv进行。

神经网络是一种玄学的工具，在传统程序中我们希望能掌握代码的运行原理，但在一个复杂的目标检测网络中我们并不要求这一点。初学神经网络时，把它当成一个能拟合任何函数的黑盒能少受很多苦（是任何，比如“输入是图片(实际是矩阵)，输出是图片里的内容”这种无法用数学公式表示的函数）。

在RM中，我们只需要学习CNN(卷积神经网络)，你如果学有余力也可以学习一下Transformer，Self-Attention，甚至是强化学习RL，对抗学习（不要勉强）。

另外，神经网络有只有python一种语言，请不要尝试使用c++来折磨自己（除了部署时），推荐编辑器PyCharm，Jupyter Notebook

## 任务3：C++/Algorithm

以下为必做：

+ 完善 `Matrix` 类
+ 完成三个 question
+ 拯救学姐（贪吃蛇）

以下为可选：

+ 修改 `thread/thread.cpp` 中的代码
+ 实现一个进程间通信（IPC）框架
+ 压缩一张位图
+ 实现一个坐标系转换类

## 任务4：证明黎曼猜想

> 黎曼猜想（或称黎曼假设）是关于黎曼ζ函数ζ(s)的零点分布的猜想，由数学家波恩哈德·黎曼于1859年提出。黎曼观察到，素数的频率紧密相关于一个精心构造的所谓黎曼zeta函数ζ(s)的性态。复平面上使黎曼ζ 函数取值为零的点被称为黎曼ζ函数的零点。s=-2n （n 为正整数）是黎曼 ζ 函数的零点，这些零点分布有序、 性质简单，被称为黎曼ζ 函数的平凡零点 (trivial zero)。除了这些平凡零点外，黎曼ζ函数还有许多其它零点，它们的性质远比那些平凡零点来得复杂，被称为非平凡零点 (non-trivial zeros)。
>
> 在黎曼猜想的研究中， 数学家们把复平面上 Re(s)=1/2 的直线称为 critical line（临界线）。运用这一术语，黎曼猜想也可以表述为：黎曼ζ 函数的所有非平凡零点都位于 critical line 上。即黎曼ζ 函数的所有非平凡零点都位于复平面上 Re(s)=1/2 的直线上（Re(s)表示复数s的实数部分）。
> 
> (百度百科)

请证明：黎曼 ζ 函数的所有非平凡零点都位于复平面上 Re(s)=1/2 的直线上。给出详细、严谨的证明过程。

## 任务5：证明哥德巴赫猜想
>哥德巴赫猜想（Goldbach's conjecture）是数论中存在最久的未解问题之一。这个猜想最早出现在1742年普鲁士数学家克里斯蒂安·哥德巴赫与瑞士数学家莱昂哈德·欧拉的通信中。用现代的数学语言，哥德巴赫猜想可以陈述为：
“	任一大于2的偶数，都可表示成两个素数之和。	”
这个猜想与当时欧洲数论学家讨论的整数分拆问题有一定联系。整数分拆问题是一类讨论“是否能将整数分拆为某些拥有特定性质的数的和”的问题，比如能否将所有整数都分拆为若干个完全平方数之和，或者若干个完全立方数的和等。而将一个给定的偶数分拆成两个素数之和，则被称之为此数的哥德巴赫分拆。例如，  
4 = 2 + 2  
6 = 3 + 3  
8 = 3 + 5  
10 = 3 + 7 = 5 + 5  
12 = 5 + 7  
14 = 3 + 11 = 7 + 7  
16 = 3 + 13 = 5 + 11  
>换句话说，哥德巴赫猜想主张每个大于等于4的偶数都是哥德巴赫数——可表示成两个素数之和的数。哥德巴赫猜想也是二十世纪初希尔伯特第八问题中的一个子问题。

请证明：任何一个大于2的偶数都可以表示成两个质数之和。给出详细、严谨的证明过程。
