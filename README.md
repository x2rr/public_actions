## 定时任务
jio本介绍:
掘金社区自动签到 
签到后会获得一次免费抽奖机会，自动免费抽奖一次。
执行完发送通知签到结果,调用qinglong内sendNotify.js。

jio本导入:
```
#进容器
docker exec -it qinglong bash
#拉仓库(一)
ql repo https://github.com/HarrylXue/public_actions.git "juejin_"
#或拉单文件(二)
ql raw https://raw.githubusercontent.com/HarrylXue/public_actions/master/juejin_signin.js


#发给bot
/dl https://raw.githubusercontent.com/HarrylXue/public_actions/master/juejin_signin.js
```

获取变量:
打开浏览器，登录掘金社区(https://https://juejin.cn/)，F12 查看 Network 面板 XHR里选一下查看headers，复制 cookie

添加变量:
在 qinglong 面板新建一个环境变量(暂时只兼容单用户 多用户待定)
| key | value |
| --- | ---|
| JUEJIN_COOKIE | 值为上面复制掘金的 cookie |

`注意：掘金的cookie大概有一个月的有效期，所以需要定期更新cookie`
