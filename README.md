<p align="center">
<img alt="AndroidInterviewQuestions" src="https://github.com/stormzhang/android-interview-questions-cn/blob/master/assets/android-interview-questions.png?raw=true">
</p>

# Android 面试指南

### 关于

受 [android-interview-questions](https://github.com/MindorksOpenSource/android-interview-questions) 项目启发，这里想发挥众多 Android 中国开发者的力量，整理一份高质量、范围全的 Android 面试指南，旨在帮助更多的 Android 开发者提升技术，找到工作。

现在还是项目初期，项目背景见这里：[想跟大家一起做件小事](http://mp.weixin.qq.com/s/t038R0bDDZ6dg4bwDoj2cQ)，也欢迎关注微信公众号 stormzhang，后续有任何进展我都会在公号进行通知的。

目前该项目有如下初步的计划：

1. 翻译 [android-interview-questions](https://github.com/MindorksOpenSource/android-interview-questions) 项目，不过翻译仅是我们的第一步而已，这个比较简单，目前第一步翻译工作已经被认领完毕；

2. 因为原项目很多只是列了一些问题，但是都没有答案的，所以第二步我们就是认领问题，整理答案，务必保证高质量、易理解，因为问题很多，所以这一步需要花费不少精力，也需要更多的同学参与进来，目前还在第一步阶段；

3. 第三步是补充与完善，原项目虽然列了不少领域，但是总归有些遗漏的，比如 Android 安全、插件化、Kotlin 等等，第三步是找在某一领域研究比较深的同学加入进来，对一些领域进行补充、完善，甚至会推出一些专题等；

## Contents
 * [数据结构和算法](#数据结构与算法)
 * [Java 核心](#Java核心)
 * [Android 核心](#core-android)
 * [架构](#architecture)
 * [设计问题](#design-problem)
 * [工具和技能](#tools-and-technologies)
 * [Android 测试驱动开发](#android-test-driven-development)
 * [其他](#others)

 ### 数据结构与算法

> 关于数据结构与算法，问题的难度完全取决于你所申请的公司

* 数组
* 链表
   - 链表看起来更像树，而不是数组，它使用一组结点来表示一个序列。每一个结点都包含数据和一个指针。在链表中，结点中的数据可以为任意类型，而指针则是指向下一结点的引用。链表包含一个头结点和一个尾结点。头结点是链表中的第一个结点，尾结点是最后一个结点。链表不是一个循环数据结构，所以尾结点没有指向头结点的指针，指针为空。一些基础方法的时间复杂度如下：

        | 算法          | 平均    | 最差      |
        |:------------:|:-------:|:--------:|
        | 空间 (Space)  | O(n)    | O(n)     |
        | 查找 (Search) | O(n)    | O(n)     |
        | 插入 (Insert) | O(1)    | O(1)     |
        | 删除 (Delete) | O(1)    | O(1)     |
* 双向链表
* 栈
    - 栈是一个有着“后进先出”特性的基础数据结构，这就意味着最后一个入栈的元素，也是第一个出栈的。栈就像是一堆书，想要得到书堆中的第一本书（最下面一本），必须把其他的书都先拿走。向栈中添加一个元素的操作被称为 Push（入栈），删除一个元素的操作被称为 Pop（出栈），查看且不删除最后一个入栈的元素的操作被称为 Top 。[实现栈的常用方法是使用链表（LinkedList），也可以使用不允许空值的 StackArray（使用数组实现），还有允许空值的 Vector](https://en.wikibooks.org/wiki/Data_Structures/Stacks_and_Queues#Performance_Analysis)

        <table>
            <tr>
                <th>算法</th>
                <th>平均</th>
                <th>最差</th>
                <th>图形表示</th>
            </tr>
            <tr>
                <td>空间 (Space)</td>
                <td>O(n)</td>
                <td>O(n)</td>
                <td rowspan="5">
                    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/29/Data_stack.svg/250px-Data_stack.svg.png"/>
                </td>
            </tr>
            <tr>
                <td>查找 (Search)</td>
                <td>O(n)</td>
                <td>O(n)</td>
            </tr>
            <tr>
                <td>入栈 (Push)</td>
                <td>O(1)</td>
                <td>O(1)</td>
            </tr>
            <tr>
                <td>出栈 (Pop)</td>
                <td>O(1)</td>
                <td>O(1)</td>
            </tr>
            <tr>
              <td>查看栈顶 (Top)</td>
              <td>O(1)</td>
              <td>O(1)</td>
            </tr>
        </table>
* 队列
* 优先队列
* 动态编程
* 字符串操作
* 二叉树
* 二叉搜索树
* 排序算法
* 哈希表与哈希图
* 广度优先搜索
* 深度优先搜索
* 贪心算法

 ### Java 核心

* OOP概念
   - OOP，Object-Oriented Programming，即面向对象编程，是使用类，对象，继承，多态，抽象和封装设计程序的方法论。

* 抽象对象和接口的不同之处
   - 抽象类是包含具体方法和抽象方法的类，抽象方法必须被子类继承，抽象类是可继承的。
  接口就像一个类的蓝图/合约。它只包含子类必须继承的空方法，子类提供了每个方法的具体实现。接口是可实现的。

* 什么是序列化？你是怎么实现它的？
   - 序列化是将对象转为字节流的过程，为了保存一个对象到内存，在被重新创建的时候能够仍然使用原始的状态和数据。在 Java 中有两种方式可以实现序列化：就是通过实现 Serializable 或者 Parcelable，但是在 Android 中尽量不要使用 Serializable，使用 Parcelable 比 Serializable 效率高大概十倍，因为 Serializable 使用的反射是一个很慢的进程，并且会产生大量的临时对象经常会导致垃圾回收。

* 什么是单例类？
   - 单例是一个类只能被实例化一次。单例模式限制了一个类只能实例化成一个对象，当一个对象需要在整个系统中协调行为的时候是很有用的。这个概念有时普遍用于当只有一个对象存在操作更有效，或者对于一个严格实例化确定数量对象的系统。

* 什么是匿名类？

* 对于 String 来说，== 和 .equals 的区别是什么？

* hashCode() 和 equals() 是用来做什么的？

* final, finally, finalize 是什么？

* 什么是内存泄漏，Java 是怎么处理它的？

* 什么是垃圾回收？它是怎么工作的？
   - 所有位于堆上的对象都被JVM管理，只要对象被引用，JVM就认为它是存活的，一旦对象不再被引用，也就是不会被代码所使用，垃圾收集器就会回收它并收回不再使用的内存。

* Array 和 ArrayList

* HashSet 和 TreeSet

* Java 中的类型转换

* 重载和重写的区别
   - 重载是发生在编译时，而重写发生在运行时。重载方法声明的绑定在编译时调用，而重写方法声明的绑定在运行时。
  静态方法可以被重载，也就是说相同方法名的静态方法可以不只有一个。静态方法不可以被重写，即使你在子类里声明了一个静态方法，它与父类中相同方法名的那个方法也无关。
  它们最基本的区别就是：重载在同一个类里，而重写是父类和子类中发生的。重写是子类对父类中方法的具体实现。
  静态绑定是用于重载方法，动态绑定用于重写方法。相比于重写，重载给出了更好的体验，原因就是重写是动态绑定的。
  私有方法和最终方法可以被重载但不能被重写，一个类可以有多个相同方法名的私有/最终方法，但是子类不可以重写父类的私有/最终方法。
  返回值类型不能区分方法重载，方法重载中返回值类型什么不重要，它可以是相同的，也可以是不同的。但是在方法重写中，重载方法必须和原方法具有相同的返回值类型。
  方法重载中，参数列表需要时不相同的。方法重写中，参数列表必须是相同的。

* 你知道有哪些访问修饰符？每个的作用范围都是什么？

* 一个接口可以继承另一个接口吗？

* Java 中 static 是什么意思？

* Java 中 static 方法是否可以被重写？

* 什么是多态？继承呢？

* Integer 和 int 的区别什么？

* Java 中是否可以传递值或引用，请详细说明。

* 什么是线程池？

* 局部变量，实例变量和全局变量的区别是什么？

* 什么是反射？

* Java 中强引用，软引用，弱引用都是什么？

* 什么是依赖注入？你能举出几个库吗？你用过哪些吗？

* synchronized 关键字的含义。

* 为什么说 String 是不可变的？

* 修饰符 transient 和 valatile 是用来干什么的？

* finalize() 方法是干什么的？

* try{}finally{} 实现流程是什么？ 

* 对象的实例化和初始化的区别。

* 静态块什么时候执行？

* 解释 Java 中的泛型。

* StringButter 和 StringBuilder 的区别。

* StringBuilder 怎么去避免不可变 String 的分配问题？

* 什么是自动装箱和自动拆箱？

* Enumeration 和 Iterator 的区别。

* Java 中 fail-fast 和 fail-safe 的区别是什么？

* 什么是 Java 优先队列？

* 什么是设计模式？

### 贡献者

感谢这些无私的贡献者，排名不分先后。

[mengxn](https://github.com/mengxn)

### License
```
   Copyright (C) 2017 stormzhang

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
```
