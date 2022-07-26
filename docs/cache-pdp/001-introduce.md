# 001. 课程介绍以及高并发高可用复杂系统中的缓存架构有哪些东西
[[toc]]

## 现在常见的 java 工程师/架构师对缓存技术的了解和掌握程度
我常年在一些国内最大的那些互联网公司里负责招人，java 这块我们也会招，各种各样的人我都见过

比如大型的互联网公司的人，传统行业的一些人，初级的人，高阶的架构师，高级工程师，技术经理，技术总监，带几十个人

缓存技术，并不是使用 redis 简简单单的存进去取出来，在复杂的场景的时候，就会出现复杂的缓存架构

工作中都会用到一些缓存技术，redis/memcached 基础使用，初步的集群知识

我面试过的人里，能掌握到很少的缓存架构的人，屈指可数（个位数），而且都是在大公司有过类似的大型复杂系统架构经验的人

## 缓存架构/技术掌握的不够，对你的发展带来了哪些阻碍？

> 工作中

如果你这块技术掌握不够，然后你的公司的项目遇到了一些相关的难题，高并发+高性能的场景，hold 不住类似的这种高并发的系统

因为缓存架构做得不好，不到位，实际在公司的项目里，出了一些大 case，导致系统崩溃，造成巨大的经济损失

> 职业发展中

我面试过的人中有在简历上写了 redis、memcached、activemq、zookeeper、kafka、lucene、activiti、爬虫等等，各种技术写了都几十种技术

没有一样是精通的，redis 就会简单的操作，memcached、activemq、zookeeper、爬虫等全都是简单的操作

叫你说一下架构设计思路，有没有一些考量的点，高并发的中场景，高可用的场景，说不出来

如果是这样的话，那么你不太可能做到更高级的一个职位了，因为很多公司的人也不傻，技术一看就平平庸庸，怎么给你一个很好的职位呢？职业发展怎么做上去呢？

那么就需要你具备亮点：技术亮点，高人一筹

当你去面试 java 高工、java 资深工、java 架构的时候，有技术亮点，在某些方面有一些造诣，如果你的技术很牛，各种技术都有深度，架构面临过一些复杂的场景，别人搞不定的高并发高可用的系统架构，你都能搞定，职业发展就会做的很好

## 课程的一个简单的介绍

亿级流量电商网站的商品详情页系统，项目实战、业务背景，当然不可能是一个完完全全系统，会简化，把要讲的东西贯穿起来，学习到亿级流量的电商网站商品详情页的整体架构设计

其中 **复杂的缓存架构**：才是我们最真实要讲解的东西，支撑高并发、高可用

缓存架构过程中，我们会讲解各种高并发场景下的各种难题，怎么去解决这些难题、缓存架构的过程、各种技术和解决方案、高可用性

「亿级流量电商网站的商品详情页系统」的架构讲解会作为项目背景贯穿，且项目实战；
缓存架构，支撑高并发，高可用的系统架构；

在缓存架构的过程中，高并发以及高可用相关的各种技术点和知识点、解决方案串在一起讲解了


这套课程，下面的 12 个问题学完以后，会学到很多的全网独家的技术

- 大型电商网站的商品详情页系统的架构
- 复杂的缓存架构
- 如何用复杂的缓存架构去支撑高并发

在自己项目中如果有可能将缓存架构做成高可用机会，那么可以学到高可用系统架构构建的技术，做到真正把这课程知识点融会贯通

## 真正能支撑高并发以及高可用的复杂系统中的缓存架构有哪些东西？

1. 如何让 redis 集群支撑几十万 QPS 高并发 + 99.99% 高可用 + TB 级海量数据 + 企业级数据备份与恢复？

    redis 企业级集群架构
2. 如何支撑高性能以及高并发到极致？同时给缓存架构最后的安全保护层？

    (nginx + lua) + redis + ehcache 的三级缓存架构
3. 高并发场景下，如何解决数据库与缓存双写的时候数据不一致的情况？

    企业级的完美的数据库 + 缓存双写一致性解决方案
4. 如何解决大 value 缓存的全量更新效率低下问题？

    缓存维度化拆分解决方案
5. 如何将缓存命中率提升到极致？：

    双层 nginx 部署架构，以及 lua 脚本实现的一致性 hash 流量分发策略
6. 如何解决高并发场景下，缓存重建时的分布式并发重建的冲突问题？

    基于 zookeeper 分布式锁的缓存并发重建解决方案
7. 如何解决高并发场景下，缓存冷启动 MySQL 瞬间被打死的问题？

    基于 storm 实时统计热数据的分布式快速缓存预热解决方案

8. 如何解决热点缓存导致单机器负载瞬间超高？

    基于 storm 的实时热点发现，以及毫秒级的实时热点缓存负载均衡降级
9. 如何解决分布式系统中的服务高可用问题？避免多层服务依赖因为少量故障导致系统崩溃？

    基于 hystrix 的高可用缓存服务，资源隔离 + 限流 + 降级 + 熔断 + 超时控制
10. 如何应用分布式系统中的高可用服务的高阶技术？

    基于 hystrix 的容错 + 多级降级 + 手动降级 + 生产环境参数优化经验 + 可视化运维与监控

11. 如何解决恐怖的缓存雪崩问题？避免给公司带来巨大的经济损失？

    独家的事前 + 事中 + 事后三层次完美解决方案

12. 如何解决高并发场景下的缓存穿透问题？避免给 MySQL 带来过大的压力？

    缓存穿透解决方案

13. 如何解决高并发场景下的缓存失效问题？避免给 redis 集群带来过大的压力？

    缓存失效解决方案

## 学会了这套课程，能给你带来些什么？工作中以及职业发展中？

> 工作中

如果你遇到了类似的缓存架构的一些问题，你可以立刻将学到的东西结合你的项目业务融入到架构中去；系统架构重构，抵抗各种更加复杂的场景的架构

> 职业发展中

缓存、redis、复杂的缓存架构，解决的复杂场景，技术亮点，青睐，拿到更好的职位

> 学完这套课程能去应聘 java 架构师吗？

绝对不行，缓存架构 只是 java 架构师必备的一项架构技能，还包含其他的技能，比如高并发（缓存架构、异步队列架构、复杂的分库分表）、高可用架构（hystrix 分布式系统服务的高可用），微服务的架构等

本课程只是让你积累了成长为 java 架构师过程中，必备的一项缓存架构的技能


<iframe  height="500px" width="100%" frameborder=0 allowfullscreen="true" :src="$withBase('/ads.html')"></iframe>