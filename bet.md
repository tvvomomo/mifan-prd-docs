# 竞猜

![](/images/bet-list.png)

竞猜页面在信息层级上分为 2 级：

* 赛事列表页 - 列出今日的比赛，和所有的赛事列表，作为赛事详情的入口。
* 赛事详情页 - 显示赛事的详细信息、相关直播，以及赛事所有的竞猜类型，供用户投注使用。

## 赛事列表页

如上图的赛事列表页，该页共包含两块：

* 今日赛事 - 所有以北京时间为基准的今日内的赛事，在头部以左右列表的形式排列，可以左右滑动。
* 所有赛事 - 所有赛事以【全部】和【联赛名称】为 TAB 区隔开，用户可筛选。所有赛事下的赛事以距离当前时刻的时间的正序排列，即越靠近当前时间的赛事越往上。

### 今日赛事

今日赛事是指，所有以北京时间为基准的今日内的赛事。即当地时间为明日的赛事，根据时区换算，中国观众会在北京时间的今日收看的比赛，都算作是今日赛事。

而竞猜中心里所有赛事的时间显示，都以北京时间为准。

今日赛事所包括的功能：

* 单个赛事卡片包含以下信息：
  * 主场名称
  * 主场 image
  * 客场名称
  * 客场 image
  * 联赛信息
  * 对战北京时间
* 今日赛事从左至右按照距离当前时刻的时间的正序排列，即越靠近当前时间的比赛越靠左。
* 今日赛事可以左右滑动来查看赛事列表。
* 点击单个赛事卡片，进行该赛事详情页。

### 所有赛事

所有赛事是指，显示平台所抓取的所有还未结束的比赛。竞猜中心和未来的比分功能中所有赛事的区别在于：

* 竞猜中心 - 显示所有还未结束的比赛，供用户投注使用。
* 比分 - 显示已经结束、正在进行中的比赛，辅助用户投注决策。

所有比赛，按照以下的联赛进行分类：

* 全部
* 世界杯
* 英超
* 等，但不限于此。以运营的需求为准。

所有赛事卡片可以实现的交互：

* 上线滑动 - 实现赛事的上下滚动查看，赛事按照距离当前时刻的时间的正序排列，即越靠近当前时间的比赛越往上。
* 左右滑动 - 实现联赛的左右切换。联赛的排列以运营的需求为准。
* 点击单个赛事卡片，进行该赛事详情。

## 赛事详情

![](/images/bet-detail.png)

赛事详情共包括以下的部分：

* 赛事信息
  * 联赛信息
  * 赛事时间
  * 主场名称
  * 主场名称
  * 主场得分 - 仅进行中的比赛会包含得分信息
  * 客场名称
  * 客场名称
  * 客场得分 - 仅进行中的比赛会包含得分信息
* 相关直播
  * 电视直播，或其他平台（有转播版权的）的相关信息
  * 米饭直播相关的直播间
* 竞猜单元列表

### 相关直播

相关直播共包括两部分：

* 直播相关信息
* 米饭直播相关直播间

直播相关信息是指，其他平台，包括体育视频网站、体育直播平台、电视转播等其他平台的直播信息。直播信息包括：

* 其他平台名称
* 直播的北京时间

点击直播相关信息卡片：

* 若用户开启了 App 通知，则该时间信息会保存在个人中心的我的预约里，等到时间到来的前 5 分钟，米饭直播会通过推送信息提醒用户查看直播。
* 若用户未开启 App 通知，则调用 OS 开启推送的功能，提示用户开启推送。
  * 若用户开启了通知，则如上会等到赛事到来前 5 分钟提醒用户。
  * 若用户未开启通知，则返回到赛事详情。

米饭直播相关直播间，是指主播在开启直播时会选择直播相关的：

* 联赛
* 联赛中的比赛

在米饭相关直播间，会列出所有与该联赛下的比赛相关的所有直播间。点击直播间卡片，则打开直播观看。

### 竞猜

竞猜卡片会列出所有该赛事可投注的竞猜信息。

在一期需求范围内，竞猜类型仅包括足球赛事。竞猜类型的详细信息，请参见[第三方 API、SDK 文档](/thirdpart.html)。

以下内容由产品整理，内容采集自网络。若存在疏漏，请研发及时反馈：[足球投注类型](/soccers-types.html)

点击投注单元，竞猜单会产生 **[+1]** 动效：

* 若用户走默认配置，需要点击竞猜单，查看投注，最终确认投注。
* 若用户开启了【自动投注】的功能，则确认投注。

*注：自动投注可以在个人中心的竞猜配置里进行设置。*

有关投注的功能请查看：[竞猜 - 投注](/betting.html)

![](/images/bet-detail-more.png)

竞猜列表的交互说明，若用户上滑竞猜列表：

* 头部 banner 收缩至显示：
  * 主场 image
  * 主场得分
  * 客场 image
  * 客场得分
* 【相关直播】和【竞猜列表】是作为一个视图，上滑时，一起移动

若用户点开某个竞猜类型，如全场波胆中胜更多的选项，则：

* 向下展开更多投注单元
* 页面自动上滑至内容视图的顶部

*注：内容视图是指除去头部卡片外，相关直播和竞猜列表的所有内容所在的视图。*