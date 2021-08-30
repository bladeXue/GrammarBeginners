# 编程语法快速学习指南

在实际编程的过程中，我们往往需要针对不同的需求使用不同的技术和语言，本项目列举了一些表格和笔记，帮助开发人员快速掌握一门新语言

## 关于本手册

本手册是一份编程初学者语法指导，我们罗列了一些编程语言学习中的通用概念，帮助入门者建立一个比较清晰的逻辑图谱

如果你是个编程新手，建议浏览一下下文的3691概念和特性表，而对于手册中的大部分内容，我们假定你已经有了一门或以上的语言学习经历，并对数组和指针有比较好的理解

## 语言的概念

人们总是喜欢讨论各种语言的优缺点，但是我们在讨论语言时到底在说什么，其实大部分时候我们在这个概念上是很模糊的，以至于到最后针对语言的讨论变成了无意义的口水战

当我们冷静下来，回归编程的本质，你就会发现任何一门语言，都只是计算机指令的排列组合，在编译过程结束后，它们的行为是一样的，都可以归结为两个点：

1. 整理参数
2. 调用函数

最简单程序称为**顺序执行**，它依次执行语句即可，但是当我们程序希望对各种条件因素作出反应时，我们会尝试改动各条语句的执行顺序，这就诞生了**逻辑结构**，但是到最后，我们最本质的操作还是单纯的**使用各种参数来调用函数**，而尝试组合不同参数，并让数据在各类函数结构中流动计算，从而获得目标结果的行为，称之为**算法**

在这种想法的驱使下，编程语言之间的界限开始变得模糊，除去了它们各自特殊的运行环境（如Javascript运行在浏览器中，Java字节码运行在虚拟机中等等），它们的目标行为其实是一致的，都是为了在某种参数的约定下，调用一组函数，在此基础上，我们整理了一张表，罗列了各种常见的语言特性，希望在你学习新语言时有所帮助

## 语言的3691

一门语言的句法内容通常有以下：

> 所有通用语言都会有这个部分，这个是编程语言的核心功能，也就是**运算**，我们称之为**语言句法的3691**

- 3种型：整型，浮点型和布尔型（另一种分类为值型，结构型和类型）
- 6种式：算术，逻辑，赋值，比较/关系，位和其它表达式
- 9种结构：控制流结构

| 分支   | 循环  | 中止     |
| ------ | ----- | -------- |
| if     | do    | break    |
| switch | while | continue |
| goto   | for   | return   |

> 不同语言中`for`和`break`有时会有不同的机制，同时除了这9大关键字，更加现代的语言还会有更多的语法糖关键字，比如`foreach`和`yield`都是很常见的新词，而且他们其实在运行时会翻译成语句，而不是单纯地作为关键字被执行

- 1种子程：表示了函数和面向对象在内的封装复用体系（概念源头是汇编的**子程序**），因为太多了，当作一种来说（但其实基本上都是C++那一套）

拿到一门语言，先把它的关键字扒拉出来看一遍，把上面的各个概念都圈出来，主动翻翻手册，那么配合一些类库的使用，基本可以编写一些简单的程序了

## 特性表

在3691这些基础句法之外，还会有一些比较常见的语言特性，共36项，这些特性有些是某门语言的灵魂，有些则是非常让人费解的设计（且大概率是新手的雷区），学习新语言时可以当个参考：

> 按照这张表看完后基本上这门语言的语法你就熟练了，学习新语言时应该照个这个表（重要特性有\*号），写出对应的代码片段并收录起来

> 使用这张表会使得你的学习从被动变成主动，思考语言的共性可以帮助理解，比如在JS中没有模板的概念，那你就要考虑是否存在替代的写法或者更好的解决方案，如果没有的话，为什么开发者放弃了这个特性，时刻要记住**即使语言不同，但是编程要造成的“行为”是一致的**

| 类型            | 语言特性     | 描述                   | 典例               |
| --------------- | ------------ | ---------------------- | ------------------ |
| 模块化\*7       | 注释         | 一些语言支持文档注释   |                    |
|                 | 注解         |                        |                    |
|                 | 入口         |                        |                    |
|                 | 命名风格     | 命名风格，如驼峰命名法 | C++ C#             |
|                 | 命名空间\*\* |                        |                    |
|                 | 包和模块     |                        |                    |
|                 | 异常处理     |                        |                    |
| 运行时和事件\*7 | 宏           |                        | C++ Rust           |
|                 | 常量         |                        |                    |
|                 | 编译过程\*\* |                        |                    |
|                 | 运行时       |                        | C# Java            |
|                 | 委托         |                        | C#                 |
|                 | 异步         |                        |                    |
|                 | 事件         |                        | C#                 |
| 函数和容器\*5   | 函数\*\*     |                        |                    |
|                 | Lambda表达式 |                        | C# Java JavaScript |
|                 | 装饰器       |                        | Python             |
|                 | 迭代器       |                        |                    |
|                 | 索引器       |                        |                    |
| 结构\*5         | 字符串       |                        |                    |
|                 | 元组         |                        | C# Python          |
|                 | 数组\*\*     |                        |                    |
|                 | 结构体       |                        | C C++ C# Rust      |
|                 | 指针         |                        | C C++ C# Rust      |
| 面向对象\*8     | 泛型         |                        |                    |
|                 | 模板         |                        | C++                |
|                 | 类\*\*       | 封装，继承，多态       |                    |
|                 | 虚类         |                        | C++ C#             |
|                 | 抽象类       |                        |                    |
|                 | 接口\*\*     |                        |                    |
|                 | 运算符重载   |                        | C++ C#             |
|                 | 多继承       |                        | C++                |
| 库\*4           | 数学库       |                        |                    |
|                 | IO库         |                        |                    |
|                 | 集合框架\*\* |                        |                    |
|                 | 网络库       |                        |                    |

## 学习之后

在完成上面的各个具体概念的学习后，你需要的就只剩下风格指导和最佳实践了，一般来说，不建议新手自己写代码，作为这个领域的新手应该去抄一份大佬的案例作为范本（如Java领域的绝对范本是Spring和官方文档的案例），修修改改成自己的内容，在这个过程中渐渐吃透大佬的代码，当你拥有大佬50%的功力时，你就是入门了，可以进一步学习发展出自己的风格了

## 总结

最后记住，学习是一个**持续**的过程，简单阅读我们的手册只能让你**入门**而不是**成为大牛**，不断地学习和思考才是成为大佬的必由之路


