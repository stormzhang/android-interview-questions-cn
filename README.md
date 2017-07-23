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
 * [Android 核心](#android-核心)
 * [架构](#架构)
 * [设计问题](#设计问题)
 * [工具和技能](#工具和技能)
 * [Android 测试驱动开发](#android-测试驱动开发)
 * [其他](#其他)


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


### Android 核心

* 阐述一下 Activity 的生命周期。

* 谈谈 Android 的四大组件。

* Service 与 IntentService 的区别。[Link](https://stackoverflow.com/a/15772151/5153275)

* Android 应用的结构是什么？

* Android 应用中如何保存数据。

* 如何在 Android 应用中执行耗时操作。

* 两个 Fragment 之间如何通信。

* 阐述一下 Android 的通知系统。

* 两个不同的 app 之间如何交互。

* 什么是 Fragment？

* 为什么建议只使用默认的构造方法来创建 Fragment？[Link](https://stackoverflow.com/a/16042750/2809326)

* 为什么 Bundle 被用来传递数据，为什么不能使用简单的 Map 数据结构？

* 阐述一下 Fragment 的生命周期。[Link](https://www.techsfo.com/blog/wp-content/uploads/2014/08/complete_android_fragment_lifecycle.png)

* 如何理解 Android 的 Dialog ？

* 解释下 Android 的 View 。

* 你能创建自定义 View 吗？具体是如何创建的？

* 什么是 ViewGroup ，它与 View 的区别在哪里？

* Fragment 和 Activity 有什么区别？它们之间又有什么关系？

* 谈谈 Serializable 接口和 Parcelable 接口的区别。在 Android 中最好使用哪种接口？

* Activity 的启动模式有哪些？[Link](https://blog.mindorks.com/android-activity-launchmode-explained-cbc6cf996802)

* 解释一下 Android 中的 Intent 。[Link](https://stackoverflow.com/questions/6578051/what-is-an-intent-in-android)

* 什么是隐式 Intent ？

* 什么是显式 Intent ？

* 解释一下 AsyncTask 。

* 如何理解 Android 中的广播。[Link](https://stackoverflow.com/questions/5296987/what-is-broadcastreceiver-and-when-we-use-it)

* 如何理解 Android 的 LocalBroadcastManager 。[Link](https://developer.android.com/reference/android/support/v4/content/LocalBroadcastManager.html)

* 什么是 JobScheduler ？[Link](http://www.vogella.com/tutorials/AndroidTaskScheduling/article.html)

* 什么是 DDMS ？你可以用它来做什么？

* 解释一下什么是 support libary ，以及为什么要引入 support library ？[Link](http://martiancraft.com/blog/2015/06/android-support-library/)

* 如何理解 Android 中的 ContentProvider 。它通常用来干什么？

* 什么是 Data Binding ？[Link](https://developer.android.com/topic/libraries/data-binding/index.html)

* Android 的核心组件具体都有什么？[Link](https://developer.android.com/topic/libraries/architecture/index.html)

* 什么是 ADB ？

* 什么是 ANR ？如何避免发生 ANR ？

* AndroidManifest.xml 是什么？

* 解释一下 broadcast 和 intent 在 app 内传递消息的工作流程。

* 当 Bitmap 占用较多内存时，你是怎么处理的？

* Android 应用有哪些不同的存储数据的方式？

* 什么是 Dalvik 虚拟机？

* AsyncTask 的生命周期和(它所属的) Activity 的生命周期有什么关系？这种关系可能会导致什么
样的问题？ 如何避免这些问题发生？

* Intent filter 是用来做什么的？

* 什么是 Sticky Intent？[Link](http://www.androidinterview.com/what-is-a-sticky-intent/)

* 什么是 AIDL ？列举一下通过 AIDL 创建被绑定的服务（bounded service）的步骤。

* Android 的权限有多少个不同的保护等级？

* 在转屏时你如何保存 Activity 的状态？[Link](https://stackoverflow.com/questions/3915952/how-to-save-state-during-orientation-change-in-android-if-the-state-is-made-of-m)

* 相对布局和线性布局的区别。

* 如何实现 XML 命名空间？

* View.GONE 和 View.INVISIBLE 之间的区别。

* Bitmap 和 .9（nine-patch）图片之间有什么区别？

* 谈谈位图池。[Link](https://blog.mindorks.com/how-to-use-bitmap-pool-in-android-56c71a55533c)

* 在 Android 中如何避免内存泄漏？

* Android 桌面的小部件是什么？

* 什么是 AAPT ？

* 你是如何在 Android 应用程序中发现内存泄漏的？

* 你如何排查应用崩溃的原因？

* 为什么你应该避免在主线程上运行非用户界面相关的代码？

* 你是如何适配不同分辨率的手机的？

* 如何理解 Doze 模式。如何理解应用程序待机模式（App Standby）。

* 在 Android 中，你可以使用什么来进行后台操作?

* 什么是 ORM ？它是如何工作的？

* 什么是 Loader ？

* 什么是 NDK ，为什么它是有用的？

* 如何理解严格模式（StrictMode）。 [Link](https://blog.mindorks.com/use-strictmode-to-find-things-you-did-by-accident-in-android-development-4cf0e7c8d997)

* 什么是 Lint ？它的用途是什么？

* 什么是 SurfaceView ？

* ListView 和 RecyclerView 有什么区别？

* 什么是 ViewHolder 模式？为什么我们应该使用它？

* 什么是 PendingIntent ？

* 你能手动调用垃圾回收吗？

* 周期地更新页面的最好方式是什么？

* 有哪些类型的广播？

* 你开发过组件吗？请描述一下。[Link](https://blog.mindorks.com/android-widgets-ad3d166458d3)

* 如何理解上下文（Context）。怎么使用它？[Link](https://medium.com/p/understanding-context-in-android-application-330913e32514)

* 你知道什么是视图树(View Tree)吗？怎样优化它的深度？

* onTrimMemory() 方法是什么？

* Android 应用可以使用多进程吗？怎样使用？

* 内存溢出（OutOfMemory）是怎么发生的？

* 文本样式接口（Spannable）是什么？

* 什么是过度绘制（overdraw）？

* 什么是渲染脚本（renderscript）？[Link](https://blog.mindorks.com/comparing-android-ndk-and-renderscript-1a718c01f6fe)

* Dalvik 虚拟机模式和 ART（Android Runtime）虚拟机模式的区别。

* FlatBuffers 和 JSON 的区别。[Link](https://blog.mindorks.com/why-consider-flatbuffer-over-json-2e4aa8d4ed07)

* 谈谈 Android 的注解。[Link1](https://blog.mindorks.com/creating-custom-annotations-in-android-a855c5b43ed9), [Link2](https://blog.mindorks.com/improve-your-android-coding-through-annotations-26b3273c137a)

* 描述一下约束布局（Constraint Layout）。[Link](https://blog.mindorks.com/using-constraint-layout-in-android-531e68019cd)

* 阐述一下 Android 中的 HashMap , ArrayMap 和 SparseArray 。[Link](https://blog.mindorks.com/android-app-optimization-using-arraymap-and-sparsearray-f2b4e2e3dc47)

* 阐述一下 Looper, Handler 和 HandlerThread 。[Link](https://blog.mindorks.com/android-core-looper-handler-and-handlerthread-bd54d69fe91a)

* 如何降低 Android 应用的耗电量？[Link](https://blog.mindorks.com/battery-optimization-for-android-apps-f4ef6170ff70)

* SnapHelper 是什么？[Link](https://blog.mindorks.com/using-snaphelper-in-recyclerview-fc616b6833e8)

* 在 Android 中怎么处理多点触控？[link](https://arjun-sna.github.io/android/2016/07/20/multi-touch-android/)


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


### Android 测试驱动开发

* Espresso 是什么？ [链接](https://developer.android.com/training/testing/ui-testing/espresso-testing.html)

* Robolectric 是什么？ [链接](http://robolectric.org/)

* UI-Automator 是什么？ [链接](https://developer.android.com/training/testing/ui-testing/uiautomator-testing.html)

* 请解释一下单元测试。 

* 请解释一下设备化测试。

* 你是否做过单元测试或者自动测试？

* 为什么要使用 Mockito？ [链接](http://site.mockito.org/)

* 请描述一下 JUnit 测试。


### 其他

* 描述一下 REST APIs 如何工作 ？

* 描述一下 SQLite 。

* 描述一下 数据库 。

* 项目管理工具 - trello ，basecamp ，kanban ，jira ，asana 。

* 关于构建系统 - gradle , ant , buck 。

* APK 逆向工程 。

* 混淆器用于什么 ？

* 什么是混淆？ 用于什么？ 如何压缩 ？

* 如何构建你的发布版本的 APP ？

* 如何面向特定用户群体更新应用程序版本 ？

* 可以识别卸载我们的应用程序的用户吗 ？

* 缩小 APK 的体积 。[链接](https://blog.mindorks.com/how-to-reduce-apk-size-in-android-2f3713d2d662)

* Android 开发最佳实践 。[链接](https://blog.mindorks.com/android-development-best-practices-83c94b027fd3)

* Android 代码风格和指南 。[链接](https://blog.mindorks.com/android-code-style-and-guidelines-d5f80453d5c7)

* 你尝试使用过 Kotlin 吗 ？[链接](https://blog.mindorks.com/why-you-must-try-kotlin-for-android-development-e14d00c8084b)

* 开发 Android 应用程序时应该连续测量哪些指标 ？[链接](https://blog.mindorks.com/android-app-performance-metrics-a1176334186e)


### 贡献者

感谢这些无私的贡献者，排名不分先后。

[mengxn](https://github.com/mengxn)、[innovatorCL](https://github.com/innovatorCL)、[SmartNJ](https://github.com/SmartNJ)、[Zhiw](https://github.com/Zhiw)、[innovatorCL](https://github.com/innovatorCL)


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
