# JimmyComment-HuaWei
# 吉米点评系统
## 技术栈：Spring、SpringBoot、Mybatis-Plus、MySQL、Redis
## 项⽬简介：
本项⽬是⼀个以社交为核⼼的新电商项⽬，向⽤⼾提供了短信登录、发布/阅览帖⼦、商铺分类检索、点赞关注、
⾼并发优惠券秒杀等功能。
## 责任描述：
- 后端开发主要采⽤SpringBoot与Mybatis-Plus技术，通过controller层处理浏览器发起的请求，service层处理业务逻辑，mapper层对数据库中的数据进⾏更改；
- 采⽤Redis缓存中间件，对⽤⼾登录信息、秒杀券信息、商铺类型列表信息、点赞信息等热点key进⾏缓存，提⾼⽤⼾的访问速度；
- 采⽤拦截器责任链模式，实现对⽤⼾登录token续期以及⽤⼾登录拦截功能；
- 基于AOP思想，记录数据库操作⽇志；
- 使⽤乐观锁+版本号，解决⾼并发下的库存超卖问题；
- 使⽤分布式锁解决⾼并发下的⼀⼈⼀单问题；
