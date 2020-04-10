## URL中文名称统一资源定位符

URL=协议+域名或IP+端口号+路径+查询参数+锚点

----------
### 域名
IP是用来定位一个设备的
域名就是对IP的别称

域名是怎么对应IP的？通过DNS(即域名服务)
baidu.com对应什么IP？使用命令行(ping baidu.com)就可以得到对应的IP
注意：一个域名可以对应不同的IP，这个叫做负载均衡，防止一台服务器扛不住
同时一个IP也可以对应不同的域名，这个叫做共享主机

当你输入xiedaimala.com发生了什么？
过程

 1. 你的浏览器会向电信/联通/移动提供的DNS服务器询问xiedaimala.com对应什么IP(命令：nslookup
    xiedaimala.com)
 2. 电信/联通/移动会回答一个IP(具体过程很复杂，不研究)
 3. 然后浏览器才会向对应IP的80端口(http服务)或443端口(https)发送请求
 4. 请求内容是查看xiedaimala.com的首页

www.xiedaimala.com和xiedaimala.com是同一个域名吗？不是
com是顶级域名
xiedaimala.com是二级域名(俗称一级域名)
www.xiedaimala.com是三级域名(俗称二级域名)
它们是父子关系
----------
如：https://www.baidu.com/s?wd=hello&rsv_spt=1#5

协议：https

域名：www.baidu.com

路径：/s(一般默认访问根目录)

查询参数：?wd=hello&rsv_spt=1

锚点：#5
