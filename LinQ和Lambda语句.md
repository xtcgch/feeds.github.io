#LinQ和Lambda语句
[TOC]

---

##LinQ
命名空间：System.LinQ
表达式：
>int[] numbers = {1,2,3,4,5,6};
>var numQuery1 = from num in numbers where num%2 == 0 orderby num select num;

特点：以语句的形式使用，在真正使用到numQuery1时才会执行该查询语句
优点：在全是**对象**的集合中进行查询

---

##Lambda
命名空间：默认引入
表达式：
>int[] numbers = {1,2,3,4,5,6};
>var numQuqry2 = numbers.Where(n=>n%2 == 0).OrderBy(n=>n);

特点：以方法的形式使用