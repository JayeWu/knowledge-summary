## Nosql和关系型数据库的区别

### 1.存储方式

* 关系型数据库是表格式的，因此存储在表的行和列中

*  他们之间很容易关联协作存储，提取数据很方便

*  Nosql数据库则与其相反，他是大块的组合在一起

*  通常存储在数据集中，就像文档、键值对或者图结构



### 2.存储结构

*  关系型数据库对应的是结构化数据，数据表都预先定义了结构

*  虽然预定义结构带来了可靠性和稳定性，但是修改这些数据比较困难

*  Nosql数据库基于动态结构，使用与非结构化数据

*  可以很容易适应数据类型和结构的变化



### 3.存储规范

*  关系型数据库的数据存储为了更高的规范性，把数据分割为最小的关系表以避免重复，减少数据冗余

*  Nosql数据存储在平面数据集中，数据经常可能会重复

*  数据存储成了一个整体，这样整块数据更加便于读写



### 4.存储扩展

*  关系型数据库是纵向扩展，也就是说想要提高处理能力，要使用速度更快的计算机

*  Nosql数据库是横向扩展的，它的存储天然就是分布式的，可以通过给资源池添加更多的普通数据库服务器来分担负载



### 5.查询方式

*  关系型数据库通过结构化查询语言来操作数据库

*  Nosql查询以块为单元操作数据，使用的是非结构化查询语言，它是没有标准的

*  关系型数据库表中主键的概念对应Nosql中存储文档的ID



### 6.事务

*  关系型数据库遵循ACID规则（原子性(Atomicity)、一致性(Consistency)、隔离性(Isolation)、持久性(Durability)）

*  Nosql数据库遵循BASE原则（基本可用（Basically Availble）、软/柔性事务（Soft-state ）、最终一致性（Eventual Consistency））

*  关系型数据库的数据强一致性，所以对事务的支持很好

*  关系型数据库支持对事务原子性细粒度控制，并且易于回滚事务

*  Nosql数据库是在CAP（一致性、可用性、分区容忍度）中任选两项

*  因为Nosql基于节点的分布式系统中，很难全部满足，所以对事务的支持不是很好

