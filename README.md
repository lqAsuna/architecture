# architecture

## 软件架构与框架之间的区别与联系

### 软件架构：
软件架构是一个系统的草图，把系统分解为一些部件，描述这些部件的职责及它们之间的协作行为。它决定了子系统之间的关系、分层与通讯方式、公共设计原则/风格、功能需求与非功能需求的优先级与取舍原则等。

### 软件框架
软件框架是特定语言和技术的架构应用解决方案，用于分离与业务无关的内容，让开发人员更专注于业务实现。软件框架是领域分析结果的软件化，是领域内最终应用的模板。  

### 区别
- 软件架构是一个系统的草图，软件框架就是领域分析结果的软件化，是领域内最终应用的模板
- 软件架构不是软件，软件框架是软件

### 联系

- 软件架构用于指导软件框架的设计，是软件框架的重要决策
- 框架是一种或多种架构的组合实现

## 以你的项目为案例，绘制三层架构模型图，细致到分区

![image](https://github.com/lqAsuna/architecture/blob/master/image/res.png)

## 结合你程序的结构，从程序员角度说明三层架构给开发者带来的便利

- 三层架构使得开发工作分工明确，每个层、包的职责清晰
- 三层架构可以减少耦合度、增强内聚性、提高复用性。提供了并行开发支持。利用前后端分离，实现并行开发。
- 结构清晰，有利于后期的维护和升级
- 可以降低层与层之间的依赖

## 研究 VUE 与 Flux 状态管理的异同

### 相同点
- VUE与Flux数据流均是单向流
- VUE与Flux状态管理都是基于FLUX架构，该架构有效解决大型业务中复杂数据流的管理问题

### 不同点
- Vuex拥有同步异步2种更新方式，而Flux不区分同步异步
- VUE是一个构建数据驱动的web界面的渐进式框架，而Flux是一种前端状态管理架构思想，专门解决软件的结构问题
- VUE与Flux对数据流的顺序不同
