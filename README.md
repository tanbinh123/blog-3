## 2020/2/19
写了一篇，从0开始部署一个网站，以我的这个项目为例，版本1.1的target文件下有我打好的jar包，博客地址:https://blog.csdn.net/hangao233/article/details/104395693

## 2020/2/17
最外面的.sql文件是配合第一个版本的blog，第一代版本安全是用的拦截器做的，blog1.0是用的shiro做的，后面的版本都是根据shiro来的。blog1.0里有shiro版的.sql文件。

## 2020/2/15
最近学习了linux和docker，在阿里云租了个服务器，买了个域名，将自己的博客网站跑起来了，虽然还很简陋哈哈。如果有想把自己的项目部署到公网上的，可以联系我，我可以提供一些简单（自己太菜）的指导，传送门：http://www.ronggb.cn/


# 错误
1.一些小伙伴在用我的代码时跑不起来，有些pojo类中的基础方法爆红，是因为没有安装lombok插件。。这是我的偷懒，不好意思，安装上应该就不会爆红了

2.解决了一个shiro的bug，在登录时，会跳到一个错误的页面，还有很多bug，希望大家指出。


3.记得修改自己的maven home directory配置，不然会报错
![](https://rong-1257752702.cos.ap-chengdu.myqcloud.com/%E5%8D%9A%E5%AE%A2%E9%A1%B9%E7%9B%AE/1.png)


# 更新
blog1.0 :最近学习了一波shiro安全框架，原来是用的拦截器做的登录认证，现在用shiro的登录认证，只是最基础的shiro用法，入门即可，shiro的授权功能还用不到


blog1.1 :可以自己打包，在linux服务器上跑，解决了一些小bug。 

# blog
blog系统，后台管理系统，前台展示

## 注意
1. 参考b站Yancy02发布的视频，特此感谢
2. 原视频用的jpa，自己用mybatis进行了改写，想学习mybatis的同学可以进行了解参考
3. 由于自己第一次用mybatis做一个项目，代码写的很丑，希望大家能指导指导
4. 后面会陆续添加一些功能，慢慢完善，有兴趣的朋友可以交流



## 我觉得的难点
1. mybatis的一对多，多对一，对于我这个编程小白还是挺难的
2. mybatis的动态sql语句
3. 数据库的设计，为了（范式规范）连表查询，所以在设计数据库时，blog表包含了很多其他表的id


个人联系方式：qq:1437810640(备注来源，可以进行一些问题的交流）


环境：
1. idea
2. mysql 5.7
3. springboot2.2.2
4. shiro1.4.1

技术栈
1. mybatis
2. springMvc
3. springboot
4. thymeleaf模板引擎
5. Semantic Ui
6. shiro
7. docker
