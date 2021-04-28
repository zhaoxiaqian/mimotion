> 小米运动 微信步数 支付宝步数

#### VPS部署
```bash
wget --no-check-certificate -O mimotion.sh https://raw.githubusercontent.com/mixool/mimotion/main/mimotion.sh
chmod 755 mimotion.sh
bash mimotion.sh 18812345678@password@10000-20000
```

| 参数 | 说明 |
| -------- | ----- |
| `18812345678@password@10000-20000` | 账号@密码@随机步数起止点,可多次传入支持多账号 |
| `deviceId@*************` | 设备ID,无则使用随机ID |
| `token@*** chat_id@***` | telegram bot通知所需参数,无则不进行信息通知 |
| `ding_token@*** ding_secret@***` | 钉钉机器人通知所需参数,无则不进行信息通知 |
| `others` | 其它说明查看脚本内容 |

* 小米运动app步数不会更新,仅更新关联应用  

* 默认每天18:35随机延迟任务1-20秒运行一次,自行按需调整   

* 微信排行榜开关:微信-设置-通用-辅助功能-微信运动-隐私及提醒设置  

* 支付宝排行榜开关:支付宝运动-...-设置  

* 因各种原因,不提供任何定时运行脚本,推荐在本地运行  

#### thanks:  
* jd_docker
* [mimotion](https://github.com/Squaregentleman/mimotion)
