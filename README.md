分布式数字交易系统。
### _ＡＰＰ主要界面_
 
   <img src="https://ae01.alicdn.com/kf/U59977bba76bf49c69d39e6809ff0e0a52.jpg" alt="首页"  height="500" align="bottom" /> 　　　  <img src="https://www.hualigs.cn/image/6058141976745.jpg" alt="合约交易"  height="500" align="bottom" /> 
 　　　  <img src="https://www.hualigs.cn/image/605814358deac.jpg" alt="充值"  height="500" align="bottom" />
### _后台管理主要界面_
<img src="https://ae01.alicdn.com/kf/U0054bc0a2b8040ae9db2abe50eea18bc1.jpg" alt="个人中心"  height="500" align="bottom" /> <img src="https://ae01.alicdn.com/kf/U3ce9ce1c8d4f4dd4b34e33323c3207a2Q.jpg" alt="个人中心"  height="500" align="bottom" />
### _项目结构_

```
coin_exchage
  ---admin-manager 交易所后台管理模块
  
  ---admin_manager_robot 现货马丁网格机器人后台管理模块
  
  ---common-service 公共接口依赖（服务之间的调用接口）
  
  ---common-entity  公共实体类依赖（负责服务之间的数据传输序列化，Model，DTO,POJO,以及工具类）
  
  ---front-api  前端服务（提供对外接口，通过RESTful接口调用，充当服务的消费者）
  
  ---provider-service 服务提供者模块
  
       ---assets-api     币币交易服务
	   
	   ---contract-api  合约交易服务
	   
	   ---member-api  用户中心,用户个人资料设置基本服务
	   
	   ---recharge-api  充值服务
	   
	   ---robot-api   现货马丁网格机器人交易服务
	   
	   ---system-api  系统的基础设置服务
	   
	   ---socket-api  系统对外的socketio服务（将系统的数据推送给客户端）
	   
  ---xianhuo-web-socket-api 与火币币币交易socket通讯，并将价格同步到系统
  
  ---contract-socket-api 与火币合约交易socket通讯，并将价格同步到系统```
```
### _主要技术_
  dubbo，springboot，mybatisplus，rabbitMq，redis，zookeeper，分布式锁，分布式事物，vue
  源码后续更新，感谢关注。
  
### _联系方式_
- QQ：549930434
- 邮箱：coinExchangeOwerZH@protonmail.com

