全民k ge 一面：   
C/C++ 内存管理的问题有遇到过吗？  
深拷贝和浅拷贝区别？  
浅拷贝可能有什么问题？  
智能指针相关问题？  
智能指针的实现？  
智能指针的作用？  
HashMap Map区别？  
什么情况使用hashMap ,  什么情况使用map  
hashMap 什么情况下会冲突， 冲突怎么解决？  
解决哈希冲突的拉链法，如果链太长了会有什么影响？ 怎么解决链太长的问题？  
mysql, redis 有用过吗？  
分布式理论， 集群，负载均衡了解吗？  
三次握手涉及两个队列，半连接队列和全连接队列，他们的作用？  
为什么要三次握手？  
SYN攻击(DDOS攻击)是怎么产生的？ 有什么规避方案？  
还了解其他的一些网络攻击吗？  
有遇到过运营商劫持吗？  
select/poll/epoll 区别？ 进化历程  
epoll收到请求和收到数据的时候处理有什么不同吗？  



shopee一面：  
介绍一下自己，人脸抓拍工程服务端的架构？  
两个栈怎样实现一个队列？ pop方法怎么实现？  
找文件中出现次数最多的前K个单词？ 有哪几种堆？ 用哪一个堆？ 时间复杂度是怎样的？  
数据库用过哪一些？mysql用过吗？  
mysql有哪些存储引擎？  
innodb 有什么特点？  
四个隔离级别？  
Redis有哪些数据结构？  
用过哪些中间件？  
tcp是怎么保证传输的可靠性的？  
拥塞避免是怎么做的？  
tcp粘包了解吗？  
tcp keep-alive 机制了解吗？怎么实现的？  
进程、线程、协程的概念了解吗？  
进程与线程之间的区别？进程与线程之间通信方式有什么区别？  
进程间有哪些通信方式？  
epoll了解吗？是怎么实现的？怎么注册回调的，底层数据结构了解吗？  
epoll有哪些触发机制？  
epoll和selet的区别？  
leetcode第三题， 求字符串中最长不重复子串的长度

TEG 腾讯一面  
第一个个项目设计上的思路和细节？  
加密算法有什么考量？ AES里面CBC和ECB这几种模式，具体有没有考虑选择哪种模式？ 有没有考虑过中间的数据即使被加密也有被攻击的风险， 比如重放攻击？  
有了解过证书里面的非对称算法？ RSA算法的思路？  
C/C++  
有没有了解C11, 14, 17？  

inline 内联为什么快？实际放开了什么？ 递归函数加inline会发生什么，编译器会怎么做？  

.a进行链接可执行程序，不同的.a之间内联？有没有一些机制做到？链接时优化-flto  

11之后的移动语言，move 和右值引用  

有没有并发的开发， 线程与进程的区别？ 对于线程和进程linux是怎么实现的？是系统调度线程吗？ 线程之间的调度需要进内核态吗？  

在C++里面怎么实现协程？  

有了解过内存屏障吗？无锁的实现用的内存屏障的原理？解决什么问题？  

函数的返回值返回一个比较大的结构体， 性能有没有损耗？如果return 指针，内存管理怎么做呢？ 如果用静态变量用多线程怎么办？  

算法：  
平衡二叉排序树，找到里面的最小值。  
平衡二叉树平均时间复杂度  
从小到大遍历一遍，整个时间复杂度是多少？  
n x log n  
取第k小的值， 复杂度是多少？  
无序数据找第k小，有没有什么算法？ 有没有O（N）的算法？ 堆， 快排选节点的算法  

操作系统：  
numa 有没有了解  


计算机网络：  
select, poll , epoll 实现思路？  
tcp拥塞控制存在的意义？不遵循这套机制，有什么收益吗？ 
tcp拥塞控制算法基于丢包的拥塞控制算法， 
有没有了解过新的拥塞控制算法？QUIC？  bbr拥塞算法实现？

tcp拥塞控制的缺点，bbr的优点  
https://cloud.tencent.com/developer/article/1482633  
http://kquic.com/2020/06/08/bbr%E5%9C%A8%E5%AE%9E%E6%97%B6%E9%9F%B3%E8%A7%86%E9%A2%91%E9%A2%86%E5%9F%9F%E7%9A%84%E5%BA%94%E7%94%A8/  
RTprop 链路的物理时延
BtlBW 
Bottleneck Bandwidth and Round-trip propagation time  瓶颈带宽和往返传播时间  
BBR对所谓的“长肥网络”（带宽延迟积大、丢包率高的网络）非常有效  
探测最大带宽和最小延时， 
BBR 优缺点：
缺点： BBR在丢包率达到25%以上，吞吐量会断崖式下降  
BBR的最小RTT有个10s超时时间，在10s超时后，进入ProbeRTT 状态，并持续最小200ms，此状态下，为了排空拥塞，inflight只允许有4个包，这会导致音视频数据在这段时间内堆积在发送队列中，使得时延增加。  

迅雷一面： 



字节一面：
嵌入式开发和非嵌入式开发的区别？  
你了解哪些设计模式？  
设计模式分为几类  
构建型模式， 结构性模式，行为型模式）  
观察者模式适合什么样的场景？  
为什么要使用设计模式？  

TCP怎么保证可靠传输？  
滑动窗口在里面用来做什么？  
TCP是怎么做拥塞控制，整个流程是怎样？  
C++用的哪个版本？  
智能指针有哪些？有哪些区别？  
unique, share, weak   

多线程怎么怎么做并发控制？有哪些锁？互斥，读写，自旋， 有什么区别  
原子变量用过吗？ atomic原子变量  

有没有用过存储的组件，数据库，redis  
redis有哪些数据结构？   
一般用redis来做什么？如果用来做发布订阅为什么不直接用消息队列？  
用过的集合类有哪些？  
一堆学生信息，用快速查找，用什么结构， unordered_map， unordered_map怎么扩容  
local cache怎么实现？ 双向链表 + unordered_map  



# interviewrecode
