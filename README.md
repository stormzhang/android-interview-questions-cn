### 关于

受 [android-interview-questions](https://github.com/MindorksOpenSource/android-interview-questions) 项目启发，这里想发挥众多 Android 中国开发者的力量，整理一份高质量、范围全的 Android 面试指南，旨在帮助更多的 Android 开发者提升技术，找到工作。

现在还是项目初期，项目背景见这里：[想跟大家一起做件小事](http://mp.weixin.qq.com/s/t038R0bDDZ6dg4bwDoj2cQ)，欢迎持续关注。

## Contents
 * [数据结构和算法](#data-structures-and-algorithms)
 * [Java 核心](#core-java)
 * [Android 核心](#core-android)
 * [架构](#architecture)
 * [设计问题](#design-problem)
 * [工具和技能](#tools-and-technologies)
 * [Android 测试驱动开发](#android-test-driven-development)
 * [其他](#others)


### Android 核心


* 解释 Activity 的生命周期 .
* 说出所有 Android 组件 .
* Service vs IntentService . [Link](https://stackoverflow.com/a/15772151/5153275)
* Android Application 的结构是什么 ?
* Android 中怎么进行数据持久化 ?
* 怎么实现一个耗时操作 ?
* 在两个 Fragments 中怎么进行通信 ?
* 解释 Notification ?
* 两个不同应用怎么相互作用 ?
* Fragment 是什么 ?
* 为什么提倡使用默认构造方法来创建 fragment ? [Link](https://stackoverflow.com/a/16042750/2809326)
* 为什么用Bundle进行数据传递 , 为什么不使用简单的Map数据结构 ?
* 解释 Fragment 的生命周期. [Link](https://www.techsfo.com/blog/wp-content/uploads/2014/08/complete_android_fragment_lifecycle.png)
* Android 中的 Dialog 是什么 ?
* Android 中的 View 是什么 ?
* 你会自定义 View 吗 ? 怎么自定义 ?
* ViewGroup 是什么 ? 它和 View 有什么区别 ?
* Activity 和 Fragment 有什么区别 ? 解释下两者之间的关系 .
* Serializable 和 Parcelable 之间有什么区别 ? 哪个是Android中最好的方法 ?
* "launch modes" 是什么 ? [Link](https://blog.mindorks.com/android-activity-launchmode-explained-cbc6cf996802)
* Intents 是什么 ? [Link](https://stackoverflow.com/questions/6578051/what-is-an-intent-in-android)
* 隐式 Intent ( Implicit Intent ) 是什么 ?
* 显式 Intent ( Explicit Intent ) 是什么 ?
* AsyncTask 是什么 ?
* BroadcastReceiver 是什么 ? [Link](https://stackoverflow.com/questions/5296987/what-is-broadcastreceiver-and-when-we-use-it)
* LocalBroadcastManager 是什么 ? [Link](https://developer.android.com/reference/android/support/v4/content/LocalBroadcastManager.html)
* JobScheduler 是什么 ? [Link](http://www.vogella.com/tutorials/AndroidTaskScheduling/article.html)
* DDMS是什么 ? 可以用它来做什么 ?
* support library 是什么 ? 它是为什么引进的 ?[Link](http://martiancraft.com/blog/2015/06/android-support-library/)
* ContentProvider 是什么 ? 它通常用于做什么 ?
* Android Data Binding 是什么 ? [Link](https://developer.android.com/topic/libraries/data-binding/index.html)
* Android Architecture Components 是什么 ? [Link](https://developer.android.com/topic/libraries/architecture/index.html)
* ADB 是什么 ?
* ANR 是什么 ? 怎么防止ANR出现 ?
* `AndroidManifest.xml` 是什么 ?
* 说明 broadcasts 和 intents 是如何工作的 , 使其可以在你的应用中传递消息 ?
* 由于 `Bitmaps` 在 Android 中会消耗过多的内存 , 你是怎么处理的 ?
* 在 Android 中有哪些数据存储的方法 ?
* Dalvik Virtual Machine 是什么 ?
* AsyncTask 和 Activity 之间的生命周期有什么关系 ? 这里面有什么问题 ? 如何避免 ?
* intent filter 是用来干嘛的 ?
* Sticky Intent 是什么 ? [Link](http://www.androidinterview.com/what-is-a-sticky-intent/)
* AIDL 是什么 ? 举例说明通过AIDL创建一个 bounded service 的步骤 .
* permission 中的不同保护级别是什么 ?
* 在屏幕旋转的时候如何保持 Activity 状态 ? [Link](https://stackoverflow.com/questions/3915952/how-to-save-state-during-orientation-change-in-android-if-the-state-is-made-of-m)
* Relative Layout vs Linear Layout.
* How to implement XML namespaces?
* `View.GONE` 和 `View.INVISIBLE` 之间的区别 ?
* 一个正常的 bitmap 和 一个 nine-patch 图片之间有什么区别 ?
* 谈谈位图池 .  [Link](https://blog.mindorks.com/how-to-use-bitmap-pool-in-android-56c71a55533c)
* 如何避免Android内存泄漏 ?
* Android 主屏幕上的 widgets 是什么 ?
* AAPT 是什么 ?
* 如何在Android应用程序中找出内存泄漏 ?
* 如何解决应用异常崩溃 ?
* 为什么要避免在主线程上运行非ui代码 ?
* How did you support different types of resolutions?
* Doze 是什么 ? What about App Standby?
* What can you use for background processing in Android?
* ORM 是什么 ? 它是怎么工作的 ?
* Loader 是什么 ?
* 什么是NDK，为什么它是有用的 ?
* StrictMode 是什么 ? [Link](https://blog.mindorks.com/use-strictmode-to-find-things-you-did-by-accident-in-android-development-4cf0e7c8d997)
* Lint 是什么 ? 用来做什么 ?
* `SurfaceView` 是什么 ?
* `ListView` 和 `RecyclerView` 有什么区别 ?
* ViewHolder 模式是什么 ? 为什么要用它 ?
* PendingIntent 是什么 ?
* 可以手动调用垃圾收集器吗 ?
* 什么是定期更新屏幕的最佳方式 ?
* Broadcasts 的不同类型是什么 ?
* 你开发过 widgets 吗? 描述下 . [Link](https://blog.mindorks.com/android-widgets-ad3d166458d3)
* Context 是什么? 怎么用 ? [Link](https://medium.com/p/understanding-context-in-android-application-330913e32514)
* 你知道 view tree 是什么吗 ? 如何优化其深度 ?
* `onTrimMemory` 这个方法是干嘛的 ?
* 一个 Android app 可以运行在不同的进程中吗 ? 怎么做到 ?
* 什么时候会出现 OutOfMemory ?
* `spannable` 是什么 ?
* renderscript 是什么 ? [Link](https://blog.mindorks.com/comparing-android-ndk-and-renderscript-1a718c01f6fe)
* Dalvik 和 ART 之间的区别 ?
* FlatBuffers vs JSON. [Link](https://blog.mindorks.com/why-consider-flatbuffer-over-json-2e4aa8d4ed07)
* Annotations 是什么 ? [Link](https://blog.mindorks.com/creating-custom-annotations-in-android-a855c5b43ed9), [Link](https://blog.mindorks.com/improve-your-android-coding-through-annotations-26b3273c137a)
* 谈谈 Constraint Layout [Link](https://blog.mindorks.com/using-constraint-layout-in-android-531e68019cd)
* `HashMap`, `ArrayMap` 和 `SparseArray` [Link](https://blog.mindorks.com/android-app-optimization-using-arraymap-and-sparsearray-f2b4e2e3dc47)
* 解释 Looper, Handler 和 HandlerThread. [Link](https://blog.mindorks.com/android-core-looper-handler-and-handlerthread-bd54d69fe91a)
* How to reduce battery usage in an android application? [Link](https://blog.mindorks.com/battery-optimization-for-android-apps-f4ef6170ff70)
* `SnapHelper` 是什么? [Link](https://blog.mindorks.com/using-snaphelper-in-recyclerview-fc616b6833e8)
* 如何在Android中处理多点触控 [link](https://arjun-sna.github.io/android/2016/07/20/multi-touch-android/)


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
