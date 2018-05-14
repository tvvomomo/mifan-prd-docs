# 直播观看

![](/images/watch-bet-list-v.png)

直播观看页面共包含以下功能：

* 观看相关
  * 横屏 \ 竖屏 观看，以及切换
  * 暂停直播
  * 返回上一页
* 竞猜相关
  * 查看直播所对应的赛事，赛事所对应的所有投注列表
  * 点击投注单元，进行投注
  * 查看竞猜单
  * 查看竞猜榜
* 互动功能
  * 查看弹幕，弹幕包括：
    * 文本讨论信息
    * 礼物发送信息
  * 输入文本信息
  * 赠送礼物
  * 查看礼物榜
* 分享
  * 分享至微博、微信好友、微信朋友圈、QQ 好友

## 竞猜功能

竞猜是直播观看的主要功能，是指在观看直播的过程中，对下方竞猜列表的投注单元，进行点选后，确认下注的过程。其中涉及的操作：

|操作步骤|设计图|
|---|---|
|1. 查看竞猜列表|![](/images/betting-list-v.png)|
|2. 选择投注单元|![](/images/watch-bet-list-v.png)||
|3. 查看投注单元|![](/images/betting-v.png)|
|4. 输入投注金额|![](/images/betting-input-v.png)|
|5. 确认投注|点击确认竞猜按钮后，若后端接口返回成功，则数量 icon 变成成功符号，确认竞猜变成成功符号后，停留 60s 后关闭竞猜单。回到打开竞猜单的原页面。|

其中有关投注的细节需求说明，请见：[竞猜 - 投注](/betting.html)。

除此之外，在竖屏模式下，用户可以点选竞猜榜，查看该直播间所对应的比赛的投注单元排名情况。目前排名可以按照以下两种方式进行排序：

1. 购买人数的倒序排列。即购买人数越多的投注单元越靠上。
2. 目前平台预测收益率的倒序排列。即预测对平台收益越大的投注单元越靠上。

竞猜榜中的投注单元也可点击加入竞猜单中，和竞猜列表中的投注单元一样。

![竞猜榜](/images/watch-bet-hot-v.png)

## 互动功能

互动功能包括了以下功能：

* 弹幕观看
* 发弹幕
* 赠送礼物
* 查看直播间礼物
* 查看礼物榜

|功能|设计图|
|---|---|
|弹幕观看|![](/images/watch-discuss-v.png)|
|赠送礼物|![](/images/watch-gift-v.png)
|礼物榜|![](/images/watch-gift-hot-v.png)

由于以上功能通用，且目前的产品中已经包含，所以不再赘述。

其中特别说明的是，目前产品中可以一次性批量赠送礼物。如下图所示：

![修改礼物数量](/images/watch-gift-input-v.png)

## 横屏 / 竖屏观看

![](/images/watch-h.png)

### 竞猜横屏 / 竖屏

|名称|水平图|垂直图|
|---|---|---|
|竞猜列表|![](/images/betting-list-h.png)|![](/images/betting-list-v.png)|
|竞猜列表 - 点选|![](/images/betting-selected-h.png)|![](/images/watch-bet-list-v.png)|
|竞猜单|![](/images/betting-h.png)|![](/images/betting-v.png)|
|竞猜单 - 输入|![](/images/betting-input-h.png)|![](/images/betting-input-v.png)|

### 互动横屏 / 竖屏

|名称|水平图|垂直图|
|---|---|---|
|弹幕|![](/images/watch-discuss-h.png)|![](/images/watch-discuss-v.png)|
|礼物|![](/images/watch-gift-h.png)|![](/images/watch-gift-v.png)|


## 其他功能

### 分享

![直播内容分享](/images/watch-share.png)

目前直播间可以分享至：

* 微信朋友圈
* 微信好友
* 新浪微博
* QQ 好友

### 修改分辨率

![修改分辨率](/images/watch-resolution.png)
