[简体中文](README.md) | [繁體中文](README.zh-TW.md) | [English](README.en.md)

# 德州撲克完整原始碼：金幣大廳、MTT/SNG 與 C++ 牌桌服務

本專案聚焦 **德州撲克原始碼、德州原始碼、德州金幣大廳、德州俱樂部原始碼、Texas Holdem source code**。真實畫面涵蓋撲克大廳、經典德州、AOF、短牌入口、MTT、SNG、活動與牌桌；公開程式可核驗 C++ 玩家狀態、盲注、下注池、公牌、保險、牌譜、計時器、Tars GM 服務、MySQL 配置與 Unity/Lua 工具。

> 完整建置仍需倉庫外的協定、框架、服務、設定和資源；實際功能以程式及交付清單為準。

## 產品功能與玩法

- 大廳提供經典德州、AOF、6+ 短牌、排位、私人房與錦標賽入口。
- 一般牌局依序進行底牌、翻牌前下注、翻牌、轉牌、河牌與攤牌。
- 玩家依行動順序選擇過牌、下注、跟注、加注或棄牌。
- MTT/SNG 包含報名、開賽、升盲、桌間平衡與名次結算等產品流程。

## 真實產品畫面

| 大廳與房間 | 錦標賽與牌桌 |
|---|---|
| ![德州撲克金幣大廳](docs/assets/images/poker-lobby.png) | ![經典德州房間](docs/assets/images/classic-holdem.jpg) |
| ![MTT 多桌錦標賽](docs/assets/images/mtt-tournament.jpg) | ![SNG 錦標賽](docs/assets/images/sng-tournament.jpg) |
| ![德州撲克活動](docs/assets/images/events.png) | ![德州撲克牌桌](docs/assets/images/table-win.png) |
| ![多人牌桌與荷官](docs/assets/images/dealer-table.png) | |

## 技術架構

公開程式涵蓋玩家/座位、大小盲、底牌與公牌、下注池、牌譜、保險及等待隊列；C++ 服務端包含遊戲服務、GMServer、Tars 介面、計時器與 MySQL 操作；客戶端資源包含 Unity prefab 及 Lua 網路、資源、音訊與卡牌工具。

## 聯絡與核驗

- Telegram：[@xuzongbin001](https://t.me/xuzongbin001)
- Email：[masterai918@gmail.com](mailto:masterai918@gmail.com)

請說明需要核驗的客戶端、伺服器、資料庫、賽事或部署範圍。

