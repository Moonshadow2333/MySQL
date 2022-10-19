### B+Tree
![](./imgs/b%2Btree.png)

B+Tree 是 B-Tree 的变种，区别在于：
- 所有数据都会出现在叶子节点；
- 叶子节点形成一个单向链表。

MySQL 的 B+Tree 和传统的 B+Tree 略有不同。
#### MySQL 的 B+Tree 索引
![](./imgs/mysql-b%2Btree.png)

在原 B+Tree 的基础上，**增加一个指向相邻叶子节点的链表指针**，就形成了带有顺序指针的 B+Tree，提高区间的访问性能。