# GeeORM
一款Go语言开发的ORM框架

### 1. database/sql 基础
- SQLite 的基础操作（连接数据库，创建表、增删记录等）。 
- 使用 Go 语言标准库 database/sql 连接并操作 SQLite 数据库，并简单封装。代码约150行

### 2. 对象表结构映射

- 使用 dialect 隔离不同数据库之间的差异，便于扩展。
- 使用反射(reflect)获取任意 struct 对象的名称和字段，映射为数据中的表。
- 数据库表的创建(create)、删除(drop)。代码约150行
