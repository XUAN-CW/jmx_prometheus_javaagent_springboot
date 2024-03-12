

# 运行方式

## 下载 jmx_prometheus_javaagent-0.20.0.jar

https://github.com/prometheus/jmx_exporter/releases/tag/0.20.0



## 编写配置文件

 [simple-config.yml](config\simple-config.yml) 

## 添加启动参数

```
-javaagent:C:\core\java\demo\jmx_prometheus_javaagent_springboot\config\jmx_prometheus_javaagent-0.20.0.jar=30100:C:\core\java\demo\jmx_prometheus_javaagent_springboot\config\simple-config.yml 
```
```
-javaagent:/Users/xuanchengwei/my-data/core/java/demo/jmx_prometheus_javaagent_springboot/config/jmx_prometheus_javaagent-0.20.0.jar=30100:/Users/xuanchengwei/my-data/core/java/demo/jmx_prometheus_javaagent_springboot/config/simple-config.yml 
```


```

C:\core\java\demo\jmx_prometheus_javaagent_springboot\config\simple-config.yml 表示 JMX Exporter 的配置文件
```

1. `javaagent:C:\core\java\demo\jmx_prometheus_javaagent_springboot\config\jmx_prometheus_javaagent-0.20.0.jar=30100` 表示 JMX Exporter 的代理端口为30100
2. `C:\core\java\demo\jmx_prometheus_javaagent_springboot\config\simple-config.yml` 表示 JMX Exporter 的配置文件

IDEA可以在这里添加：

![image-20240311224756873](assets/images/image-20240311224756873.png)

## 启动

添加完参数后直接启动即可

## 访问

http://localhost:30100/

## 参考

 [JMX Exporter 规则编写教程.html](assets\references\JMX Exporter 规则编写教程.html)

 [linux上使用JMX Exporter结合prometheus.html](assets\references\linux上使用JMX Exporter结合prometheus.html) 











