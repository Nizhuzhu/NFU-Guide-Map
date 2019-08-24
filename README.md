<div align=center>

![QRcode](https://656e-enanyuan-6db383-1257936504.tcb.qcloud.la/showcase/QRcode.jpg?sign=2f3aa5f8f9a8edc282ff67a20fb6deae&t=1566624511)

</div>

# 南苑导览 · [![GitHub license](https://img.shields.io/github/license/observer-l/NFU-Guide-Map)](https://github.com/Observer-L/NFU-Guide-Map/blob/master/LICENSE) [![test](https://img.shields.io/badge/platform-微信小程序-green)]() [![GitHub stars](https://img.shields.io/github/stars/observer-l/NFU-Guide-Map)](https://github.com/observer-l/NFU-Guide-Map/stargazers)

南苑导览是一款由学生独立开发的以地图为载体，提供**中山大学南方学院**（南苑）具体地点的位置信息、导航、校园历史及文化介绍的小程序。旨在解决校园导航标识不到位、地图形式低效单一、信息设计不够好等问题，为来南苑新人和游客提供更加完美的出行体验。

<div align=center>

**仅需修改地图配置文件，即可适配任意场景（校园、景区）的小程序个性化地图定制。**

原生小程序 + TypeScript + gulp + vantUI + 云开发能力

项目开源，持续维护，欢迎[反馈](issues)、 [PR](pulls) 和 Star⭐️！

</div>

## ⚡️ 功能

✅ 路线推荐  
✅ 路线规划  
✅ 地点搜索  
✅ 校园留言板  
✅ 人文地理信息一览  
✅ 景点分类动态展示  
✅ 全景看景（功能已实现，个人类小程序受限，暂未开放）  
🔲 社团、商铺信息互联互通

## 📋 使用指南

1. 在根目录 config 中，根据自身需求修改应用配置

```javascript
—— src
——— config
————— index.ts // 入口
————— cloud.ts // 云开发相关配置
————— info.ts // 应用介绍信息
————— markerStyle.ts // 地图marker样式
————— panorama.ts // 第三方全景地图配置（个人类型无webview权限，默认关闭）
————— secret.ts // 腾讯地图key等敏感信息（可选）
```

2. 在开发环境中，如不使用云开发能力，可以使用本地 mock 数据

```javascript
—— src
——— mock
————— index.ts // 入口
————— board.ts // 公告
————— comments.ts // 留言
————— markers.ts // 地点
————— routes.ts // 路线推荐
```

1. 本项目使用 excel 管理数据，使用 python pandas 来清洗数据，数据格式及使用说明详[见此](example)。

2. 通过 npm 使用第三方 UI 组件库[VantUI](https://youzan.github.io/vant-weapp/#/intro)，因此需要在开发工具中进行 npm 构建，详细操作见[小程序文档 - npm 支持](https://developers.weixin.qq.com/miniprogram/dev/devtools/npm.html)。

3. 起飞：

```
npm install
npm run dev
```

## 🔩 分支管理

```
NFU-Guide-Map
  ├─ master       // 默认分支
  ├─ wepy@1.7.2       // 使用wepy框架开发的初始版本，在wepy2和框架踩坑的权衡之后停止维护，用原生重写
  └─ [other]      // 其他开发分支（只允许该项目Collaborators创建及push分支）
```

## 📄 版本日志

每个版本详细的迭代记录在[release notes](releases)。

## 📷 影像资源版权说明

本项目所用影像收集自校园官网、在校师生，社团组织。版权所有，未经允许，禁止盗用。

## 参考资料

- [小程序 API 文档](https://tencent.github.io/wepy/)

- [玩转故宫 · 小程序](https://img.91ud.com/FgTgB47bc6dmAACekIjFxLO342mW/256)

- [莞香广科 · 校园导览](https://github.com/gxgk/school-map)

- [wxapp-typescript-demo](https://github.com/godbasin/wxapp-typescript-demo)

## LICENSE

「南苑导览」使用[MIT license](LICENSE)
