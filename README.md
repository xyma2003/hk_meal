# Hong Kong Eats 🇭🇰

A curated list of restaurants I've actually eaten at and would go back to.
Organized by area, with honest ratings, must-orders, and notes.

> 评分纯属个人口味，欢迎约饭。

## What's inside

```
hk_meal/
├── README.md              # 你正在看的这份
├── data/
│   └── restaurants.csv    # 结构化数据，可检索/排序
├── restaurants/           # 每家店一个 md 文件，按地区归档
│   ├── central/           # 中环
│   ├── wan-chai/          # 湾仔
│   ├── causeway-bay/      # 铜锣湾
│   ├── tst/               # 尖沙咀
│   ├── mongkok/           # 旺角
│   └── ...
├── lists/                 # 主题合集（早茶/宵夜/米其林…）
├── photos/                # 店照片，按店 slug 分子目录
│   └── <slug>/
└── CONTRIBUTING.md        # 评分标准、模板说明
```

## Rating system

每家店四项打分，各 0–10：

| 维度 | 含义 |
|---|---|
| 味道 Taste | 核心因素 |
| 环境 Vibe | 装修、噪音、桌距 |
| 服务 Service | 态度、效率（不苛求） |
| 性价比 Value | 对得起价 |

**综合评分** = 味道 × 0.5 + 环境 × 0.15 + 服务 × 0.15 + 性价比 × 0.2，四舍五入到一位小数。

参考区间：
- **9.0+** 必吃，会带朋友去
- **8.0–8.9** 很好，值得专门跑
- **7.0–7.9** 不错，路过会吃
- **6.0–6.9** 一般，有更好的替代
- **<6** 避雷

## Price

| 标记 | 人均 HKD |
|---|---|
| `$` | <100 |
| `$$` | 100–200 |
| `$$$` | 200–400 |
| `$$$$` | 400+ |

## Index

### By area

| 地区 | 店数 | 平均分 |
|---|---|---|
| 中环 Central | – | – |
| 湾仔 Wan Chai | – | – |
| 铜锣湾 Causeway Bay | – | – |
| 尖沙咀 TST | – | – |
| 旺角 Mongkok | – | – |

> 填写后用 `data/restaurants.csv` 脚本生成。

### By list

- [早茶 Dim Sum](lists/dim-sum.md)
- [茶餐厅 Cha Chaan Teng](lists/cha-chaan-teng.md)
- [粥粉面 Congee & Noodles](lists/congee-noodles.md)
- [宵夜 Late Night](lists/late-night.md)
- [米其林/必比登 Michelin](lists/michelin.md)
- [甜品 Dessert](lists/dessert.md)
- [东南亚 Southeast Asian](lists/southeast-asian.md)
- [台式 Taiwanese](lists/taiwanese.md)
- [川菜 Sichuan](lists/sichuan.md)
- [韩式 Korean](lists/korean.md)
- [约会 Date Night](lists/date-night.md)
- [已关店 Closed 🕊️](lists/closed.md)

### Top 10

> 按综合评分排序，至少吃过一次才会进榜。

| # | 店 | 地区 | 菜系 | 分 |
|---|---|---|---|---|
| – | – | – | – | – |

## How to add a restaurant

1. 复制 [`restaurants/_template.md`](restaurants/_template.md)。
2. 重命名后放进对应地区目录，文件名用店名英文 slug（如 `yat-lok.md`）。
3. 填内容，照片放 `photos/<slug>/`。
4. 在 `data/restaurants.csv` 加一行。
5. 视情况加进某个 `lists/*.md`。

详细规范见 [`CONTRIBUTING.md`](CONTRIBUTING.md)。

## Notes

- 所有评价基于**自费**用餐，不接受招待。
- 最近一次访问时间写在店文件顶部，超过两年没回访的评分会标"过时"。
- 营业时间、地址可能变动，去之前自己再查一遍。
