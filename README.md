## 功能实现的目标

1-基于springBoot平台，集成Redis，实现注册、登录、商品展示、商品详情、订单详情以及秒杀抢购功能  
2-解决缓存穿透、缓存雪崩及缓存击穿等问题  
3-添加消息队列消峰  
4-利用JMeter进行压测  
5-master-slave服务器，分摊DB压力  

## 已完成的工作

1环境搭建(Spring Boot+MyBatis+Druid)  
2登录功能实现与完善（包括数据校验、异常处理等）  
3Redis实现分布式Session  
4各种页面展示以及秒杀功能开发  
5利用AOP对service方法进行拦截，打印日志  
6展示页面的优化加速，对象缓存+页面缓存+页面静态化+前后端分离  
7利用jmeter进行压测，查看优化效果  
8集成RocketMQ，利用消息队列进行消峰、业务解耦    
9添加布隆过滤器防止缓存穿透  
10Redis缓存过期时间在原基础上附加一个随机值，避免缓存雪崩  
11安全方面：1)接口隐藏 ; 2)首次秒杀不需验证码，之后的请求需要验证码，将请求散开，分摊压力; 3)ip限流  
