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

#### 14 - 20
* 方法重载和重写的区别
    <p align="center">
        <img alt="Overloading and Overriding" src="https://github.com/stormzhang/android-interview-questions-cn/blob/master/assets/overloading-vs-overriding.png">
    </p>

    重载发生在编译时，重写发生在运行时。重载方法调用与其定义的绑定发生在编译时，但是重写方法调用与其定义的绑定在运行时发生。

    静态方法可以重载，意味着一个类可以有多个同名的静态方法。静态方法不能被重写，即使在子类中声明了一个相同的静态方法，它与父类的相同方法无关。

    最基本的区别是重载是在同一个类中完成的，重写父类需要有子类。重写是给父类的继承方法一个具体的实现。

    静态绑定用于方法重载，动态绑定用于方法重写。性能：重载比重写更有效率，原因是方法重写的绑定是在运行时完成的。

    私有方法和用 `final` 修饰的方法可以重载但不可重写。这意味着一个类可以有多个同名的 `private/final` 方法，子类不能重写父类的 `private/final` 方法。

    方法重载的情况下不关心返回值类型， 它可以相同，也可以不同。但是方法重写的情况下可以有多个具体的返回值类型。

    方法重载时参数列表必须不同，方法重写时参数列表必须相同。

#### 36 - 41    
* 什么是访问修饰符？它们能做什么？
* 接口可以继承另一个接口吗？
* Java 中 `static` 关键字是什么意思？
* Java 中静态方法可以被重写吗？
* 什么是多态？什么是继承？
* `Integer` 和 `int` 之间的区别



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
