## 培训课程体系

#### 准备阶段（版本0.0.1）

##### 准备一：开发环境搭建
  1. meteor安装<https://www.meteor.com/install>
    - windows 32-bit 安装时可能存在问题
    - 默认安装在系统盘根目录下。安装成功后
      1. win+r
      2. cmd
      3. enter
      4. meteor create myFirstMeteorProject
      5. cd /file-path/myFirstMeteorProject
      6. meteor run或meteor 
      7. 浏览器地址栏 - meteor默认3000端口
        - 127.0.0.1:3000 或者
        - localhost:3000  
      8. meteor --port 4000 //自定义，让这个meteor项目在4000端口跑。
        - 应用场景，有了一个meteor项目正在使用3000端口;但是你开了一个新的terminal，需要跑第二个meteor项目。
  2. text editor 
    1. 我们用的是Atom，sublime
    2. 其它常用的编辑器有：vim, Emacs。其它编辑器<https://developer.mozilla.org/en-US/Learn/Common_questions/Available_text_editors>
  3. 浏览器与Dev Tools 
    1. 浏览器 
      1. 我们用的是 chrome browser。
      2. MS Edge, FireFox <https://www.mozilla.org/en-US/firefox/developer/> 等也可以
    2. Dev Tools
      1. 打开：按下 F12;  或者 ctrl + shift + I
      2. 关闭：再次按下 按下 F12;  或者 ctrl + shift + I
      3. 关于Dev Tools,更多 详见 <https://developer.chrome.com/devtools>. 目前开发中，90%只用到了其中的console.
  4. 数据库相关工具robomongo -可选
    1. 下载，安装<https://robomongo.org/download>。
    2. 免费版即可。
    3. 主要操作：
      1. create
      2. connect
      3. 删除某一条记录 
  5. 代码托管: 
    1. 我们目前用的是 github.com <https://github.com/>. 
    2. 其它的代码托管平台详见<http://www.cnblogs.com/yunfeifei/p/4209625.html>
    3. 在你选择的代码托管平台上注册帐号。
    4. 了解 :
     - repository
     - fork
     - branch
     - issue
     
  6. git 
    1. windows 系统用户请下载 gitbash，地址<https://git-scm.com/>
    2. Mac系统自带，不用另行下载。
  7. 安装nodejs 和 npm 
    1. 下载地址<https://nodejs.org/en/> 
  8. 翻墙软件。可选。

##### 准备二：背景知识
  1. HTML基础知识 <http://www.w3school.com/> <http://www.w3school.com.cn/>
    1. 注释 的作用？
    2. HTML中的注释。JS中的注释。二者的区别。
    3. open tag, close tag. 有的element 不需要 close tag.
    4. block element; inline element
  2. CSS基础知识 <http://www.w3school.com/> <http://www.w3school.com.cn/>
    1. 主要看selector 部分
  3. Javascript基础知识 <http://www.w3school.com/> <http://www.w3school.com.cn/>
    1. 数据类型
    2. 函数的定义，函数的执行，函数的调用
    3. 条件判断语句和循环语句。尤其是if statement；for loop
    4.  对象
    5. HTML, CSS, JavaScript在 web development中各自的作用
    6. events, 事件绑定
    7. this
  4. Meteor:
    1. 参见 <https://www.meteor.com/tutorials/blaze/creating-an-app>，一步步把示例中的Todo App做出来。 
    2. <http://zh.discovermeteor.com/>前七章过一遍
    3. reactivity
      1. 后台MongoDB,前台Minimongo-- 之前的互动机制 
    4. Meteorjs 与react, angular等框架的区别与联系
    5. Meteor项目的文件结构
    6. Meteor.isClient, Meteor.isServer
    7. publish, subscribe
    8. helpers, event handlers
    
  
    
##### 学习资源
###### 精
  1.Meteor官网
    - <http://guide.meteor.com/#guide-concepts> 
    - <http://docs.meteor.com/#/full/>
  2. git官网 <https://git-scm.com/>. 
    1. 必读：<https://git-scm.com/about/branching-and-merging>.
    2. 必须掌握的命令. 注意: windows操作系统，git命令必须在git bash 的terminal 里输入，不能在windows自带的CMD terminal里运行。
      1. git clone 
      2. git status
      3. git diff
      4. git add
      5. git commit -m
      4. git pull origin master
      5. git push origin master
      5. git remote -v
      6. git remote add origin
      7. git checkout -b 
      8. git branch -l
    3. <https://git-scm.com/book/en/v2>  
    4. 基础的Linu文件操作命令(在git bash shell中用，部分也可以用于CMD terminal 或MS power shell)。- 请补充、更正
      1. cp
      2. mv
      3. ls, ls -l, ll
      4. pwd
      5. mkdir
      6. touch
      7. vim
      8. rm - 如何删除空文件夹？如何删除不为空的文件夹？ 
      9. q
      10. i
      11. spacebar

###### 博
  1. <https://npmjs.com/>
  2. <https://atmospherejs.com/>
  3. markdown 
    1. 什么是markdown?
      - <https://guides.github.com/features/mastering-markdown/>
      - markdown新手指南 <http://www.wiz.cn/feature-markdown.html>
    2. markdown编辑器
      1. sublime - 要安装相应的插件 <https://packagecontrol.io/search> search for "markdown"
      2. 有道云 <http://note.youdao.com/> 
      3. 作业部落 <http://wwwzybuluo.com> 
  4. sublime text 3
    - sublime 的使用 <https://www.sublimetext.com/docs/3/> 请熟手提炼后补充。
    - <https://packagecontrol.io>
  5. <https://github.com/vhf/free-programming-books/blob/master/free-programming-books-zh.md>

#### 第一阶段: 用户系统
  0. 预习内容
    1. Meteor: users and accounts <http://guide.meteor.com/accounts.html>
    2. Meteor: password login <http://guide.meteor.com/accounts.html#accounts-password>
    3. alanning:roles <https://atmospherejs.com/alanning/roles>
    4. iron router<https://github.com/iron-meteor/iron-router> 或  flow router<https://github.com/kadirahq/flow-router>
    5. meteor: accounts <http://docs.meteor.com/api/accounts.html>
    6. meteor:accounts-ui <http://docs.meteor.com/packages/accounts-ui.html>
    7. meteor:currentUser <http://docs.meteor.com/api/accounts.html#currentUser>
    4. 下载培训时要演示的代码。地址：<https://github.com/maodouio/users-boilerplate>
      1. git clone https://github.com/maodouio/users-boilerplate.git 
  1. 培训内容：
    1. 基本用户登录系统
      - 用户名和邮箱登录
    2. 用户角色设置和权限管理
      - 管理员, 会员, 普通用户
  

#### 同学的常见问题
1. isInRole
2. users
3. Roles
4. Meteor.login(), Meteor.logout()
5. ctrl+/
6. {{> atForm}}
7. 关系型数据库与非关系型数据库的区别与联系
8. JSON格式
9. 如何推送到服务器？如何布署？
10. blaze是什么？与包的区别与联系
11. route的概念和作用
12. subscribe, publish互动的机制？



作者：张冰
日期：20160616
如有任何错误、问题、意见、建议等，欢迎指出。或径行更正并注明出处或联系：
roy2020china@github
40224272@qq.com
