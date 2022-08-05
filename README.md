# a-robot
企微机器人推送消息，检测gitlab push 和 merge请求

# 不生产代码，只做代码的搬运工 😉

# 运行前你需要做什么

- 根目录下创建 .env文件
- 添加企微webhook作为环境变量 bot_api=https://qyapi.weixin.qq.com/123123/webhook/send?key=1234556 
- 然后就没了
- 如果gitlab机器人没有成功启动的话。可以在本地或者服务器内手动添加该环境变量

# 如何启动

> npm i or yarn

> node app.js

> cd gitlab-bot 

> npm run start or yarn start

# 如何添加自己的组件

> cd plugins
> 创建自己要做的事，可以在modules文件夹的class bot中查看自己可以使用的方法。发送文字 图片，md等。
> 在app.js中，在run()方法中使用cron表达式为任务添加定时。[不会cron表达式的可以看这里](https://crontab.guru/)

# 两个项目的原地址在这里

https://github.com/goodideal/gitlab-bot
https://github.com/im3x/GeekBot
