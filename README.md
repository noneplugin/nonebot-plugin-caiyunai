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
