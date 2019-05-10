## JAVA基础
### Java多线程
线程池的原理，为什么要创建线程池？  
线程的生命周期，什么时候会出现僵死进程；  
什么实现线程安全，如何实现线程安全；  
创建线程池有哪几个核心参数？ 如何合理配置线程池的大小？  
synchronized、volatile区别、synchronized锁粒度、模拟死锁场景、原子性与可见性；  
java cas原理
JAVA线程池有哪些参数，如果自己设计一个线程池要考虑哪些问题？
Java的lock的底层实现？
乐观锁和悲观锁？可重入锁和Synchronized？
CountDownLaunch和Cylicbarrior的区别以及分别是在哪样场景下使用的？

### Java扩展
红黑树的实现原理和应用场景；
NIO是什么？适用于何种场景？
NIO了解么，讲一下和BIO的区别，AIO呢。阻塞，非阻塞，异步。具体。
Java9比Java8改进了什么；
HashMap内部的数据结构是什么？底层是怎么实现的？
说说反射的用途及实现，反射是不是很慢，我们在项目中是否要避免使用反射；
说说自定义注解的场景及实现；
List和Map区别，Arraylist与LinkedList区别，ArrayList与Vector 区别；
讲一下ArrayList和linkedlist的区别，ArrayList的扩容方式，扩容时机。
hashmap的实现，以及hashmap扩容底层实现。
常见集合类的区别和适用场景？
如何判断链表是否有环？
平时会用到哪些数据结构？
解决hash冲突的方法有哪些？
讲讲自己对HashMap的理解，以及和Weakhashmap的区别？
concurrentHashMap如何实现？
说说treemap和HashMap的区别？HashMap和ConcurrentHashMap的区别？
HashMap底层如何实现(JDK1.8有所改动)？
说说Hash的一致算法？
阻塞队列不用Java提供的该怎么实现？

### JVM相关
JVM内存模型，GC机制和原理；GC分哪两种；什么时候会触发Full GC？
JVM里的有几种classloader，为什么会有多种？
什么是双亲委派机制？介绍一些运作过程，双亲委派模型的好处；(这个我真的不会...)
什么情况下我们需要破坏双亲委派模型；
常见的JVM调优方法有哪些？可以具体到调整哪个参数，调成什么值？
JVM虚拟机内存划分、类加载器、垃圾收集算法、垃圾收集器、class文件结构是如何解析的；
自定义类加载器怎么实现，其中哪个方法走双亲委派模型，哪个不走，不走的话怎么加载类（实现findclass方法，一般用defineclass加载外部类），如何才能不走双亲委派。（重写loadclass方法）
JAVA的垃圾回收，标记算法和复制算法的区别，用在什么场合？
GC、G1和ZGC的区别？
JVM相关的分析工具有使用过哪些？具体的性能调优步骤吗？
你知道的GC算法和回收策略有哪些？GC的机制是什么？
垃圾回收器的基本原理？是否可以立即回收内存？怎么样主动的通知JVM进行垃圾回收？


### 并发编程
你在项目中怎么用到并发的。
高并发情况下，如何使用线程池
并发juc了解么，有哪些线程安全的list。
并发容器了解哪些？
高并发场景下如何防止死锁，保证数据的一致性？



## Spring
Spring AOP的实现原理和场景；（应用场景很重要）
Spring bean的作用域和生命周期；
Spring Boot比Spring做了哪些改进？ Spring 5比Spring4做了哪些改进；（惭愧呀，我们还在用Spring4，高版本的没关心过）
Spring IOC是什么？优点是什么？
SpringMVC、动态代理、反射、AOP原理、事务隔离级别；
说一下Spring源码把，它的架构，流程。
Spring的bean如果要在实例化过程中修改其某一个成员变量，应该怎么做呢。不通过构造方法，并且AOP也并不能实现。
Spring IOC如何管理Bean之间的依赖关系，怎么样避免循环依赖？
SpringBean创建过程中的设计模式？


