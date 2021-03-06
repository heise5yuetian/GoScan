# GoScan
> GoScan是采用Golang语言编写的一款分布式综合资产管理系统，适合红队、SRC等使用。

> 该项目是自己空余时间所写，进度较慢；特公开源代码，有能力的人可以二次开发。

> 示例：http://112.74.169.239:9999/  admin/admin888@A  请不要进行增删改

### 一、开发进度

2021.02.1

```
1、更换web框架，不使用gin框架

2、优化端口扫描、新增子域名探测模块、web指纹探测模块(所有模块都为go写，不调用三方组件)

3、web指纹探测模块 指纹规则为json格式，支持自定义添加

4、添加扫描引擎，配置信息统一下发到客户端

5、消息队列nsq采用两组，避免消息流过大及单点故障

6、新增综合扫描（一条龙服务）
```

2021.01.03

```
1、Web框架整体完成：

后台管理：用户登录、添加用户、登录锁定、删除用户、日志管理、消息通知设置（邮件、server酱）等

实用功能：杀毒进程检测、分布式端口扫描

2、客户端：

端口扫描：采用golang开发端口扫描器（Syn探测+精简服务指纹库）
```

### 二、部署教程
> 项目分为web和client端，web端需要postgresql数据库，详情参考：https://github.com/CTF-MissFeng/GoScan/tree/1f51fd92805fa4468333b117a44610ed53edd4ba


### 三、演示

![index](https://github.com/CTF-MissFeng/GoScan/blob/main/doc/1.png)

![index](https://github.com/CTF-MissFeng/GoScan/blob/main/doc/2.png)

![index](https://github.com/CTF-MissFeng/GoScan/blob/main/doc/3.png)

![index](https://github.com/CTF-MissFeng/GoScan/blob/main/doc/4.png)
