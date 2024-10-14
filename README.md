# GeeORM
一款Go语言开发的ORM框架

### 1. database/sql 基础
- SQLite 的基础操作（连接数据库，创建表、增删记录等）。 
- 使用 Go 语言标准库 database/sql 连接并操作 SQLite 数据库，并简单封装。代码约150行

### 2. 对象表结构映射

- 使用 dialect 隔离不同数据库之间的差异，便于扩展。
- 使用反射(reflect)获取任意 struct 对象的名称和字段，映射为数据中的表。
- 数据库表的创建(create)、删除(drop)。代码约150行

### 3. 记录新增和查询

- 实现新增(insert)记录的功能。
- 使用反射(reflect)将数据库的记录转换为对应的结构体实例，实现查询(select)功能。代码约150行

### 4. 链式操作与更新删除

- 通过链式(chain)操作，支持查询条件(where, order by, limit 等)的叠加。
- 实现记录的更新(update)、删除(delete)和统计(count)功能。代码约100行

### 5. 实现钩子

- 通过反射(reflect)获取结构体绑定的钩子(hooks)，并调用。
- 支持增删查改(CRUD)前后调用钩子。代码约50行
