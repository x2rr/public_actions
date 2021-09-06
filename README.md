## jio本学习
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
打开浏览器，登录 [掘金社区](https://https://juejin.cn/)，F12 查看 Network 面板 XHR里选一下查看headers，复制 cookie

添加变量:
在 qinglong 面板新建一个环境变量(暂时只兼容单用户 多用户待定)
| key | value |
| --- | ---|
| JUEJIN_COOKIE | 值为上面复制掘金的 cookie |

`注意：掘金的cookie大概有一个月的有效期，所以需要定期更新cookie`


## 特别声明

- 本仓库发布的脚本及其中涉及的任何解锁和解密分析脚本，仅用于测试和学习研究，禁止用于商业用途，不能保证其合法性，准确性，完整性和有效性，请根据情况自行判断。

- 本项目内所有资源文件，禁止任何公众号、自媒体进行任何形式的转载、发布。

- 本人对任何脚本问题概不负责，包括但不限于由任何脚本错误导致的任何损失或损害。

- 间接使用脚本的任何用户，包括但不限于建立VPS或在某些行为违反国家/地区法律或相关法规的情况下进行传播, 本人对于由此引起的任何隐私泄漏或其他后果概不负责。

- 请勿将本仓库的任何内容用于商业或非法目的，否则后果自负。

- 如果任何单位或个人认为该项目的脚本可能涉嫌侵犯其权利，则应及时通知并提供身份证明，所有权证明，我们将在收到认证文件后删除相关脚本。

- 任何以任何方式查看此项目的人或直接或间接使用该项目的任何脚本的使用者都应仔细阅读此声明。本人保留随时更改或补充此免责声明的权利。一旦使用并复制了任何相关脚本或Script项目的规则，则视为您已接受此免责声明。


**您必须在下载后的24小时内从计算机或手机中完全删除以上内容**

> ***您使用或者复制了本仓库且本人制作的任何脚本，则视为 `已接受` 此声明，请仔细阅读***

## 特别鸣谢

- [@hccluck](https://github.com/hccluck/public_actions)

## 更新日志

- 2021-09-06
    * 添加【掘金社区】每日签到抽奖脚本

## 历史 Star 数


## Stargazers over time

[![Stargazers over time](https://starchart.cc/HarrylXue/public_actions.svg)](https://starchart.cc/HarrylXue/public_actions)
