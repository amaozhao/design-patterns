# 设计模式

在软件工程中, 设计模式是软件设计中常见问题的通用可重复解决方案. 设计模式不是可以直接转换为代码的完成设计. 它是用来解决可在许多不同情况下使用的问题的描述或模板.

## 设计模式的使用

设计模式可以通过提供经过验证的经过验证的开发范例来加速开发过程. 有效的软件设计需要考虑在实施后期才可见的问题. 重用设计模式有助于防止可能导致重大问题的细微问题, 并提高熟悉模式的编码人员和架构师的代码可读性.

通常, 人们只了解如何将某些软件设计技术应用于某些问题. 这些技术难以应用于更广泛的问题. 设计模式提供了一般解决方案, 以不需要与特定问题相关的细节的格式记录.

此外, 设计模式允许开发人员使用众所周知的, 易于理解的名称进行软件交互. 通用设计模式可以随着时间的推移而得到改进, 使其比特殊设计更加强大.

## 创建型模式

这些设计模式都是关于类实例化的. 这种模式可以进一步分为类创建模式和对象创建模式. 虽然类创建模式在实例化过程中有效地使用继承, 但是对象创建模式有效地使用委托来完成工作.

*  [抽象工厂](./creational-patterns/abstract-factory.md)
  > 创建相似类的实例
*  [生成器](./creational-patterns/builder.md)
  > 将对象构造与其表示分开
*  [工厂方法](./creational-patterns/factory-method.md)
  > 创建多个派生类的实例
*  [对象池](./creational-patterns/object-pool.md)
  > 通过回收不再使用的对象，避免昂贵的资源获取和释放
*  [原型](./creational-patterns/prototype.md)
  > 复制或克隆完全初始化的实例
*  [单例](./creational-patterns/singleton.md)
  > 只存在一个实例的类

## 结构型模式

这些设计模式都是关于类和对象的组合. 结构类创建模式使用继承来组成接口. 结构对象模式定义了组合对象以获得新功能的方法.

* [适配器](./structural-patterns/adapter.md)
  > 匹配不同类的接口
* [桥接](./structural-patterns/bridge.md)
  > 将对象的接口与其实现分开
* [组合](./structural-patterns/composite.md)
  > 简单和复合对象的树结构
* [装饰器](./structural-patterns/decorator.md)
  > 动态地向对象添加职责
* [外观](./structural-patterns/facade.md)
  > 表示整个子系统的单个类
* [享元](./structural-patterns/flyweight.md)
  > 用于高效共享的细粒度实例
* [私有数据](./structural-patterns/private-class-data.md)
  > 限制 访问者/mutator 访问
* [代理](./structural-patterns/proxy.md)
  > 表示另一个对象的对象

## 行为设计模式

这些设计模式都是关于Class的对象通信. 行为模式是那些最特别关注对象之间通信的模式.

* [责任链](./behavioral-patterns/chain-of-responsibility.md)
  > 一种在一组对象之间传递请求的方法
* [命令](./behavioral-patterns/command.md)
  > 将命令请求封装为对象
* [解释器](./behavioral-patterns/interpreter.md)
  > 一种在程序中包含语言元素的方法
* [迭代器](./behavioral-patterns/iterator.md)
  > 按顺序访问集合的元素
* [中介者](./behavioral-patterns/mediator.md)
  > 定义类之间的简化通信
* [备忘录](./behavioral-patterns/memento.md)
  > 捕获并恢复对象的内部状态
* [空对象](./behavioral-patterns/null-object.md)
  > 旨在充当对象的默认值
* [观察者](./behavioral-patterns/observer.md)
  > 一种通知更改多个类的方法
* [状态](./behavioral-patterns/state.md)
  > Alter an object's behavior when its state changes
* [策略](./behavioral-patterns/strategy.md)
  > 将算法封装在类中
* [模板方法](./behavioral-patterns/template-method.md)
  > 将算法的确切步骤推迟到子类
* [访问者](./behavioral-patterns/visitor.md)
  > 为类定义新操作而不进行更改

## 批评

设计模式的概念受到计算机科学领域的一些人的批评.

### 针对错误的问题

对模式的需求源于使用计算机语言或抽象能力不足的技术. 在理想分解下, 不应复制概念, 而应仅参考. 但是如果引用某些东西而不是复制, 那么标签和目录就没有"模式".(Paul Graham)

### writes in the essay Revenge of the Nerds

Peter Norvig 提出了类似的论点. 他演示了设计模式书中23个模式中的16个(主要关注C++)在Lisp或Dylan中被简化或消除(通过直接语言支持).

### 缺乏正式的基础

对设计模式的研究过于临时， 有些人认为这个概念需要更加正式化。 在1999年的OOPSLA， 四人帮(在他们的全力合作下)进行了一次表演审判, 他们被指控犯有许多反对计算机科学的罪行. 他们被参加审判的"陪审员""定罪".

### 导致效率低下的解决方案

设计模式的想法是试图标准化已经接受的最佳实践. 原则上这似乎是有益的, 但在实践中它经常导致不必要的代码重复. 它几乎总是一个更有效的解决方案, 使用一个良好的因素实现, 而不是"只是勉强够用"的设计模式.

### 与其他抽象没有显着差异

一些作者声称设计模式与其他抽象形式没有显着差异, 并且使用新术语(从架构社区借用)来描述编程领域中的现有现象是不必要的. 模型 - 视图 - 控制器范例被吹捧为"模式"的一个例子, 它早于几年的"设计模式"概念. 一些人进一步认为, 设计模式社区(以及四人帮书)的主要贡献是使用亚历山大的模式语言作为一种文档形式; 这种做法在文献中经常被忽略.
