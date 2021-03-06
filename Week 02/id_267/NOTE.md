# W02.第5节.哈希表、映射、集合

## 哈希表

散列方法：
    选取某个函数，依据该函数按关键字计算元素的存储位置，并按此存储；
    查找时，由同一个函数，对给定值k计算存储地址，将k于地址单元中元素关键码进行比较，确定查找是否成功。查找的时间复杂度为O(1)

散列函数（Hash函数）：
    散列方法中使用的转换函数。

散列表(Hash表)：
   按照散列方法构造的表

冲突：
     不同的关键码映射到同一个散列地址

散列表来源于数组，它借助散列函数对数组这种数据结构进行扩展，利用的是数组支持按照下标随机访问元素的特性。散列表两个核心问题是散列函数设计和散列冲突解决。散列冲突有两种常用的解决方法，开放寻址法和链表法。散列函数设计的好坏决定了散列冲突的概率，也就决定散列表的性能。

由于计算机内存的不断加大，我们可以认为Hash表的增删改查的时间复杂度为O(1)，实际最坏复杂度为O(n)

## 映射(map/dict)、集合(set)

在真正的工程代码里面经常使用的不再是哈希表，而是在哈希表的基础上抽象出来的。使用比较多的就是map和set。

map: 键值对，key不重复。
set: 不重复元素的集合

