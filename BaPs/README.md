![introduce](https://socialify.git.ci/gucooing/BaPs/image?description=1&font=Source+Code+Pro&forks=1&issues=1&language=1&name=1&owner=1&pattern=Plus&pulls=1&stargazers=1&theme=Light)

# BaPs-Lite 🎮

#### [English](README_EN.md)

> ⚠️ 项目仅供学习用途，严禁用于商业用途，请于24小时内删除。

# 仅供学习用途，严禁用于商业用途，请于24小时内删除！！！

> 🌟 由于是无状态设计,所以对内存的要求会略高

> 📅 当前支持版本：Japan 1.58.349018

## 📍Discord

[![Discord](https://img.shields.io/badge/Join-Discord-blue?logo=discord&logoSize=auto)](https://discord.gg/222yVp6pUq)


---
## 🚀 已实现功能
```
- 登录  
- 新手教程  
- 队伍管理
- 抽卡  
- 剧情 待测试  
- 账号基础管理  
- MomoTalk  
- 邮件 全局/私人 收发管理  
- 角色养成管理  
- 背包管理  
- 副本 - 悬赏通缉 / 特别依赖 / 学院交流会 / 综合战术考试  
- 可恢复品自动恢复  
- 咖啡厅  
- 好友管理  
- 课程表  
- 社团  
- 战斗援助  
- 总力战  
- 彩奈登录奖励  
- 制约解除决战  
- 大决战  
- 商店
- 角色好感系统
- 竞技场
- 贴纸
- 走格子战斗
```
---
## 使用协议

```
1. 禁止传播
严禁在中国大陆地区的任何公共或私有平台上传、分享或宣传本项目的源码、编译文件、部署教程、截图、演示视频等相关内容；
若发现违规传播行为，作者有权采取封禁、公开拉黑等措施。

2. 禁止开服
严禁使用本项目进行任何形式的私服搭建，包括但不限于公网开服、内网搭建、测试服部署；
无论是否收费、是否开放给他人使用，均视为违反本协议；
一经发现，作者将永久停止支持，并可能公开违规行为及其责任人信息。

3. 免责声明
本项目仅供技术研究与学习之用；
使用者应自行承担由本项目引发的一切法律责任，与项目作者无关；
任何因传播本项目所引发的法律责任，均由最终传播者承担。

4. 协议更新
本协议可随时更新，使用即视为接受协议的所有内容及后续变更。
```

## 重要内容！！！！！！

1. Lite版只能在内网环境下运行且移除了大部分功能 (目前仍在考虑是否进一步锁紧功能)
2. Lite版的api没有密码且内置了远程shell便于调试,所以如果你违反使用协议在公网环境下运行造成的后果自行承担
3. 没有遵守我们使用协议的任何行为所造成的后果皆自行承担与我们组织和开发者无任何关系
4. 一旦下载了BaPs的任何文件都代表您同意了使用协议
5. 仅供学习用途，严禁用于商业用途，请于24小时内删除！！！
6. 如若此项目侵犯了您的权益可联系删除

## 🛠️ 使用方法

1. 前往[唐人](https://github.com/gucooing/BaPs?tab=readme-ov-file#-%E5%90%8D%E4%BA%BA%E5%A0%82)处了解详情
2. 如果你没看第一条那就回去看！！！别跳了！！！
3. 前往[Action BaPs_Server_Build](https://github.com/BanterSR/free/actions/workflows/BaPs_Server_Build.yml)下载最新的版本和`data.zip`文件
4. 完全解压data.zip文件到运行目录
5. 使用参数```-g true```运行一次将会自动生成config.json文件,打开并编辑config.json文件
6. 需要注意的是部分设置你无法进行更改,这是Lite版本的限制
7. 运行

---

## ⚙️ 配置说明
>需要注意的是,实际的json文件中不能存在注释,没有标明的配置是不能修改的
```json
{
  "Resources": {
    "ClientResPath": "./clientRes", // res 路径
    "DataPath":      "./data", // data路径
    "ExcelBinPath":  "./data/Excel.bin" // excel bin 路径
  },
  "Tutorial": true, // 是否开启教程
  "OtherAddr": {
    "ServerInfoUrl": "https://yostar-serverinfo.bluearchiveyostar.com", // 上游服务器地址 如果值为: 'local' 时使用本地文件
    "ManagementDataUrl": "https://prod-noticeindex.bluearchiveyostar.com/prod/index.json" // 公告地址
  },
  "HttpNet": {
    "InnerIp": "0.0.0.0", // 监听IP
    "InnerPort": "5000", // 监听端口
    "CertFile": "./data/cert.pem",
    "KeyFile":   "./data/key.pem"
  },
  "GateWay": {
    "MaxCachePlayerTime": 720, // 最大玩家缓存时间
    "BlackCmd": {} // 发行版无用
  },
  "DB": {
    "dbType": "sqlite", // 使用的数据库类型,支持sqlite和mysql
    "dsn": "BaPs.db" // 数据库地址,如果是mysql请填写mysql url
  },
  "RaidRankDB": {
    "dbType": "sqlite", // 使用的数据库类型,支持sqlite和mysql
    "dsn": "Rank.db" // 数据库地址,如果是mysql请填写mysql url
  },
  "Irc": { // 可使用通用irc服务器地址
    "HostAddress": "127.0.0.1", // 社团聊天服务器irc地址
    "Port": 16666, // 社团聊天服务器irc端口
    "Password": "mx123" // 社团聊天服务器irc密码
  }
}
```
---

## 🌐 代理设置
转代以下地址:其中 http://127.0.0.1:5000 为服务器地址
```plaintext
https://ba-jp-sdk.bluearchive.jp  →  http://127.0.0.1:5000
https://yostar-serverinfo.bluearchiveyostar.com → http://127.0.0.1:5000
```

### ⛓️代理方案

可前往以下docs查看
- [Android_MitmProxy代理方案](Android_Mitmproxy.md)

---

## ⌨️ GM工具

1. 推荐的GM [BlueArchiveGM](https://github.com/PrimeStudentCouncil/BlueArchiveGM/releases/latest);web版: [BlueArchiveGM Web](https://gm.bluearchive.cc)
2. 我们欢迎更多开发者开发适用于BaPs的GM

---

## 进阶操作
1. BaPs支持第三方sdk登录，仅需适配VerifyTokenUrl即可接入任意的sdk

---
## 🤝 参与贡献
我们欢迎所有想帮助我们的人加入，可通过以下方式进行帮助我们：
- 🐛 提交Issue报告问题
- 💡 提交Pull Request改进代码
- 📖 完善项目文档
- 🚀 加入Discord频道为我们提供建议
---

## ⚠️ 注意事项
1. 由于版权原因，dev使用的resources我们不会公开
2. 由于唐人原因，全部源代码将不会被公开，但我们可以保证非公开部分代码无任何恶意内容（在你遵守我们使用协议的情况下）
3. 玩家数据并不会实时保存到数据库中,如果有最新数据的需求,可通过api进行访问玩家数据
4. 该项目不支持,也不会适配32位系统

---
## 🤜 感谢名单

- 感谢 [zset](https://github.com/liyiheng/zset) 以此为基础实现排行榜
