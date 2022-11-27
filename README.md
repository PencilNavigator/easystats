# Freenom-Workers



通过Cloudflare Workers自动续期Freenom域名(.cf .ga .gq .ml .tk)。

Renew your Freenom domain (.cf .ga .gq .ml .tk) automaticly with Cloudflare Workers.

喜欢这个项目？给颗Star吧！Like this project？ Star it!


# 部署 Set-Up

打开https://dash.cloudflare.com

在账号主页左侧侧边栏选择Workers

在Workers页面，选择创建服务，设置好服务名称，选择HTTP处理程序。

在刚刚创建的Workers界面，选择“快速编辑”。

在编辑界面，粘贴worker.js内代码，点击保存。

返回刚刚创建的Workers页面，选择“设置”，再选择“变量”。

在变量页面，添加变量“SECRET_USERNAME”和“SECRET_PASSWORD”，在SECRET_USERNAME变量中填入Freenom用户名，在SECRET_PASSWORD变量中填入Freenom密码。

（可选）勾选两个变量的“加密”选项（可极大程度降低Freenom用户名和密码泄露的概率）。

返回创建的Workers页面，选择“触发器”。

在触发器界面，选择添加Cron触发器。在“添加Cron触发器”界面，设置触发器，保存。推荐执行时间为一周一次。


# 测试

访问刚刚部署的Workers服务的域名（一般URL为：服务名.设置子域.workers.dev)。顺利的话，你将看到你账户内所有域名的剩余日期。


# 待实现的功能
执行成功后，通过邮件送信/TelegramBot/DiscordBot发送执行结果。

# 类似项目
https://github.com/luolongfei/freenom

https://github.com/mkorthof/freenom-script

https://github.com/Oreomeow/freenom-py

https://github.com/RouRouX/docker-freenom-automatic-renewal

# LICENSE
可能是AGPL-V3.0？

![mona-loading](https://github.githubassets.com/images/mona-loading-dark.gif)

