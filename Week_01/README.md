学习笔记

一数组（Array）是一种线性表数据结构。它用一组连续的内存空间，来存储一组具有相同类型的数据。其特点有两点：
第一是线性表（Linear List）。顾名思义，线性表就是数据排成像一条线一样的结构。每个线性表上的数据最多只有前和后两个方向。
第二个是连续的内存空间和相同类型的数据。
数组最基础、最简单的数据结构。用一块连续的内存空间，来存储相同类型的一组数据，最大的特点就是支持随机访问，
但插入、删除操作也因此变得比较低效，平均情况时间复杂度为 O(n)。

二链表  比较数组需要一块连续的内存空间来存储，对内存的要求比较高，链表恰恰相反，它并不需要一块连续的内存空间，
它通过“指针”将一组零散的内存块串联起来使用。三种最常见的链表结构它们分别是：单链表、双向链表和循环链表。
单链表的插入与删除操作是O(1)时间复杂度。但是为了查找到值等于给定值的结点，都需要从头结点开始一个一个依次遍历对比，
直到找到值等于给定值的结点，尽管单纯的删除操作时间复杂度是 O(1)，但遍历查找的时间是主要的耗时点，对应的时间复杂度为 O(n)。
根据时间复杂度分析，删除值等于给定值的结点对应的链表操作的总时间复杂度为 O(n)，链表可以用于实现LRU缓冲淘汰算法。

三栈 栈是后进者先出，先进者后出的数据结构，栈既可以用数组来实现，也可以用链表来实现。用数组实现的栈，我们叫作顺序栈，用链表实现的栈，叫作链式栈。
它的最大特点是只支持入栈和出栈操作，它是一种操作受限的数据结构。当某个数据集合只涉及在一端插入和删除数据，并且满足后进先出、先进后出的特性，
可以首选“栈”这种数据结构。函数的调用就是用栈来保存临时变量的，因为函数调用符合后进先出的特性。常见应用递归，写递归，最重要是写出递推公式，
找出终止条件。

四队列 队列象成排队买票，先来的先买，后来的人只能站末尾，不允许插队。它是一种先进者先出的数据结构。队列跟栈非常相似，支持的操作也很有限，
最基本的操作也是两个：入队 enqueue()，放一个数据到队列尾部；出队 dequeue()，从队列头部取一个元素。队列可以用数组来实现，也可以用链表来实现。
用数组实现的栈叫作顺序栈，用链表实现的栈叫作链式栈。同样，用数组实现的队列叫作顺序队列，用链表实现的队列叫作链式队列。常用的循环队列定义需要确定好
队列为空和队列满的判断条件。