MuJoCo物理
MuJoCo代表穆lti-乔与诠释动力有限公司ntact。它是一种通用物理引擎，旨在促进机器人、生物力学、图形和动画、机器学习以及其他需要快速准确模拟与其环境相互作用的关节结构的领域的研究和开发。

DeepMind 已经收购了 MuJoCo，我们目前正在准备开源代码库。与此同时，MuJoCo 可作为免费且不受限制的预编译二进制文件在mujoco.org的 Apache 2.0 许可下 下载。

MuJoCo 的源代码将在准备就绪后通过此 GitHub 存储库发布。同时，存储库托管 MuJoCo 的文档、其公共 API 的 C 头文件和示例程序代码。如果您想报告错误或提出功能请求，请将它们归档为GitHub 问题。也欢迎您对文档源文件提出拉取请求。

概述
MuJoCo 是一个带有 C API 的 C/C++ 库，供研究人员和开发人员使用。运行时模拟模块经过调整以最大限度地提高性能，并在由内置 XML 解析器和编译器预先分配的低级数据结构上运行。用户使用原生 MJCF 场景描述语言定义模型——一种 XML 文件格式，旨在尽可能让人类可读和可编辑。也可以加载 URDF 模型文件。该库包括具有原生 GUI 的交互式可视化，在 OpenGL 中呈现。MuJoCo 进一步公开了大量用于计算物理相关量的效用函数，不一定在模拟循环中。功能包括

在广义坐标中模拟，避免关节违规。

即使在存在接触的情况下也能很好地定义逆动力学。

通过凸优化统一连续时间的约束公式。

约束包括软接触、限制、干摩擦、等式约束。

粒子系统、布料、绳索和软物体的模拟。

执行器包括电机、气缸、肌肉、肌腱、曲柄滑块。

选择牛顿、共轭梯度或投影高斯-赛德尔求解器。

选择金字塔形或椭圆形摩擦锥，密集或稀疏雅可比矩阵。

选择 Euler 或 Runge-Kutta 数值积分器。

多线程采样和有限差分近似。

直观的 XML 模型格式（称为 MJCF）和内置模型编译器。

具有 OpenGL 交互式 3D 可视化功能的跨平台 GUI。

运行时模块用 ANSI C 编写并手动调整以提高性能。

要求
MuJoCo 二进制文件目前是为 Linux、macOS (Intel) 和 Windows 构建的。

文档
MuJoco 的当前文档可从mujoco.org/book 获得，该文档提供源自 ReStructuredText文档源文件的基于 Sphinx 的网页 。

引文
如果您使用 MuJoCo 进行已发表的研究，请引用：

@inproceedings{todorov2012mujoco,
  title={Mujoco: A physics engine for model-based control},
  author={Todorov, Emanuel and Erez, Tom and Tassa, Yuval},
  booktitle={2012 IEEE/RSJ International Conference on Intelligent Robots and Systems},
  pages={5026--5033},
  year={2012},
  organization={IEEE}
}
许可和免责声明
版权所有 2021 DeepMind Technologies Limited

目录中的 ReStructuredText 文档、图像和视频doc根据知识共享署名 4.0 (CC BY 4.0) 许可条款提供。您可以在https://creativecommons.org/licenses/by/4.0/legalcode获取许可证副本 。

源代码在 Apache 许可下获得许可，版本 2.0。您可以在https://www.apache.org/licenses/LICENSE-2.0获取许可证副本。

这不是官方支持的 Google 产品。
