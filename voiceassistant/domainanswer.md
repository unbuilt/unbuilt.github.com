信息查询
==================

信息查询是语音助手提供的另一主要功能，特别是在某些特定领域：
- 天气预报、空气质量
- 出行:公交、驾车路线、火车车次、飞机班次、限行、路况
- 餐饮
- 酒店
- 股票
- 娱乐：电影、电视、歌曲
- 体育
- 彩票
- 菜谱
- 快递
- 话费、流量
- 违章
- 假期安排
- 利率、汇率

本文将以天气、公交、餐饮这些常用领域为例来体验语音助手信息查询的功能，最后用一组足球比赛查询用例来挑战一下语音助手。


天气预报
-----------

天气预报是信息查询中最常用的领域。

本文采用以下用例来使用语音助手尝试完成查询天气预报的任务。
1. 今天天气怎么样
2. 明天下雨吗
3. 北京的天气怎么样
4. 天津呢

|| 应用 || 用例一 || 用例二 || 用例三 || 用例四 || 任务完成小结 || 语音识别 || 意图识别 ||
|| Siri || A || A || A || A || Siri可以支持各种方式天气查询，并可以给出概要信息，和具体天气情况 || A || A ||
|| 灵犀、语点 || A || A || A || D || 灵犀也可以针对问题给出回答，例如“明天不下雨。” || A || A ||
|| 搜狗语音助手 || A || A || A || A || 搜狗语音助手并不针对问题回答 || A || A ||
|| 百度语音助手 || A || A || A || A || 百度语音助手并不针对问题回答，但是对用例二采用了摘要来回答。 || A || A ||
|| 云知声语音助手 || A || A || A || A || 云知声语音助手并不针对问题回答。 || A || A ||
|| 智能360 || A || A || A || A || 智能360可以理解上下文，对用例四也可以正确回答。 || A || A ||
|| 快说 || A || A || A || D || 快说语音助手并不针对问题回答，也不支持上下文理解。 || A || B ||
|| 哦啦 || A || A || A || A || 哦啦会很好的显示答案，并针对问题进行回答。 || A || A ||
|| 虫洞语音助手 || A || D 显示今天的天气 || A || A || 虫洞语音助手可以理解上下文，但对用例二并不能理解。 || A || B ||
|| 出门问问 || A || A || A || D || 出门问问不支持上下文理解。 || A || B ||

对于最常用的天气查询功能，几乎所有的语音助手都支持得非常好，大部分可以理解上下文，除了显示天气预报外，还可以针对问题进行回答。还有的语音助手在用户查询天气时，除了给出答案，还会提供酒店查询按钮，引导用户。

公交线路
--------

出行是查公交线路也是主要的移动应用。

本文采用以下用例来使用语音助手尝试完成查询公交线路的任务。
1. 到苏州火车站怎么坐车
2. 我想到苏州火车站
3. 从创意产业园到苏州火车站怎么走

