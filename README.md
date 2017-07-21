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

- Explain OOP Concept.
  - Object-Oriented Programming is a methodology to design a program using classes, objects, 
    [inheritance](https://en.wikipedia.org/wiki/Inheritance_(object-oriented_programming)),
    [polymorphism](https://en.wikipedia.org/wiki/Polymorphism_(computer_science)),
    [abstraction](https://en.wikipedia.org/wiki/Abstraction_(software_engineering)), and
    [encapsulation](https://en.wikipedia.org/wiki/Encapsulation_(computer_programming)).
- Differences between abstract classes and interfaces? [link](https://arjun-sna.github.io/java/2017/02/02/abstractvsinterface/)
  - An abstract class, is a class that contains both concrete and abstract methods 
    (methods without implementations). An abstract method must be implemented by the abstract class
     sub-classes. Abstract classes are extended.
  - An interface is like a blueprint/contract of a class. It contains empty methods that 
    represent what all of its subclasses should have in common. The subclasses provide the 
    implementation for each of these methods. Interfaces are implemented.
- What is serialization? How do you implement it?
  - Serialization is the process of converting an object into a stream of bytes in order to store 
    an object into memory so that it can be recreated at a later time while still keeping the 
    objects original state and data. In Java there are two methods of doing this, one is by 
    implementing Serializable or Parcelable. In Android, however, Serializable should never be used 
    in Android. Parcelable was created to be more efficient then Serializable, and performs about 
    10x faster then Serializable because Serializable uses reflection which is a slow process and 
    tends to create a lot of temporary objects which may cause garbage collection to occur more often.
- What is Singleton class?
  - A singleton is a class that can only be instantiated once.[This singleton pattern restricts 
    the instantiation of a class to one object. This is useful when exactly one object is needed 
    to coordinate actions across the system. The concept is sometimes generalized to systems 
    that operate more efficiently when only one object exists, or that restrict the instantiation 
    to a certain number of objects.](https://en.wikipedia.org/wiki/Singleton_pattern)
- What are anonymous classes?
- What is the difference between using `==` and `.equals` on a string?
- What is the `hashCode()` and `equals()` used for?
- What are these `final`, `finally` and `finalize`?
- What is memory leak and how does Java handle it?
- What is garbage collector? How it works?
  -All objects are allocated on the heap area managed by the JVM. 
  As long as an object is being referenced, the JVM considers it  alive. 
  Once an object is no longer referenced and therefore is not reachable by the application code,
  the garbage collector removes it and reclaims the unused memory.
- `Arrays` vs `ArrayLists`.
- `HashSet` vs `TreeSet`.
- Typecast in Java.
- Difference between method overloading and overriding.
  <p align="center">
  <img alt="Overloading and Overriding" src="https://github.com/codeshef/android-interview-questions/blob/master/assets/overloading-vs-overriding.png">
  </p>

Overloading happens at compile-time while Overriding happens at runtime: The binding of overloaded method call to its definition has happens at compile-time however binding of overridden method call to its definition happens at runtime.

Static methods can be overloaded which means a class can have more than one static method of same name. Static methods cannot be overridden, even if you declare a same static method in child class it has nothing to do with the same method of parent class.

The most basic difference is that overloading is being done in the same class while for overriding base and child classes are required. Overriding is all about giving a specific implementation to the inherited method of parent class.

Static binding is being used for overloaded methods and dynamic binding is being used for overridden/overriding methods.
Performance: Overloading gives better performance compared to overriding. The reason is that the binding of overridden methods is being done at runtime.

Private and final methods can be overloaded but they cannot be overridden. It means a class can have more than one private/final methods of same name but a child class cannot override the private/final methods of their base class.

Return type of method does not matter in case of method overloading, it can be same or different. However in case of method overriding the overriding method can have more specific return type (refer this).

Argument list should be different while doing method overloading. Argument list should be same in method Overriding.

- What are the access modifiers you know? What does each one do?
- Can an Interface extend another Interface?
- What does the `static` word mean in Java?
- Can a `static` method be overridden in Java?
- What is Polymorphism? What about Inheritance?
- What is the difference between an Integer and int?
- Do objects get passed by reference or value in Java? Elaborate on that.
- What is a ThreadPoolExecutor? [Link](https://blog.mindorks.com/threadpoolexecutor-in-android-8e9d22330ee3)
- What the difference between local, instance and class variables?
- What is reflection? [Link](http://tutorials.jenkov.com/java-reflection/index.html)
- What are strong, soft and weak references in Java?
- What is dependency injection? Can you name few libraries? Have you used any?
- What does the keyword `synchronized` mean?
- What does it means to say that a `String` is immutable?
- What are `transient` and `volatile` modifiers?
- What is the `finalize()` method?
- How does the `try{}finally{}` works?
- What is the difference between instantiation and initialization of an object?
- When is a `static` block run?
- Explain Generics in Java?
- Difference between `StringBuffer` and `StringBuilder`?
- How is a `StringBuilder` implemented to avoid the immutable string allocation problem?
- What is Autoboxing and Unboxing?
- What’s the difference between an Enumeration and an Iterator?
- What is the difference between fail-fast and fail safe in Java?
- What is Java priority queue?
- What are the design patterns? [Link](https://github.com/iluwatar/java-design-patterns)


* ​

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
