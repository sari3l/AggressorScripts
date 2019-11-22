# Message Pusher

用于推送新 beacon 上线，目前配合 BotPush 实现 telegram bot 机器人推送

## 配置

![](https://github.com/sari3l/AggressorScripts/blob/master/MessagePusher/pics/messagepusher_1.png)

1. 修改 gui.cna 第一行中的 `<path>` 为jar文件所在绝对路径

    ```sleep
    import content.Main from: /<path>/BotPush.jar;
    ```

### 注意：

1. 由于 telebot 证书要求 CN 为所在域名或 IP，因此需要在设置中选择使用`私有证书`
2. 在 url 中需设置消息传递占位符，与占位符中的内容一致
3. 选择传递时的编码模式，目前支持 `urlencode` 以及 `base64`

## 效果

![](https://github.com/sari3l/AggressorScripts/blob/master/MessagePusher/pics/messagepusher_2.png)
