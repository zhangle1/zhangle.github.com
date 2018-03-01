# 个人简历
张乐的个人简历
#个人信息
姓名:张乐

性别：男

出生年月: 1994年9月23日

籍贯： 浙江省-温州

学历:本科

学校专业： 温州大学瓯江学院计算机系

电话： 18367803065

Email：zhangleshiye@gmail.com

博客：http://blog.csdn.net/zhangle1hao

github：https://github.com/zhangle1

stackoverflow:https://stackoverflow.com/users/6246860/zhangl

# 自我简介
* 两年Android开发工作经验

* 拥有一定的自学能力和团队合作能力。

* 希望成为一个能解决更多问题的程序员,github用户，希望接下能够写一些有用的开源代码和博客。


# 技能

* Android原生应用开发,熟悉Android开发工具Android studio，以及热门开源框架使用及封装

* 熟练使用版本管理工具git

* 一定的第三方文档阅读能力,和源码阅读能力,可以根据需要将功能需求从开源项目中拆出,积累了一些业务代码。

* 有一定的阅读英文资料的能力，可以从stackoverflow上查找报错解决方案，以及从github上搜索热门的框架，和优秀的源码并学习。

* 目前对后端框架Jhipster感兴趣，学习Spring家全家桶，前端Angular。可以根据需要，短时间上手后端。

# 个人经历

* 2012          进入温州大学瓯江学院学习

* 2012.9-2015.9 担任过小组组长，实践课，以及老师的一些小项目。 

* 2015.9-2016.9 温州创力电子科技

* 2016.9-2017.8 温州索思科技

* 2017.9-2018.3 休息，

#作品

	
* 东航的项目，利用手环检测飞行员的身体数据，以及推送消息提醒。
* 在疲劳管家中负责三大核心模块的消息推送模块，利用了第三方极光推送，实现了应用内单向角标提示，以及推送9大列表(今日航班提醒，明日航班提醒，今日跑步数等)，以及点击详情内容,和应用内弹窗提醒，另外实现一些功能点以及修复bug。
* 消息提醒细节，集成极光推送，从极光推送的静态广播中(广播只保存短暂时间，所以启动自己的服务，并传入9种不同的json类型)，启动自己的IntentService（本地服务的子类，不是运行在子线程）,解析分别处理操作（存数据库和发送广播） ，应用内存在(Local广播接收) ，数据库方面，做两张简单的表，一张存角标消息数和对应的类型，在页面中做相应的UI事件，清零。一张则存具体的类型和数据。广播则是通知界面，做一些操作（弹窗，消息刷新）。这样实现了一个简单的消息推送效果。
* Jpush缺点,因为国内Android环境原因，在应用外服务可能被杀死接收不到（即使，锁屏唤醒，和网络切换唤醒），Android和IOS不同，IOS走的是苹果的推送，而Android端第三方推送实质上是就是消息。
* 在解析明日航班信息的时候其实Json数据很复杂，有自己的，伙伴的航班，而且极光推送字数的限制,导致客户端解析很痛苦。有较强的解析json能力，但是手机测试账号里已经没有数据- -
* 完善拍照以及一些小功能点。
 *** 


<img src="https://github.com/zhangle1/zhangle.github.com/blob/master/my-pic/Screenshot_2016-08-24-21-02-54_com.mackpower.band.png" width = "30%" height = "30%"   />
<img src="https://github.com/zhangle1/zhangle.github.com/blob/master/my-pic/Screenshot_2016-08-24-21-03-08_com.mackpower.band.png" width = "30%" height = "30%"   />
<img src="https://github.com/zhangle1/zhangle.github.com/blob/master/my-pic/Screenshot_2016-08-24-21-03-10_com.mackpower.band.png" width = "30%" height = "30%"   />
<img src="https://github.com/zhangle1/zhangle.github.com/blob/master/my-pic/Screenshot_2016-08-24-21-03-13_com.mackpower.band.png" width = "30%" height = "30%"   />
<img src="https://github.com/zhangle1/zhangle.github.com/blob/master/my-pic/Screenshot_2016-08-24-21-03-23_com.mackpower.band.png" width = "30%" height = "30%"   />
<img src="https://github.com/zhangle1/zhangle.github.com/blob/master/my-pic/Screenshot_2016-08-24-21-03-25_com.mackpower.band.png" width = "30%" height = "30%"   />
<img src="https://github.com/zhangle1/zhangle.github.com/blob/master/my-pic/Screenshot_2016-08-24-21-03-28_com.mackpower.band.png" width = "30%" height = "30%"   />

*** 
	
* 公司已经有了AppCloud版的运营平台，希望有Android原生版。在这个项目中，我尝试着学习并使用Github上的一些clear-结构体系，尝试用了一些热门的三方库rxjava+retrofit,等，目前完成了此项目的前期的架构。也是这个项目让我感到困惑，希望能够重新找一份工作，能够跟优秀的程序员学习，提高自己的能力。
* 收获1，学会了一些rxjava的操作符，gson的自定义，服务器端String传空值置成"",结合retrofit对服务端自定义的错误处理。学习封装此框架。
* 目前最大的收获，也是最大的困惑，如何合适的解析数据，因为运营平台的通用性，此项目通用接口只有5个主接口，比如列表接口CommonJsonQuery?json:{}详细接口CommJsonDetail?json:{}，通过获取上一层的信息填入。得到的数据以及具体的列item也要根据11种类型填入。服务端给了一个ObjectjSON用来表示字段的属性，以及一些特殊性的json，CmmonDeatil里是数据的键值，一些引用类型又需要参照其他的表来动态填入。再结合一些侧拉搜索,以及一些UI变化，让我重新反思没有运用MVP模式. 并通过了解clear-结构体系 ,了解一些ViewModel, Responsity，一些概念，以及运用。


<img src="https://github.com/zhangle1/zhangle.github.com/blob/master/my-pic/Screenshot_2016-08-20-16-01-55_com.makepower.modo.png" width = "30%" height = "30%"   />
<img src="https://github.com/zhangle1/zhangle.github.com/blob/master/my-pic/Screenshot_2016-08-20-16-02-17_com.makepower.modo.png" width = "30%" height = "30%"   />
<img src="https://github.com/zhangle1/zhangle.github.com/blob/master/my-pic/Screenshot_2016-08-20-16-02-24_com.makepower.modo.png" width = "30%" height = "30%"   />
<img src="https://github.com/zhangle1/zhangle.github.com/blob/master/my-pic/Screenshot_2016-08-20-16-02-35_com.makepower.modo.png" width = "30%" height = "30%"   />
<img src="https://github.com/zhangle1/zhangle.github.com/blob/master/my-pic/Screenshot_2016-08-20-16-02-40_com.makepower.modo.png" width = "30%" height = "30%"   />
<img src="https://github.com/zhangle1/zhangle.github.com/blob/master/my-pic/Screenshot_2016-08-20-16-02-45_com.makepower.modo.png" width = "30%" height = "30%"   />
<img src="https://github.com/zhangle1/zhangle.github.com/blob/master/my-pic/Screenshot_2016-08-20-16-01-55_com.makepower.modo.png" width = "30%" height = "30%"   />
<img src="https://github.com/zhangle1/zhangle.github.com/blob/master/my-pic/Screenshot_2016-08-20-16-02-54_com.makepower.modo.png" width = "30%" height = "30%"   /> 

