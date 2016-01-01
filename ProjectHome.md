FxAsk爱问程序

版本信息：
版本号：v2.0
发布更新日期：2009年1月13日

此程序是免费程序，可自由使用，不过请保留程序底部的版权连接，谢谢大家的支持。


特别说明：
在后台的首页上，会显示本程序的最新版本和补丁等信息。并且有免费注册本程序的连接，注册后可不断获得程序积分，然后用户可以使用这些程序积分获取程序插件下载和新的程序下载。
程序积分获取途径：1是访问后台，每天增加50积分，1天只增加1次。2是前台访问底部的版权连接，每IP访问加10积分，每天最高加100积分。


更新的几个功能：
后台系统设置设置得很强大，各种设置已经加到其上，有【基本功能   搜索引擎优化   上传设置   积分设置   ucenter接口   网页配置   模拟静态设置   验证码设置   地图设置   广告设置   支付设置   其他 】
从上面就可以看到加了很多功能了。
启用了RSS。
邮件提醒。
尝试与dz论坛同步登陆。
升级程序。

在后台系统设置有而没有完成的功能：
1.购买积分
2.与地图插件结合

此程序近期还有更新，最多是文件的替换，请多留意后台的更新信息。
1.0升2.0程序也在近期提供。


下载请到（随时更新）：http://www.zc18.com
交流QQ群:4292329

增加了ucenter的接口，如果要使用此功能，请确认目录“uapi-”属性为777。然后在ucenter后台那里添加一个应用。最后设置后台变量设置的配置。

程序作者简介：
feixin（郑新伟）

安装环境：
本程序具备跨平台特性，可以运行于 Linux/FreeBSD/Unix 及微软 Windows 2000/2003/XP/VISITA 等各种操作系统环境下。
需要服务器上装有如下软件：

可用的 httpd 服务器（如 Apache、Zeus、IIS 等）
php 4.1.0 及以上
MySQL 3.23 及以上



安装说明：

1.解压文件后上传到某目录，如果是linux系统请设置一下目录属性（目录即其下面的images、templates、templates/cache，属性设置为0777）。

2.请运行install.php

3.安装完后删除install.php，谨记！

4.可以使用了。

后台地址是：http://www.xxx.com/admin.php


模板说明：
前台模板目录:templates/default/，模板文件都是html格式。
后天模板目录:templates/admin/ ，一般不改此目录。

首页模板是templates/default/index.html
头部模板是templates/default/header.html
底部模板是templates/default/footer.html

根据网址找到模板，如问题列表栏目首页网址是index.php?op=list\_cat；模拟静态是fxask-list\_cat.html。
那么模板文件是templates/default/list\_cat.html。其他的也根据此规则查找模板。


js调用格式说明：


&lt;script type="text/javascript" src="http://www.zc18.com/fxask/index.php?op=js&type=调用类型&num=调用记录数&strlen=文字截断长度&id=分类id"&gt;



&lt;/script&gt;



http://www.zc18.com/fxask 改成你网站的网址。

调用类型有
hot\_question = 热门问题，可带分类id
new\_good\_question = 最新编辑推荐问题，可带分类id
new\_question = 最新问题，可带分类id
new\_file = 最新共享文件，可带分类id
hot\_file = 热门共享文件，可带分类id
ask\_money = 会员积分总排行
ask\_winmoney = 会员提问赚取积分排行
share\_money = 会员共享中心赚取积分排行
zhuanjia = 某分类的专家，要带分类id
new\_zhuanjia = 最新专家
调用记录数默认10条；

文字截断长度默认40，即20个中文字；

分类id根据调用类型不同而不同。

举例
热门问题，取5条，12个中文字


&lt;script type="text/javascript" src="http://www.zc18.com/fxask/index.php?op=js&type=hot\_question&num=5&strlen=28"&gt;



&lt;/script&gt;

