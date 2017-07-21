### 关于

受 [android-interview-questions](https://github.com/MindorksOpenSource/android-interview-questions) 项目启发，这里想发挥众多 Android 中国开发者的力量，整理一份高质量、范围全的 Android 面试指南，旨在帮助更多的 Android 开发者提升技术，找到工作。

现在还是项目初期，项目背景见这里：[想跟大家一起做件小事](http://mp.weixin.qq.com/s/t038R0bDDZ6dg4bwDoj2cQ)，欢迎持续关注。

## Contents
 * [数据结构和算法](#数据结构与算法)
 * [Java 核心](#core-java)
 * [Android 核心](#core-android)
 * [架构](#架构)
 * [设计问题](#设计问题)
 * [工具和技能](#工具和技能)
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


### 架构

* 请介绍一下你做的上一个 App 的架构。
* 请介绍一下 MVP。 [链接](https://blog.mindorks.com/essential-guide-for-designing-your-android-app-architecture-mvp-part-1-74efaf1cda40)
* Presenter 是什么？
* 什么是模型？
* 请介绍一下 MVC。
* Controller 是什么？
* 请介绍一下 MVVM。 [链接](https://github.com/MindorksOpenSource/android-mvvm-architecture)
* 谈谈你对代码整洁之道（clean code）的理解。[链接](https://blog.mindorks.com/every-programmer-should-read-this-book-6755dedec78d)


### 设计问题

* 请设计 Uber App。
* 请设计 Facebook App。
* 请设计 Facebook Near-By Friends App。
* 请设计 WhatsApp。
* 请设计 SnapChat。
* 基于地理位置 App 的设计问题。


### 工具和技能

* Git. [链接](https://github.com/git-tips/tips)
* RxJava. [链接](https://blog.mindorks.com/a-complete-guide-to-learn-rxjava-b55c0cea3631)
* Dagger 2. [链接](https://medium.com/p/a-complete-guide-to-learn-dagger-2-b4c7a570d99c)
* Android 开发实用工具。 [链接](https://blog.mindorks.com/android-development-useful-tools-fd73283e82e3)
* Firebase. [链接](https://firebase.google.com/)


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
