<p align="center">
    <img src="https://raw.githubusercontent.com/xuxueli/xxl-job/master/doc/images/xxl-logo.jpg" width="150">
    <h3 align="center">XXL-CONF | 分布式配置管理平台</h3>
    <p align="center">
        XXL-CONF, A distributed configuration management platform.
        <br>
        <a href="http://www.xuxueli.com/xxl-conf/"><strong>-- Home Page --</strong></a>
        <br>
        <br>
        <a href="https://travis-ci.org/xuxueli/xxl-conf">
            <img src="https://travis-ci.org/xuxueli/xxl-conf.svg?branch=master" >
        </a>
        <a href="https://maven-badges.herokuapp.com/maven-central/com.xuxueli/xxl-conf/">
            <img src="https://maven-badges.herokuapp.com/maven-central/com.xuxueli/xxl-conf/badge.svg" >
        </a>
         <a href="https://github.com/xuxueli/xxl-conf/releases">
             <img src="https://img.shields.io/github/release/xuxueli/xxl-conf.svg" >
         </a>
         <a href="http://www.gnu.org/licenses/gpl-3.0.html">
             <img src="https://img.shields.io/badge/license-GPLv3-blue.svg" >
         </a>
    </p>    
</p>

## Introduction
XXL-CONF is a distributed configuration management platform, provide uniform configuration management for distributed systems.  
Now, it's already open source, real "out-of-the-box".

XXL-CONF 是一个分布式配置管理平台，提供统一的配置管理服务。现已开放源代码，开箱即用。

## Documentation
- [中文文档](http://www.xuxueli.com/xxl-conf/)

## Features
- 1、简单: 提供简洁实用的API，上手简单；
- 2、在线管理: 提供配置中心, 通过Web界面在线操作配置数据;
- 3、动态推送更新: 配置更新后, Zookeeper实时推送配置信息, 项目中配置数据会实时更新并生效, 不需要重启线上机器;
- 4、高性能: 底层通过Ehcache对ZK推送的配置做Local Cache, 提高性能;
- 5、客户端断线重连强化：除了依赖ZK之外，设置守护线程，提高异常情况下配置时效性；
- 6、配置备份: 配置数据同时在ZK与MySQL中存储和备份， 提高配置数据的安全性;
- 7、HA: 配置服务基于ZK集群, 只要集群节点保证存活数量大于N/2N+1, 就可保证服务稳定, 避免单点风险;
- 8、分布式: 支持多业务线接入并统一管理配置信息，支撑分布式业务场景;
- 9、分组隔离: 支持对配置进行分组管理, 方便隔离不同业务线配置;
- 10、多种配置方式：支持 "API、 @XxlConf、XML" 三种配置方式；
- 11、配置变更监听功能：可开发Listener逻辑，监听配置变更事件，可据此动态刷新JDBC连接池等高级功能；
- 12、空配置处理：主动缓存null或不存在类型配置，避免配置请求穿透到ZK引发雪崩问题；


## Communication

- [社区交流](http://www.xuxueli.com/page/community.html)


## Contributing
欢迎参与项目贡献！比如提交PR修一个bug，或者新建 [Issue](https://github.com/xuxueli/xxl-conf/issues/) 讨论新特性或者变更。

## 接入登记
更多接入的公司，欢迎在 [登记地址](https://github.com/xuxueli/xxl-conf/issues/2 ) 登记，登记仅仅为了产品推广。

## Copyright and License
产品开源免费，并且将持续提供免费的社区技术支持。个人或企业内部可自由的接入和使用。

- Licensed under the GNU General Public License (GPL) v3.
- Copyright (c) 2015-present, xuxueli.

---
## Donate
无论捐赠金额多少都足够表达您这份心意，非常感谢 ：）      [前往捐赠](http://www.xuxueli.com/page/donate.html )

