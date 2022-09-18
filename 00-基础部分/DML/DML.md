### DML
#### DML介绍
DML英文全称为 `Data Manipulation Language`（数据库操作语言），用来对数据库中的表数据记录进行增删改操作。
- 添加数据；
- 修改数据；
- 删除数据。

#### 添加数据
向表中指定字段添加一条数据
```
INSERT INTO 表名(field1,field2,...,fieldn) VALUES(val1,val2,...,valn);
```
给全部字段添加数据
```
INSERT INTO 表名 VALUES(val1,val2,...,valn);
```
批量添加数据
```
INSERT INTO 表名(field1,field2,...,fieldn) VALUES(val1,val2,...,valn),(val1,val2,...,valn)[,(val1,val2,...,valn)];
```
**注意：**
- 顺序一致：添加数据时，指定字段顺序需要与值的顺序一一对应；
- 字符串和日期类型的数据应该包含在引号中；
- 不能越界：添加的数据大小，应该在字段的规定范围内。

#### 更新数据
```
UPDATE 表名 SET field1 = val1,field2 = val2 [WHERE条件];
```
注意：
- 可以一次更新一个字段的值，也可以一次更新多个字段的值，字段与字段用逗号隔开；
- 有 `where` 条件时，更新 `where` 条件的数据，没有则更新表中所有的数据。
  
#### 删除数据
```
DELETE FROM 表名 [WHERE条件];
```
注意：有 `where` 条件时，删除 `where` 条件的数据，没有则删除表中所有的数据。