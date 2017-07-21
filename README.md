### 关于

受 [android-interview-questions](https://github.com/MindorksOpenSource/android-interview-questions) 项目启发，这里想发挥众多 Android 中国开发者的力量，整理一份高质量、范围全的 Android 面试指南，旨在帮助更多的 Android 开发者提升技术，找到工作。

现在还是项目初期，项目背景见这里：[想跟大家一起做件小事](http://mp.weixin.qq.com/s/t038R0bDDZ6dg4bwDoj2cQ)，欢迎持续关注。

## Contents
* [数据结构和算法](#data-structures-and-algorithms)
* [Java 核心](#java-核心)
* [Android 核心](#core-android)
* [架构](#architecture)
* [设计问题](#design-problem)
* [工具和技能](#tools-and-technologies)
* [Android 测试驱动开发](#android-test-driven-development)
* [其他](#others)


### Java 核心

* 解释一下 OOP 的概念
  - 面向对象编程是使用类，对象，
    [继承性](https://zh.wikipedia.org/wiki/%E7%BB%A7%E6%89%BF_(%E8%AE%A1%E7%AE%97%E6%9C%BA%E7%A7%91%E5%AD%A6))，
    [多态性](https://zh.wikipedia.org/wiki/%E5%A4%9A%E5%9E%8B_(%E8%AE%A1%E7%AE%97%E6%9C%BA%E7%A7%91%E5%AD%A6))，
    [封装性](https://zh.wikipedia.org/wiki/%E5%B0%81%E8%A3%9D_(%E7%89%A9%E4%BB%B6%E5%B0%8E%E5%90%91%E7%A8%8B%E5%BC%8F%E8%A8%AD%E8%A8%88))和
    [抽象](https://zh.wikipedia.org/wiki/%E6%8A%BD%E8%B1%A1%E5%8C%96_(%E8%A8%88%E7%AE%97%E6%A9%9F%E7%A7%91%E5%AD%B8))的一种程序设计方法。
* 抽象类和接口的区别？[链接](https://arjun-sna.github.io/java/2017/02/02/abstractvsinterface/)
    - 抽象类是一个可同时包含具体方法和抽象方法(方法未被实现)的类。抽象方法必须被该抽象类的子类实现。抽象类是可以继承的。
    - 接口像是描述类的一张蓝图或者说是类的一种契约，它包含了许多空方法，这代表着它的所有的子类都应该拥有共同点。它的子类应该提供这些空方法的具体实现。一       个类需要用```implements```来实现接口，接口可以用```extends```来继承其他接口。
* What is serialization? How do you implement it?
  - Serialization is the process of converting an object into a stream of bytes in order to store 
    an object into memory so that it can be recreated at a later time while still keeping the 
    objects original state and data. In Java there are two methods of doing this, one is by 
    implementing Serializable or Parcelable. In Android, however, Serializable should never be used 
    in Android. Parcelable was created to be more efficient then Serializable, and performs about 
    10x faster then Serializable because Serializable uses reflection which is a slow process and 
    tends to create a lot of temporary objects which may cause garbage collection to occur more often.
* 什么是单例？
  - 单例模式指的是一个类只能被初始化一次，即只有一个实例。[单例模式限定一个类只能拥有一个实例。这在系统中只需要一个实例来和其他模块协调工作时是很实用的。单例普遍使用在只需要一个或是限制一定数量实例的系统中。](https://en.wikipedia.org/wiki/Singleton_pattern)
* 什么是匿名内部类？
* 对字符串进行```==```和```equals()```操作时有什么区别？
* ```hashCode()```和```equals()```何时使用？
* What are these `final`, `finally` and `finalize`?
* 什么是内存泄露，Java 是如何处理它的？
* What is garbage collector? How it works?
  -All objects are allocated on the heap area managed by the JVM. 
  As long as an object is being referenced, the JVM considers it  alive. 
  Once an object is no longer referenced and therefore is not reachable by the application code,
  the garbage collector removes it and reclaims the unused memory.
* 比较 `Arrays` 和 `ArrayLists`。
* 比较 `HashSet` 和 `TreeSet`。
* Java 中的类型转换。
* 方法重载和重写的区别
    <p align="center">
        <img alt="Overloading and Overriding" src="https://github.com/stormzhang/android-interview-questions-cn/blob/master/assets/overloading-vs-overriding.png">
    </p>

    - 重载发生在编译时，重写发生在运行时。重载方法调用与其定义的绑定发生在编译时，但是重写方法调用与其定义的绑定在运行时发生。

    - 静态方法可以重载，意味着一个类可以有多个同名的静态方法。静态方法不能被重写，即使在子类中声明了一个相同的静态方法，它与父类的相同方法无关。

    - 最基本的区别是重载是在同一个类中完成的，重写父类需要有子类。重写是给父类的继承方法一个具体的实现。

    - 静态绑定用于方法重载，动态绑定用于方法重写。性能：重载比重写更有效率，原因是方法重写的绑定是在运行时完成的。

    - 私有方法和用 `final` 修饰的方法可以重载但不可重写。这意味着一个类可以有多个同名的 `private/final` 方法，子类不能重写父类的 `private/final` 方法。

    - 方法重载的情况下不关心返回值类型， 它可以相同，也可以不同。但是方法重写的情况下可以有多个具体的返回值类型。

    - 方法重载时参数列表必须不同，方法重写时参数列表必须相同。

* 什么是访问修饰符？它们能做什么？
* 接口可以继承另一个接口吗？
* Java 中 `static` 关键字是什么意思？
* Java 中静态方法可以被重写吗？
* 什么是多态？什么是继承？
* `Integer` 和 `int` 之间的区别
* Java 中的对象是否会以引用传递或者值传递？详细说明。
* 什么是 ThreadPoolExecutor？ [Link](https://blog.mindorks.com/threadpoolexecutor-in-android-8e9d22330ee3)
* 本地变量、实例变量以及类变量之间的区别？
* 什么是反射？ [Link](http://tutorials.jenkov.com/java-reflection/index.html)
* 在 Java 中什么是强引用、软引用、弱引用以及虚引用？
* 什么是依赖注入？能说几个依赖注入的库么？你使用过哪些？
* 关键字```synchronized```的作用是什么？
* 为什么说```String```不可变的？
* 修饰符```transient```和```volatile```的作用是什么？
* ```finalize()```方法的作用是什么？
* How does the `try{}finally{}` works?
* What is the difference between instantiation and initialization of an object?
* When is a `static` block run?
* Explain Generics in Java?
* Difference between `StringBuffer` and `StringBuilder`?
* `StringBuilder` 是怎么避免不可变字符串分配的问题？
* 什么是自动装箱和拆箱？
* 枚举和迭代器有什么区别？
* Java 中 _fail-fast_ 和 _fail-safe_ 的区别？
* 什么是 Java 优先级队列？
* 什么是设计模式？[链接](https://github.com/iluwatar/java-design-patterns)


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