## 中间件
Dubbo完整的一次调用链路介绍；
Dubbo支持几种负载均衡策略？
Dubbo Provider服务提供者要控制执行并发请求上限，具体怎么做？
Dubbo启动的时候支持几种配置方式？
了解几种消息中间件产品？各产品的优缺点介绍；
消息中间件如何保证消息的一致性和如何进行消息的重试机制？
Spring Cloud熔断机制介绍；
Spring Cloud对比下Dubbo，什么场景下该使用Spring Cloud？
你说了解Tomcat的基本原理，了解的是哪一部分，基本架构，connector和container
Tomcat的类加载器了解么，回答不了解只了解Java的类加载器。
dubbo的基本架构，几个组件说一下
dubbo的负载均衡怎么做，讲一下具体代码实现。
阿里的dubbo，rocketmq的事务消息的架构设计
mycat实现分表分库方案实现
消息队列kafka和rabbitmq等
分库分表，分片规则hash和取余数。
关于Mina框架了解多少？（因为我在项目里用到了Mina，所以提到了这个部分） netty
多个RPC请求进来，服务器怎么处理并发呢
项目中消息队列怎么用的？使用哪些具体业务场景？
MQ底层原理的实现？



## 数据库篇
锁机制介绍：行锁、表锁、排他锁、共享锁；
乐观锁的业务场景及实现方式；
事务介绍，分布式事物的理解，常见的解决方案有哪些，什么事两阶段提交、三阶段提交；
MySQL记录binlog的方式主要包括三种模式？每种模式的优缺点是什么？
MySQL锁，悲观锁、乐观锁、排它锁、共享锁、表级锁、行级锁；
分布式事务的原理2阶段提交，同步异步阻塞非阻塞；
数据库事务隔离级别，MySQL默认的隔离级别、Spring如何实现事务、
JDBC如何实现事务、嵌套事务实现、分布式事务实现；
SQL的整个解析、执行过程原理、SQL行转列；
数据库万级变成亿级，怎么处理
数据库分库分表一般数据量多大才需要？

mysql数据库默认存储引擎，有什么优点
MySQL的事务隔离级别，分别解决什么问题。
四个表 记录成绩，每个大约十万条记录，如何找到成绩最好的同学
MySQL的慢sql优化一般如何来做？除此外还有什么方法优化？
你理解的BTree机制？
有哪些MySQL常用的优化方法？
说说MySQL的锁并发？加锁的机制是什么？

说说分库与分表设计？
分库分表带来的分布式困境与对应之策有哪些？



## Redis （缓存）
Redis为什么这么快？redis采用多线程会有哪些问题？
Redis支持哪几种数据结构；
Redis跳跃表的问题；
Redis单进程单线程的Redis如何能够高并发?
Redis如何使用Redis实现分布式锁？
Redis分布式锁操作的原子性，Redis内部是如何实现的？
如果Redis有1亿个key，使用keys命令是否会影响线上服务
Redis的持久化方式，aod和rdb，具体怎么实现，追加日志和备份文件，底层实现原理知道吗
如何保证数据库与redis缓存一致的
Redis和Setnx命令使如何实现分布式锁的？使用Redis怎么进行异步队列？会有什么缺点？
缓存击穿的概念和解决方案?
Redis的数据结构？ 线程模型？ Redis的数据淘汰机制？
Redis的数据一致性问题

## 分布式
你说了解分布式服务，那么你怎么理解分布式服务。
docker和虚拟机讲一下。
听说你项目用过docker，讲一下docker的实现原理，说了虚拟机一般要对内核进行虚拟化，docker则用cgroup和namespace分别进行硬件和命名空间的隔离。
集群服务器 如何application 共享？
集群和负载均衡的算法与实现？
讲讲负载均衡的原理？
如何实现高并发环境下的削峰、限流？

## 协议
http和https的区别，http1.x和http2.0的区别，SSL和TSL之间的区别？
Https加密的方式？
Http请求过程，DNS解析的过程？
三次握手和四次握手的过程？


## 算法和数据结构
B+树和B树的区别，和红黑树的区别？
常见的负载均衡算法有哪些
B+树索引和Hash索引之间的区别？

## 服务监控
线上的服务器监控指标，你认为哪些指标是最需要关注的？为什么？

## 其它
布隆过滤器了解么，讲了ip地址过滤的布隆过滤器实现。
参与项目的挑战在哪里，有哪些收获。
双11秒杀的设计思路
请画一个完整大型网站的分布式服务器集群部署图
如何做压测，抗压手段




https://zhuanlan.zhihu.com/p/47167606


https://www.zhihu.com/question/43827750

https://zhuanlan.zhihu.com/p/48195751

https://zhuanlan.zhihu.com/p/48705394

https://zhuanlan.zhihu.com/p/42221907
`_****_`
https://zhuanlan.zhihu.com/p/38131658


