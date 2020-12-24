SunZiDong20182123048


####  软件建模作业 2：

按照第一次作业小组进行分组后完成以下作业：

理论部分，回答以下问题：

##### 1）．试论述类与用例的区别。

答：类是对一组具有相同属性、操作、关系和语义的对象的描述。类是对事物的抽象。而用例是对一组序列动作的描述，系统执行这些动作将对用例的参与者产生可以观察的结果。</br></br>

 

##### 2）．试比较边界类与实体类的异同。

答：实体类是对系统中需要存储的信息和其信息的行为建立模型。实体类具有永久的特性，这类似于数据库中的表一样用于保存系统的业务信息。

边界类位于系统与外界的交接处，它在一个或多个角色和系统之间建立相互作用的模型。<br><br>



##### 3）．试运用本节所学的静态建模技术找出用户管理模块中的所有的类。

l 边界类，描述外部与系统内部交互的类；

l 控制类，控制其他类；

l 实体类，存储信息和相关行为的类；<br><br>

 

##### 4）．请找出学生管理系统中学生注册用例的实体类，边界类，控制类。

&nbsp;&nbsp;&nbsp;&nbsp;学生类就是实体类，边界类是注册界面类，控制类是注册类，对应的是用例中的注册。<br>
&nbsp;&nbsp;&nbsp;&nbsp;UML中类有三种主要的版型：边界类、控制类和实体类。引入边界类、控制类及实体类的概念有助于分析和设计人员确定系统中的类。<br>
&nbsp;&nbsp;&nbsp;&nbsp;边界类位于系统与外界的交界处，窗体、报表、以及表示通讯协议的类、直接与外部设备交互的类、直接与外部系统交互的类等都是边界类。通过用例图可以确定需要的边界类，每个Actor/Use Case对至少要一个边界类，但并非每个Actor/Use Case都有唯一的边界类。<br>
&nbsp;&nbsp;&nbsp;&nbsp;实体类保存要放进持久存储体的信息。持久存储体就是数据库、文件等可以永久存储数据的介质。实体类可以通过事件流和交互图发现。通常每个实体类在数据库中有相应的表，实体类中的属性对应数据库表中的字段。<br>
&nbsp;&nbsp;&nbsp;&nbsp;控制类是控制其他类工作的类。每个用例通常有一个控制类，控制用例中的事件顺序，控制类也可以在多个用例间共用。其他类并不向控制类发送很多消息，而是由控制类发出很多消息。<br><br>

##### 5）．什么是依赖？它与关联有什么区别？

答：依赖是一种使用关系，它说明了一个事物声明说明的变化可能影响到使用它的另一个事物，但反之未必。也就是说，服务的使用者以某种方式依赖于服务的提供者。而关联是一种结构关系，它详述了一个事物的对象与另一个事物的对象相互联系。<br><br>

 

##### 6)．什么是泛化？泛化是否就是类的继承，如果不是请说明理由。

答：泛化是一般事物（称为父类或超类）和较特殊事物（称为子类或孩子类）之间的关系。

泛化不是类的继承，类的继承是泛化的一种。<br><br>

 

##### 7）．试论述聚合和组合的异同。

答：聚合描述了整体对象拥有部分对象的关系。

组合是聚合的一种形式，它具有强的拥有关系，而且整体与部分的生命周期是一致的。<br><br>

 

##### 2、学院公众号中，成绩查询模块可以很方便地使在校学生查询到期末考试成绩，特别是老师将期末成绩提交后，该模块会以弹窗的方式将信息通知到学生，问题：请根据滇池学院微信公众号中，学生成绩查询模块的功能，对该模块进行小组讨论分析，对该功能的类图中以

下元素进行必要说明：

1）该功能一共应该包含哪几个类

该成绩查询功能包含6个类，分别是：学生、老师、管理员、学期筛选、成绩下载、学科成绩<br><br>

 

2）每个类的属性，方法应该是什么，有什么作用，权限该是什么
      成绩查询包含下图所示类，类中标出各类属性、方法
      权限如下：
          a、学生可以查看自己成绩，能够筛选学期
          b、老师只能查询学生成绩、录入学生成绩
          c、只有管理员能添加和删除、修改学生信息
          d、所有用户都能下载全科目成绩

![成绩查询包含类](https://github.com/SZD1030/SunZiDong20182123048.github.io/blob/main/%E6%88%90%E7%BB%A9%E6%9F%A5%E8%AF%A2%E7%B1%BB.png)


<br>
3）类之间分别有什么关系

- 学科成绩依赖于学生

- 学科成绩依赖于老师

- 学科成绩依赖于管理员

- 学生于老师是多对多的关联关系

- 老师与管理员为泛化关系

- 成绩下载依赖于学生

- 成绩下载依赖于老师

- 学期筛选依赖于学生
- 学期筛选依赖于老师

 
<br>
4）使用 staruml 画出该功能模块

![成绩查询](https://github.com/SZD1030/SunZiDong20182123048.github.io/blob/main/%E6%88%90%E7%BB%A9%E6%9F%A5%E8%AF%A2.png)

 
<br>
##### 3、网络的普及带给了人们更多的学习途径，随之而来的管理远程网络教学的“远程网络教学系统”诞生了。“远程网络教学系统”的功能需求如下：学生登录网站后，可以浏览课件、查找课件、下载课件、观看教学视频。教师登录网站后，可以上传课件、上传教学视频、发布教学心得、查看教学心得、修改教学心得。系统管理员负责对网站页面的维护、审核不合法课件和不合法教学信息、批准用户注册。

问题：老师需要登录“远程网络教学系统”后才能正常使用该系统的所有功能。如果忘记密码，可与通过“找回密码”功能恢复密码。请使用staruml 画出教师参与者的类图。

老师登录“远程网络教学系统”类图：

![远程教学](https://github.com/SZD1030/SunZiDong20182123048.github.io/blob/main/%E8%BF%9C%E7%A8%8B%E6%95%99%E5%AD%A6.png)

该老师“远程网络教学系统”类图共有6个类，分别为：登录、上传教学视频、上传课件、发布教学心得、查看教学心得、修改教学心得。

- 上传教学视频依赖于登录

- 上传课件依赖于登录

- 发布教学心得依赖于登录

- 查看教学心得依赖于登录

- 修改教学依赖于登录

- 修改教学心得于查看教学心得相关联

