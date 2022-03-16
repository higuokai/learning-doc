### HashMap、HashTable、ConcurrentHashMap

1. #### HashMap

   1. HashMap数据结构

      ​		HashMap是一个数组和链表的复合结构。链表被分成一个个桶， 初始化数组长度为16, 默认负载因子0.75, 扩容时扩容为上一次的2倍，同一个数组元素中的链表/树元素的hashCode对桶长度取模值是相同的。

      ​	hashMap 元素个数超过  数组长度 * 负载因子(默认16*0.75=12)的时候, 会扩容。代表分配不均匀了。