# Data-Structure-and-Algorithms
Preparation for Interview

## Array
1. 数据结构中有哪些是线性表数据结构？
**What are the linear data structures?**
- Array(static)
- Linked List(dynamic) 
- Stack(dynamic)
- Queue (dynamic)

2. 数组的元素删除和获取，时间复杂度是多少？
**What is the time complexity of array element deletion and retrieval?**

| Operation                | Time Complexity | Explanation                      |
| ------------------------ | --------------- | -------------------------------- |
| **Retrieval (by index)** | O(1)            | Direct access via index          |
| **Delete at end**        | O(1)            | Just remove last element         |
| **Delete at beginning**  | O(n)            | Shift all elements left          |
| **Delete at middle**     | O(n)            | Shift elements after deleted one |
| **Search (unsorted)**    | O(n)            | Check each element               |
| **Search (sorted)**      | O(log n)        | Binary search                    |

3. ArrayList 中默认的初始化长度是多少？
**What is the default initial capacity of ArrayList?**
- Default capacity of ArrayList is 10.

4. ArrayList 中扩容的范围是多大一次？
**How much does ArrayList expand by each time**
- Expands to **1.5× the current capacity**
  
5. ArrayList 是如何完成扩容的，System.arraycopy 各个入参的作用是什么？
**How does ArrayList expand, and what are the parameters of System.arraycopy?**
- If the current capacity is reached, the ArrayList expands its size by approximately 50% of the old capacity, allowing for the addition of new elements without the need for creating a new array.
The resizing process ensures that there is always sufficient space to accommodate new elements, and this is managed internally. - [Scaler](https://www.scaler.com/topics/java/arraylist-in-java/)
- static void	arraycopy(Object src, int srcPos, Object dest, int destPos, int length)	
Copies an array from the specified source array, beginning at the specified position, to the specified position of the destination array. -[Oracle](https://docs.oracle.com/javase/8/docs/api/java/lang/System.html)
- Call it with System.arraycopy(...);

##
