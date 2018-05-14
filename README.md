# 米饭产品需求文档

![](/images/logo.png)

## 背景介绍

米饭直播是在如今互联网各大平台推出直播 + 竞猜的产品的背景下，推出的一款新的基于体育赛事直播的竞猜平台。

4 月 14 日，中共中央、国务院发布《关于支持海南全面深化改革开放的指导意见》强调，鼓励海南发展沙滩运动、水上运动、赛马运动等项目，探索发展竞猜型体育彩票和大型国际赛事即开彩票。

米饭的主要竞争对手包括但不限于：虎扑、暴风体育、新浪体育、PP 体育、腾讯体育、秒嗨、直播吧 Pro、懂球帝、企鹅直播、雷速体育、网易红彩、体育疯、JRS 体育、VP 电竞、斗鱼直播、熊猫直播、虎牙直播、一直播、映客直播、花椒直播。

## 迭代计划

|版本|主要功能|
|---|---|
|v0.8|完成直播的主要功能。用户可以查看直播、进行直播、直播中进行礼物打赏。个人账号体系建立，并打通充值和礼物兑换。|
|v0.9|新增竞猜的功能。用户可以针对赛事进行竞猜投注。平台具备结算的能力。竞猜均采用米粒进行投注。|
|v1.0|新增比分的功能。可以查看球队、赛事的历史比分情况，也可按照时间进行查看，辅助用户竞猜决策。同时也作为竞猜的入口。|
|v1.1|新增竞猜和比分互动的功能。在赛事详情中，给出该赛事各个球队在联赛的比分情况，辅助用户竞猜决策。|
|v1.2|新增竞猜和直播互动的功能。主播可以推荐相关竞猜项，观众可根据主播的推荐进行投注。|
|v1.3|新增比分卖料功能。可以让主播、KOL 等用户，在比分中添加内容，包括文字、语音等，分析比分情况，辅助用户竞猜决策。|

## 修订记录

|版本|修订人|修订内容|更新时间|
|---|---|---|---|
|v1.0|程默|完成米饭直播产品设计一期交付的内容。包括直播和竞猜两个主要功能。|2018-05-03|

## 需求文档安装说明

### 环境安装

产品需求文档的运行依赖于 [gitbook](https://github.com/GitbookIO/gitbook)。查看需求文档前，请自行安装 gitbook。

```bash
# Mac 环境下
brew install npm
npm install -g gitbook-cli
```

### 本地运行

改需求文档中包括了一些 gitbook 插件方便用户查看文档。所以运行前请安装插件，再运行服务。

```bash
# 安装 gitbook 插件
gitbook install
# 启动 gitbook 服务
gitbook serve
```

当看到如下信息，则代表安装成功，可以[打开本地服务](http://localhost:4000)。

```bash
...
info: >> generation finished with success in 5.9s !
Starting server ...
Serving book on http://localhost:4000
```
