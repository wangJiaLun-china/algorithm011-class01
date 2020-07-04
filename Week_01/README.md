## Queue
   - 队列是一种比较特殊的线性结构。
  -  它只允许在表的前端（front）进行删除操作，而在表的后端（rear）进行插入操作。
  - 队列中最先插入的元素也将最先被删除，对应的最后插入的元素将最后被删除。
  - 队列又称为“先进先出”（FIFO—first in first out）的线性表，与栈(FILO-first in last out)相反
###  接口方法
    boolean add(E e)
    向队列中添加元素
    E element()
    返回队列的头，且不移除
    boolean offer(E e)
    向队列中添加元素
    E peek()
    返回队列的头，且不移除
    E poll()
    返回队列的头，且移除
    remove()
    返回队列的头，且移除
##  Stack
 - 限制仅在表的一端进行插入和删除运算的线性表。
 - 栈为后进先出（Last In First Out）的线性表，简称为LIFO表。
 ###  接口方法
     boolean empty()
     判断栈是否为空
     E peek()
     返回栈顶对象，不移除
     E pop()
     返回栈顶对象，并移除
     E push(E item)
     压入栈顶
     int search(Object o)
     返回对象在栈的位置