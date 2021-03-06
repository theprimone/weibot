# bot48

一个关于 SNH48 Group 的 QQ 机器人。已有功能清单：

* 微博自动转评赞（生个h推bot，待整合进 QQ 机器人）

## 准备工作

* Windows 10
* Python 3.7
* 火狐浏览器
* Gecko （火狐浏览器驱动）

浏览器驱动可到 Selenium 官网[下载](https://www.seleniumhq.org/download/)，安装后需要将驱动添加到系统环境变量 Path 中。

由于使用了 [Pipenv](https://docs.pipenv.org/en/latest/) 包管理工具，上述环境就绪后使用 `pipenv install` 安装相关依赖即可使用。

## 快速上手

新建并配置（ utf-8 编码的） `json/mine.json` 中的相关参数，格式如下：

```json
{
  "username": "{username}",
  "password": "{password}",
  "nickname": "{nickname}"
}
```

程序会根据 `json/fcl_users.json` 中的 key 自动转评赞该用户微博，并根据 value 带上话题 tag 。

随后启动 `start.py` 即可。

## 开发计划

见 [Projects / weibot](https://github.com/theprimone/weibot/projects/1)

## 技术剖析

见 [Wiki](https://github.com/theprimone/weibot/wiki)
