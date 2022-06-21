# nonebot-plugin-caiyunai

适用于 [Nonebot2](https://github.com/nonebot/nonebot2) 的彩云小梦AI续写插件


### 安装

- 使用 nb-cli

```
nb plugin install nonebot_plugin_caiyunai
```

- 使用 pip

```
pip install nonebot_plugin_caiyunai
```

本插件使用了 [go-cqhttp](https://github.com/Mrs4s/go-cqhttp) 的 `send_group_forward_msg` 和 `send_private_forward_msg` 接口 来发送合并转发消息，

发送私聊合并转发消息需要使用 `v1.0.0-rc2` 版本以上的 go-cqhttp


### 配置

需要在 `.env.xxx` 文件中添加彩云小梦apikey：

```
caiyunai_apikey=xxx
```

apikey获取：

前往 http://if.caiyunai.com/dream 注册彩云小梦用户；

注册完成后，F12打开开发者工具；

在控制台中输入 `alert(localStorage.cy_dream_user)` ，弹出窗口中的 uid 即为 apikey；

或者进行一次续写，在 Network 中查看 novel_ai 请求，Payload 中的 uid 项即为 apikey。


### 使用

#### 触发方式：

**以下命令需要加[命令前缀](https://v2.nonebot.dev/docs/api/config#Config-command_start) (默认为`/`)，可自行设置为空**

```
@机器人 续写/彩云小梦 xxx
```


#### 示例：

<div align="left">
  <img src="https://s2.loli.net/2022/01/15/zKcCMTehNOUxFJI.jpg" width="400" />
  <img src="https://s2.loli.net/2022/01/15/R6HcEuN2gXmsDBJ.jpg" width="400" />
</div>


### 特别感谢

- [assassingyk/novel_ai_kai](https://github.com/assassingyk/novel_ai_kai) 适用hoshino的基于彩云小梦的小说AI续写插件
