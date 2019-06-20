# major-onepunch
一拳超人主题

个人兴趣爱好，喜欢一拳超人，做了个一拳超人主题的后台系统

在线体验地址 http://47.105.230.85
           体验账号：king  123456
                   janos 123456
           （超级管理员账号不开放）

项目介绍：

现在都在走前后端分离开发，作为java小白也去学了相对其他两大前端框架相对入手比较简单的vue，虽然开始遇到过很对问题，但是用着确实舒服！

主要用到的技术：

后端：
springboot 2.1.4 
springsecurity
redis
mybatis
fastjson
pagehelper

前端：
vue 2.5.2
element-ui
axios
vuex
echarts
vue-particles
vue-router

主要功能：
1、登录：登录之后将通过京东万象买的接口查询当前登录用户的ip信息，并生成token存储到redis，最后通过json返回给前端，每次登录成功都会将路由初始化时随机加载的动画全屏播放，播放完成之后跳转到系统首页，系不系很炫酷😁！

2、首页：主要展示当前登录用户的信息、登录信息及系统访问统计等；

3、个人中心：可以修改个人信息（身份信息、头像、密码等）😁；

4、系统管理：后台权限使用的是springsecurity进行权限控制，包括用户管理、角色管理、权限管理，前端权限控制是通过vue的自定义指令，后台返回用户的权限及角色信息后，将信息存储到vuex里，按钮的权限控制旧通过自定制指令加vuex里的权限去控制；

5、头像管理：用户可进行上传头像、查看头像、修改头像分类及删除头像等

6、在线用户：查看当前系统的在线用户，是通过查询redis中存储token，管理员权限可强制下线其他用户;

7、系统日志：用户进行操作之后，系统会将用户的操作信息进行入库，可进行查询及删除操作；

8、一拳漫画：想做，但是还没想好怎么做，待思考🤔

