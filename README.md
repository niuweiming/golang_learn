# Golang学习路线

#### GO安装

https://golang.google.cn/dl/

##### 环境配置:

编译器:

建议选择GoLand对于新手比较友好

[GoLand安装与环境配置_goland配置环境-CSDN博客](https://blog.csdn.net/weixin_40563757/article/details/115476327?ops_request_misc=%7B%22request%5Fid%22%3A%22171924045516800213024036%22%2C%22scm%22%3A%2220140713.130102334..%22%7D&request_id=171924045516800213024036&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduend~default-2-115476327-null-null.142^v100^pc_search_result_base1&utm_term=go ： GoLand安装及环境配置&spm=1018.2226.3001.4187)



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