|| 应用 || 用例一 || 用例二 || 用例三 || 用例四 || 任务完成小结 || 语音识别 || 意图识别 ||
|| Siri || D || D || D || 用例四 || Siri无法正确确定目标地点，需要用户选择，但是选择后仍无法给出路线。 || A || A ||
|| 灵犀、语点 || B 直接打开百度地图，驾车路线 || B 同用例一 || D 目标地识别错误，直接打开百度地图，无法给出路线 || D || 灵犀识别出此类问题后，打开百度地图查找路线。 || A || B ||
|| 搜狗语音助手 || A- 直接打开搜狗地图，公交路线非最优 || A- 同用例一 || C 直接打开搜狗地图，需确认起点与终点后，给出驾车路线与时间 || A || 搜狗语音助手识别出此类问题后，打开搜狗地图查找路线，有一些默认参数影响了搜索的路线结果 || A || A ||
|| 百度语音助手 || B 经过多次确认地点，公交路线非最优 || B 同用例一 || A || A || 百度语音助手对用例三可以直接显示公路线路。 || A || A ||
|| 云知声语音助手 || B 生成百度地图链接，供用户打开，驾车路线 || D 查询从苏州到苏州的火车 || B 生成百度地图链接，供用户打开，驾车路线 || A || 云知声语音助手识别出此类问题后，生成打开百度地图的链接。 || A || B ||
|| 智能360 || D 查询火车 || D 查询火车 || D 无法找到路线，起点定位错误 || A || 智能360理解查询意图为火车查询。 || A || C ||
|| 快说 || D 查询火车 || D 不能识别意图 || B 经过多次确认地点，公交路线非最优 || D || 快说语音助手生成指向不同地图应用的链接，最终结果由所选择的地图应用决定。 || A || C ||
|| 哦啦 || A 直接给出乘车方案 || D 不能识别意图 || B 列出几条线路，然后进入语音输入模式让用户选择进行导航 || A || 哦啦对于能识别出用户意图的问题可以进行很好的交互。 || A || B ||
|| 虫洞语音助手 || B 经过确认终点，公交路线非最优 || B 同用例一 || D 识别出用户意图，无法正确找到起点 || A || 虫洞语音助手对答案显示较好。 || A || B ||
|| 出门问问 || A 给出乘车方案及路线图 || B 给出驾车时间及路线图 || B 给出驾车时间及路线图 || D || 出门问问可以提供出行方案和路线图，并提示进入地图应用的链接。 || A || A ||

在公交线路查询中，大多数助手都是直接打开地图应用，这样就脱离了语音助手的环境，中断了交互。大多数语音助手的线路查询结果都要比地图应用差，这也是影响用户使用语音助手进行线路查询的原因。

出门问问给出了乘车方案和路线图，这样可以让用户方便的了解具体的路线信息，而且没有脱离交互环境，在这一组用例上表现最好，确实是为出行而生，也从Google Now上学到了很多。


餐饮美食
--------

民以食为天，餐饮是另一个主要的查询功能。

本文采用以下用例来使用语音助手尝试完成查询餐饮的任务。
1. 附近有什么吃的
2. 附近有没有必胜客
3. 观前街有什么美食

|| 应用 || 用例一 || 用例二 || 用例三 || 用例四 || 任务完成小结 || 语音识别 || 意图识别 ||
|| Siri || D || D || D || 用例四 || Siri无法正确确定目标地点，需要用户选择，但是选择后仍无法给出路线。 || A || A ||
|| 灵犀、语点 || B 直接打开百度地图，驾车路线 || B 同用例一 || D 目标地识别错误，直接打开百度地图，无法给出路线 || D || 灵犀识别出此类问题后，打开百度地图查找路线。 || A || B ||
|| 搜狗语音助手 || A || A || A || A || 搜狗语音助手 || A || A ||
|| 百度语音助手 || A || A || A || A || 百度语音助手不仅列出餐饮，而且在地图上进行显示。 || A || A ||
|| 云知声语音助手 || A || D || D || A || 云知声语音助手只能显示附近的餐饮。 || A || B ||
|| 智能360 || C || D || A || A || 智能360。 || A || C ||
|| 快说 || A || C 位置不正确 || B 非餐饮列表 || D || 快说语音助手。 || A || B ||
|| 哦啦 || A || A || A || A || 哦啦可以列出餐饮，并提示可以选择导航。 || A || B ||
|| 虫洞语音助手 || A || A || A || A || 虫洞语音助手对答案显示较好，显示附近的优惠券引导用户，但是没有给出餐饮的距离。 || A || B ||
|| 出门问问 || A || A || A || || 出门问问显示列表及地图，并显示电话、距离等必要信息和导航等相关链接。 || A || A ||

在餐饮查询中，大多数助手都可以给出餐饮列表，提供电话、距离等信息。一些语音助手还显示出了地图。

出门问问给出的信息全面、界面清晰、附加功能丰富，体验要好于其他语音助手。


