# 程序员的狼人杀 (wolf)

[![Build Status](https://api.travis-ci.org/node-webot/weixin-robot.png?branch=master)](https://travis-ci.org/node-webot/weixin-robot) [![repo dependency](https://david-dm.org/node-webot/weixin-robot.png)](https://david-dm.org/node-webot/weixin-robot)

A solution for playing 'Werewolf' without cards！

[微信公众平台](http://mp.weixin.qq.com/)提供的[开放信息接口](http://mp.weixin.qq.com/wiki/index.php?title=%E9%A6%96%E9%A1%B5)的自动回复系统。


`wolf` 是基于[weixin-robot](https://github.com/wuhaifengdhu/weixin-robot) 模块开发的。

程序安装：

1，拷贝代码到本地。
    >git clone https://github.com/wuhaifengdhu/wolf.git
    
2，安装nodejs依赖。
    >npm install
    
3,运行。
    >node index.js


微信公众号简介：
如果一群人围在一起想玩狼人杀却发现没有带狼人杀的牌，是不是很蛋疼？那么就由我们这个小机器人将给你一个非常舒适的解决方式。
任何一个人通过命令创建一个房间，得到一个房间号，其他人输入房间号和自己的名字，就能获得自己的角色了。然后就可以愉快的游戏了。


添加微信帐号，试试效果：

![微信公众号帐号：moonlight_melody](http://m1.img.srcdd.com/farm4/d/2014/1101/14/50D93ED12176EFF4FCDDD449D14C5F90_B500_900_344_344.jpeg)


常用命令：
    创建房间命令：
        >create 狼人 3 女巫 1 预言家 1 村民 4
    进入房间命令：
        >1449 小明
    上帝查看角色命令：
        >list
    再来一局命令：
        >restart
    房间重启后获得新角色命令：
        >role

补充说明：
    1,创建房间时，系统会默认加入一个上帝角色，所以玩家不用输入上帝了。其他玩家可以任意发挥。
    
    2,第一次进入房间（以后只需输入房间号），请严格按照标准："房间号 名字"输入，并且名字不能有空格。上帝查看游戏角色时，会显示这个名字。
    
    3,再来一局命令，只有房间创建者和上帝可以使用;
