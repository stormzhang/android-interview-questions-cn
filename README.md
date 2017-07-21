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
 * [Java 核心](#core-java)
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
