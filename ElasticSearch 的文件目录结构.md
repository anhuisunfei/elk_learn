  
## ElasticSearch 的文件目录结构

|目录|配置文件|描述|
|:---|---|:---|
|bin|   |脚本文件，包括启动elasticsearch,安装插件。运行统计数据等|
|config|elasticsearch.yml| 集群配置文件，user, role based 相关配置|
|JDK |   | JAVA 运行环境 |
|data | path.data | 数据文件 |
|lib  |     | java 类库|
|logs | path.log | 日志文件 |
|modules |  | 包含所有ES模块 |
|plugins |  | 包含所有已安装插件|


## 插件安装
``` bash
 .\bin\elasticsearch-plugin.bat list
 .\bin\elasticsearch-plugin.bat install analysis-icu
```


## 多实例运行

```
.\bin\elasticsearch.bat -E node.name=node1 -E cluster.name=test -E path.data=node1_data -d
```