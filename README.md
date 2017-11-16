# PHP-MSF开发手册

PHP微服务框架开发手册，即Micro Service Framework For PHP Develop Manual，PHP微服务框架即[“Micro Service Framework For PHP”](https://github.com/pinguo/php-msf)，是Camera360社区服务器端团队基于Swoole自主研发的现代化的PHP服务框架，简称msf或者php-msf，它的核心设计思想是采用协程、异步、并行的创新技术手段提高系统的单机吞吐能力，降低整体服务器成本。

本手册从介绍异步、并行、协程等基础概念出发，再到[PHP-MSF](https://github.com/pinguo/php-msf)框架如何使用，其中也介绍了部分内部实现的原理，简单易上手。通过学习本手册，再结合我们的demo示例项目，就能够使用[PHP-MSF](https://github.com/pinguo/php-msf)构建大规模高性能的微服务化分布式系统。

```bash
      _______                               ____
________  / /_  ____        ____ ___  _____/ __/
___/ __ \/ __ \/ __ \______/ __ `__ \/ ___/ /_
__/ /_/ / / / / /_/ /_____/ / / / / (__  ) __/
_/ .___/_/ /_/ .___/     /_/ /_/ /_/____/_/
/_/         /_/         Camera360 Open Source TM
```

# 交流与反馈

PHP-MSF#1群(QQ): 614054288

<img src="./images/QR.JPG" title="扫二维码加群" width="40%" />

# 目录

* [1 为什么要研发新的PHP框架](chapter-1/1.0-为什么要研发新的PHP框架.md)
	* [1.1 传统php-fpm工作模式的问题](chapter-1/1.1-传统php-fpm工作模式的问题.md)
	* [1.2 压测数据对比](chapter-1/1.2-压测数据对比.md)
	* [1.3 小结](chapter-1/1.3-小结.md)
* [2 微服务框架研发概览](chapter-2/2.0-微服务框架研发概览.md)
	* [2.1 通信框架技术选型](chapter-2/2.1-通信框架技术选型.md)
	* [2.2 swoole](chapter-2/2.2-swoole.md)
	* [2.3 协程原理](chapter-2/2.3-协程原理.md)
	* [2.4 异步、并发](chapter-2/2.4-异步、并发.md)
	* [2.5 小结](chapter-2/2.5-小结.md)
* [3 框架运行环境](chapter-3/3.0-框架运行环境.md)
	* [3.1 环境变量](chapter-3/3.1-环境变量.md)
	* [3.2 运行代码](chapter-3/3.2-运行代码.md)
	* [3.3 docker](chapter-3/3.3-docker.md)
	* [3.4 小结](chapter-3/3.4-小结.md)
* [4 框架结构](chapter-4/4.0-框架结构.md)
	* [4.1 结构概述](chapter-4/4.1-结构概述.md)
	* [4.2 控制器](chapter-4/4.2-控制器.md)
	* [4.3 模型](chapter-4/4.3-模型.md)
	* [4.4 视图](chapter-4/4.4-视图.md)
	* [4.5 同步任务](chapter-4/4.5-同步任务.md)
	* [4.6 配置](chapter-4/4.6-配置.md)
	* [4.7 路由](chapter-4/4.7-路由.md)
	* [4.8 小结](chapter-4/4.8-小结.md)
* [5 框架组件](chapter-5/5.0-框架组件.md)
	* [5.1 协程](chapter-5/5.1-协程.md)
	* [5.2 类的加载](chapter-5/5.2-类的加载.md)
	* [5.3 异步HttpClient](chapter-5/5.3-异步HttpClient.md)
	* [5.4 请求上下文](chapter-5/5.4-请求上下文.md)
	* [5.5 连接池](chapter-5/5.5-连接池.md)
	* [5.6 对象池](chapter-5/5.6-对象池.md)
	* [5.7 RPC](chapter-5/5.7-RPC.md)
	* [5.8 公共库](chapter-5/5.8-公共库.md)
	* [5.9 RESTful](chapter-5/5.9-RESTful.md)
	* [5.10 多语言](chapter-5/5.10-多语言.md)
	* [5.11 小结](chapter-5/5.11-小结.md)
* [6 常见问题](chapter-6/6.0-常见问题.md)
* [7 附录](chapter-7/7.0-附录.md)

# links
  * 下一节: [为什么要研发新的PHP框架](chapter-1/1.0-为什么要研发新的PHP框架.md)
