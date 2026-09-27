[简体中文](README.md) | [繁體中文](README.zh-TW.md) | [English](README.en.md)

# 德州扑克完整源码：金币大厅、MTT/SNG 与 C++ 牌桌服务

面向 **德州扑克源码、德州源码、德州金币大厅源码、德州俱乐部源码、Texas Holdem source code** 的多端项目资料。真实界面覆盖扑克大厅、经典德州、AOF、短牌入口、MTT 多桌锦标赛、SNG、活动与牌桌操作；公开代码可核验 C++ 玩家/房间状态、大小盲、下注池、公牌、保险、牌谱、计时器、Tars GM 服务、MySQL 配置，以及 Unity/Lua 工具资源。

> 公开仓库是源码与资源集合。完整编译仍依赖仓库外的协议、框架、服务、配置与资源；上线范围应以实际交付清单和测试结果为准。

## 产品功能与玩法

| 模块 | 玩家体验 | 仓库/截图依据 |
|---|---|---|
| 多模式大厅 | 经典德州、AOF、6+ 短牌、排位、私人房和赛事入口 | `Screenshots/大厅.png` |
| 经典牌桌 | 盲注、买入、座位、下注、跟注、加注、弃牌与公共牌 | `context.*`、`user.*`、牌桌截图 |
| MTT 锦标赛 | 多桌赛事列表、报名状态与倒计时 | MTT 产品截图、比赛配置结构 |
| SNG | 不同买入与奖励档位的 Sit & Go 赛事入口 | SNG 产品截图 |
| 局内记录 | 玩家信息、下注池、牌谱步骤、收藏与结算数据 | `context.*` |
| 活动呈现 | 活动入口、奖励进度和大厅运营界面 | 活动产品截图 |

## 德州扑克流程

玩家从大厅选择模式和房间，确认盲注或赛事报名条件后入座。牌局依次经历发底牌、翻牌前下注、翻牌、转牌、河牌和摊牌；玩家可根据行动顺序选择过牌、下注、跟注、加注或弃牌。MTT/SNG 还需要报名、开赛、升盲、桌间平衡和名次结算流程。

## 真实产品截图

| 大厅与模式 | 牌桌与赛事 |
|---|---|
| ![德州扑克金币大厅与模式入口](docs/assets/images/poker-lobby.png) | ![经典德州扑克房间配置](docs/assets/images/classic-holdem.jpg) |
| ![德州扑克 MTT 多桌锦标赛](docs/assets/images/mtt-tournament.jpg) | ![德州扑克 SNG 赛事](docs/assets/images/sng-tournament.jpg) |
| ![德州扑克活动中心](docs/assets/images/events.png) | ![德州牌桌下注与公共牌](docs/assets/images/table-win.png) |
| ![多人德州牌桌与荷官](docs/assets/images/dealer-table.png) | |

## 技术结构

- **牌桌状态：** 玩家、座位、大小盲、底牌、公牌、下注池、等待队列与游戏详情。
- **流程计时：** 开始/结束计时器、操作时间和客户端计时广播。
- **服务接口：** C++ 游戏服务、GMServer、Tars servant 与外部工厂入口。
- **数据层：** MySQL 操作与比赛基础配置结构。
- **客户端资源：** Unity prefab 与 Lua 网络、资源、音频、卡牌和俱乐部工具。

## 构建与二次开发

`makefile` 引用了多个仓库外的 Tars/XGame 协议和服务模块。构建前需补齐依赖、数据库结构、服务配置和客户端工程，并对下注边界、边池、全下、断线重连、牌型比较、结算与赛事流程建立测试。

## 在线图文文档

- [简体中文](https://masterai-top.github.io/Texas-Holdem-Poker-Complete-Source-Code/zh-cn/)
- [繁體中文](https://masterai-top.github.io/Texas-Holdem-Poker-Complete-Source-Code/zh-tw/)
- [English](https://masterai-top.github.io/Texas-Holdem-Poker-Complete-Source-Code/en/)

## 联系与项目核验

- Telegram：[@xuzongbin001](https://t.me/xuzongbin001)
- Email：[masterai918@gmail.com](mailto:masterai918@gmail.com)

联系时请说明需要核验的客户端、服务端、数据库、赛事或部署范围。

