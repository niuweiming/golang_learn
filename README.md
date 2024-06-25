# Golang学习路线

#### GO安装

https://golang.google.cn/dl/

##### 环境配置:

编译器:

建议选择GoLand对于新手比较友好

[【七天入门Go语言】Goland && Golang 的安装与配置 | 第一天_go and golang-CSDN博客](https://blog.csdn.net/weixin_45304503/article/details/119295577)





#### 基础

常量  const

变量   var

##### 数据类型

基础类型: 

int  float  string bool array 

其他类型:

slice 基础扩容

map 基础扩容

struct 

chan 

interface

##### 流程控制

if else 

switch case

select case 

defer  defer原理

goto 

recover 

panic

os.Exit 

break

##### 函数

有名函数

匿名函数

##### 命令行

go build  

go run  

go get  

go install 



#### 项目构建

包管理:

go mod   go mod init   go mod tidy 

代码风格:

go fmt 

代码文档

swagger(可以不学)



#### 高级特性

##### GC 三色标记

##### 反射

##### 内存管理

##### 并发编程

goroutine 调度  GMP调度

waitgroup

chan 

mutex

once

sync.map

##### Context

CGO

unsafe



#### 优化

###### 逃逸分析

###### GC优化

###### 池化sync.pool

###### 内存分配模型

对齐方式

填充方式

减少内存拷贝





#### 实战用到的第三方包

fasthttp替换net/http

json-iterator替换json

mysql 相关 gorm 

es相关 github.com/olivere/elastic

mq相关:

Kafka相关  github.com/Shopify/sarama

recketmq相关 github.com/apache/rocketmq-client-go/v2

rabbitmq相关 github.com/stradway/amqp

redis相关:

github.com/go-redis/redis

配置相关

yaml   gopkg.in/yaml.v2

toml   github.com/BurntSushi/toml



#### 常用包

math 

net/http

fmt

io

csv

json

time

strconv

strings



#### 问题排查

trace  查频繁gc

pprof 内存泄漏   cpu过高  程序慢  锁的争用 程序阻塞



####　框架

gin  beego (挑一个学就行,推荐gin 好上手)

go-zero



#### 中间件

mysql 

redis 

消息队列 {kafka recketMQ rabbitMQ}

MongoDB

Nginx



#### 工程能力

docker 

k8s

微服务 

操作系统

分布式



#### 推荐项目

推荐先写一个小的练手项目

B站--https://www.bilibili.com/video/BV1Xi421Z72A

看一遍基本上就了解前后端之间的关系,以及掌握crud技巧

这是我写好的代码--[niuweiming/vote_project: 投票项目 (github.com)](https://github.com/niuweiming/vote_project)

或者是 写一个备忘录

[CocaineCong/TodoList: Gin+Gorm+Redis+Swagger 基于 RESTful API 规范搭建备忘录，包括redis缓存，swagger文档，docker部署 (github.com)](https://github.com/CocaineCong/TodoList)

https://www.bilibili.com/video/BV1GT4y1R7tX/



下面就是进阶一点的项目

微服务的备忘录

[CocaineCong/micro-todoList at v2 (github.com)](https://github.com/CocaineCong/micro-todoList/tree/v2)

https://www.bilibili.com/video/BV1h44y1L7LN/



关于秒杀问题解决方案

https://github.com/CocaineCong/Go-SecKill.git



做一个即时通信

[CocaineCong/gin-chat-demo: gin+websocket+mongodb实现 IM 即时聊天系统，基于WS连接的即时聊天，支持单聊，在线回复以及历史记录查询 (github.com)](https://github.com/CocaineCong/gin-chat-demo)

https://www.bilibili.com/video/BV1BP4y1H7gV





这些项目学完基本上大体已经对后端各种框架技术有一个很好的掌握了

后端技术栈

go+gorm+gin+mysql+redis+kafka+websocket+mongoDB

云原生技术栈

go+docker+k8s