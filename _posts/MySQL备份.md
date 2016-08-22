### MySQL备份还原

---
layout: post
title:  "mySql备份还原"
date:   2016-08-22 19:18:23 +0800
categories: [mysql]
---

#### 备份:

1. 使用mysqldump命令备份
   ```
   --mysqldump备份数据库的基本如法格式如下:
   mysqldump -u user -h host -p dbname[tbname,[tbname..]] >filename.sql
   ```
   其中:   
   user表示用户名称;  
   host表示登陆用户的主机名称;    
   dbname为需要备份的数据库名称;  
   tbname为dbname数据库中需要备份的数据表，可以制定多个需要备份的表;  
   filename.sql为备份文件.  

2. 直接拷贝mysql的数据目录。这样很直接，但在执行前最好执行lock table，flush tables.对INNODB不适用。
3. 使用mysqlhotcopy工具备份.只适用于MyISAM和ACHIVE表  
   ```
   mysqlhotcopy db_name_1,..db_name_n /path/to/new_directory
   -- 其中db_name1,..db_name_n分别为需要备份的数据库的名称./path/to/new_directory指定备份文件目录。
   ```


#### 还原:
1. 使用mysql命令还原  
   `
   mysql -u user -p [dbname] <filename.sql
   `  
   user 是指定登陆的用户.    
   dbname 数据库名称，如果我们备份的是数据库，并且包括数据库的创建语句，则不需要指定数据库名。

2. 直接复制到数据库目录/data。此方法只对MyISAM有效。
3. mysqlhotcopy快速恢复，也是将mysqlhotcopy的文件复制到/data目录，然后重新启动数据库.  

