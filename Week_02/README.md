## HashMap
### 特点
    - 使用哈希表进行数据存储，使用链地址法来解决冲突
    - 当链表长度大于等于 8 时，将链表转换为红黑树来存储
    - 每次进行二次幂的扩容
### 属性
    - Node[] table：存储数据的哈希表；初始长度 length = 16（DEFAULT_INITIAL_CAPACITY），扩容时容量为原先的两倍（n * 2）
    - final float loadFactor：负载因子，确定数组长度与当前所能存储的键值对最大值的关系；不建议轻易修改，除非情况特殊
    - int threshold：所能容纳的 key-value 对极限 ；threshold = length * Load factor，当存在的键值对大于该值，则进行扩容
    - int modCount：HashMap 结构修改次数（例如每次 put 新值使则自增 1）
    - int size：当前 key-value 个数
### 构造函数
    - 无参构造，初始容量默认16，负载因子默认0.75
    - 指定初始容量，负载因子默认0.75
    - 指定初始容量和负载因子
    - 通过传入的map构造
