---
title: Linux Cmd
date: 2019-04-16 20:46:25
categories:
- cmd
tags:
- cmd
---

## 搜索查看
    1. tail -f file|grep --line-buffered xxx
    2. tail -f debug.log | grep --line-buffer
    3. ps -aux | grep tomcat
    4. ps -ef | grep nginx
    5. unzip report-api.war -d report-api
  
    tail -f debug.log | grep --line-buffer EquipmentCkMapper
    
    
    grep "Server port" -rl /koabs/local/tomcat7.0/jekins-inst-inst/conf/server.xml | xargs sed -i "s#shutdown_port#9999#g" 

    "sed -i "s#8080#shutdown_port#g" /koabs/local/tomcat7.0/jekins-inst-inst/conf/server.xml
    
    
    grep -rn "hello,world!" *  // 搜索文件


> chmod -R 777 /home/mypackage
1. -rw------- (600)      只有拥有者有读写权限。
2. -rw-r--r-- (644)      只有拥有者有读写权限；而属组用户和其他用户只有读权限。
3. -rwx------ (700)     只有拥有者有读、写、执行权限。
4. -rwxr-xr-x (755)    拥有者有读、写、执行权限；而属组用户和其他用户只有读、执行权限。
5. -rwx--x--x (711)    拥有者有读、写、执行权限；而属组用户和其他用户只有执行权限。
6. -rw-rw-rw- (666)   所有用户都有文件读、写权限。
7. -rwxrwxrwx (777)  所有用户都有读、写、执行权限。

 ##### 查看磁盘和文件大小
    1. df -h 
    2. du -sh *


## 查看系统环境信息
查看磁盘和文件大小
1. df -h 
2. du -sh *