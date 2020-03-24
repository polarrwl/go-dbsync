# dbsync
database sync tools.

## config
config.json file.

1. SrcDB source database config.
2. DesDB destcation database config.
3. DataSync data sync handle config.

eg : 

<p align="center"><img src="doc/config/eg.jpg" alt="eg Logo"></p>


## build
- make install
- make
- make release

## run
./bin/start.sh

## note
dbsync是数据库同步工具,使用go编写，主要特性有
1. 支持数据库种类多(oracle,postgresql,mysql,sqlserver等,其他添加中)
2. 灵活支持自定义SQL,支持多表和视图
3. 支持字段映射,可以配置字段的映射关系
4. 批量操作,性能较高

## benchmark
- 本地虚拟机 centos6 2核2G 
- PostgreSQL 10.6
- mysql 5.1.73

1. insert 117275 条记录 14S TPS 8376/s
2. update 117275 条记录 44S TPS 2665/s

