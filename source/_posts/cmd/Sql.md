---
title: Sql Cmd
date: 2019-04-16 20:46:25
categories:
- cmd
tags:
- cmd
---

## mysql 排错
1. 执行过程查看
```
show processlist;  
show variables like '%profil%';  
set profiling = 1;  
show profiles;  
show profile for query 4;

```
2. 死锁和结束死锁
```
1、查询是否锁表
show open tables where in_use>0;
 
2、查询进程
show processlist
查询到相对应的进程，然后 kill id
 
3、查看正在锁的事务
select * from information_schema.innodb_locks; 
 
4、查看等待锁的事务
select * from information_schema.innodb_lock_waits;

5、分析死锁 -- information_schema.INNODB_TRX 

6、查看死锁日志
SHOW ENGINE INNODB STATUS;

```
3. 慢日志查询分析
```

```