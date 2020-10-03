booking-hospital数据库设计

1 用户表 user_id  usersname userscardnum user_phonenum users_id  hos_id

2 医院表 hos_id  user_id  hos_name  hos_intro

3 科室表 class_id  hos_id  class_name doctor_id

4 医生表 doctor_id  doctor_name class_id  work_id doctor_img

5 预约表book_id  user_id hos_id class_id doctor_id  work_id

6 上班时间表  work_id  doctor-id  work_date 

Booking—Hospital网上预约

1 主要的产品介绍：

  对着科技的进步，APP，程序，已经成为我们做事的便捷首选，我们可以用 美团 饿了吗进行订餐，可以用淘宝，京东等电商平台订购我们生活所用品，出行可以用APP扫扫共享单车。为我们节约了很多的宝贵时间，所有我们小组此次的项目是针对网上预约挂号，通过这个程序进行预约挂号

2 主要的技术

开发环境：Linux vmware  xshell 6 

前端：HTML ajax Bootstrap3  jquery css json

后端：springBoot  dubbo 

数据库： redis 

3 实现的功能

1   用户只用单次注册就可以在多家医院进行挂号

2  个人中心页面，记录个人的就医的详细情况，可以作为个人的健康监控表，守约记录表，记录个人的挂号信用值，一个月超过三次，就拒接挂号，下个月才可以网约挂号

3  提醒就医，预约时间的前两个小时会手机提醒就医（加入行程表中？）