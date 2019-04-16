---
title: WEB常用技术总结
date: 2019-01-02 20:46:25
categories:
- summary
tags:
- summary
---

#### 后台

---

##### 代码生成
https://github.com/guozilanTK


##### 应用框架
######  开发框架
1. SpringBoot2

###### 分布式服务
1. SpringCloud 系列
2. Dubbo
3. ice


###### 反编译
1. ghidra


##### 测试运维

##### 监控可视化
1. Grafana
2. InfluxDB(时序数据库)

###### 环境
1. Docker
2. Kubernetes

###### 发布 && 基础服务
1. jenkins
2. git && gitlab

###### 代码质量检测
1. Sonar(SonarQube)


##### 数据存储
1. mysql
2. mongodb
3. hbase

##### 中间件
1. RocketMQ, Kafka ...
2. canal && otter
3. mycat 
4. redis
5. 大数据量定时消息通知(支持回撤)

##### 大数据处理
1. greenplum
2. hadoop
3. spark
> 适用范围和分析流程

##### 测试工具
1. Selenium    
2. loadrunner   
3. jmeter  
4. Robot Framework  

> 相关github:   
https://github.com/xiaozi0lei/teslaX    
https://github.com/mzky/easyNmon    
https://github.com/mengde0077/RF-auto-test-demo 
https://github.com/hagyao520/JMeter 




#### 前端

---

##### 基础框架
1. [Vue](https://cn.vuejs.org/v2/guide/) 
2. react
3. Jquery(用的比较少了)

##### 自动化构建工具
1. webpack
2. [glup](https://www.gulpjs.com.cn/)

##### 开发流程
1. 定义前后端交互接口文档

2. 接口管理平台API mock数据开发
> [doclever](http://www.doclever.cn/controller/index/index.html)  
[swagger](https://www.baidu.com/link?url=lfnOzcSpgjqojhyVeDSRiJEpmqqxoOg0borGLOnRJV3&wd=&eqid=f80127f00002cc50000000065b69875a)
3. 本地代理访问mock接口数据
> [Vue-cli](https://segmentfault.com/a/1190000011007043)   
Nginx

4. 前后端联调测试

##### 部署上线
部署在Nginx 等静态服务器中


