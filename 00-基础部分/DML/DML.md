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