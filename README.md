<div align="center">
  <a href="https://v2.nonebot.dev/store"><img src="https://raw.githubusercontent.com/Harry-Jing/nonebot-plugin-bing-chat/main/resources/NoneBot_Plugin_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
  <br>
  <p><img src="https://raw.githubusercontent.com/Harry-Jing/nonebot-plugin-bing-chat/main/resources/NoneBot_Plugin_text.svg" width="240" alt="NoneBotPluginText"></p>
</div>

<div align="center">

# nonebot-plugin-bing-chat

_✨ 一个可以使用新版Bing进行聊天的插件 ✨_


<a href="./LICENSE">
    <img src="https://img.shields.io/github/license/Harry-Jing/nonebot-plugin-bing-chat.svg" alt="license" />
</a>
<a href="https://pypi.python.org/pypi/nonebot-plugin-bing-chat">
    <img src="https://img.shields.io/pypi/v/nonebot-plugin-bing-chat.svg" alt="pypi" />
</a>
<img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python" />

</div>


## 📖 介绍

一个可以使用新版Bing进行聊天的插件

目前正在完善更多的设置

## 💿 安装

<details>
<summary> <b> 使用 nb-cli 安装（推荐） </b> </summary>
在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装

    nb plugin install nonebot-plugin-bing-chat

</details>

<details>
<summary> <b> 使用包管理器安装 </b></summary>
在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令

    pip install nonebot-plugin-bing-chat


打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入

    plugins = ["nonebot_plugin_bing_chat"]

</details>

## ⚙️ 配置
<details>
<summary> <b> 在 nonebot2 项目的`data/BingChat`文件中添加`cookies.json（必须） </b> </summary>

- 在浏览器安装 `cookie-editor` 的插件 
  - [Chrome/Edge](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm)（需要魔法）
  - [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
- 打开`bing.com`（需要魔法）
- 打开 `cookie-editor` 插件
- 点击右下角的 `Export` 按钮（这会把cookie保存到你的剪切板上）
- 把你复制道德内容放到 `cookies.json` 文件里
 <img src="https://raw.githubusercontent.com/Harry-Jing/nonebot-plugin-bing-chat/main/resources/How_to_export_cookies.png" max-height="100" alt="How_to_export_cookies" />
  
</details>


<details>
<summary> <b> 在 nonebot2 项目的`.env`文件中添加下表中的配置（可选） </b> </summary>


| 配置项 | 必填 | 类型 | 默认值 | 说明 |
|:-----:|:----:|:-----:|:----:|:----:|
| bingchat_allow_group | 否 | Bool | True | 是否允许在群聊中使用 |
| bingchat_command_chat | 否 | str/list[str] | ['chat'] | 对话关键词 |
| bingchat_command_new_chat | 否 | str/list[str] | ['刷新对话'] | 新建对话关键词 |
  
</details>

## 🎉 使用
### 指令表
以下为指令可以在配置文件中更改
| 指令 | 权限 | 需要@ | 范围 | 说明 |
|:-----:|:----:|:----:|:----:|:----:|
| chat | 所有人 | 否 | 私聊/群聊 | 与Bing进行对话 |
| 刷新列表 | 所有人 | 是 | 私聊/群聊 | 新建一个对话 |

  
## 📄 ToDo

<details>
  
  - [ ] 支持更多的适配器
    - [x] onebot-v11
  - [ ] 支持更好的权限管理
    - [ ] 每个人的次数限制
    - [ ] 白名单/黑名单机制
  - [ ] 支持账号自动切换
  - [ ] 更好的错误处理

</details>


  
## 🌸 致谢
- [@A-kirami](https://github.com/A-kirami)  项目使用了README[模板](https://github.com/A-kirami/nonebot-plugin-template)
- [@acheong08](https://github.com/acheong08)  项目使用了与Bing通讯的接口 [EdgeGPT](https://github.com/acheong08/EdgeGPT)
