# Contributing / 评分规范

## 文件命名

- 店文件：`restaurants/<area>/<slug>.md`
  - `<area>` 用英文：`central` / `wan-chai` / `causeway-bay` / `tst` / `mongkok` / `jordan` / `sham-shui-po` / `hkust` 等
  - `<slug>` 用店名英文或拼音，短横线分词：`no-2-cafe` / `assam-chicken-rice` / `shi-er-wei-kt`
- 照片：`photos/<slug>/<描述>.jpg`，如 `photos/assam-chicken-rice/chicken-rice.jpg`
- 主题列表：`lists/<主题英文>.md`，如 `lists/dim-sum.md`

## 店文件模板

见 [`restaurants/_template.md`](restaurants/_template.md)。关键字段：

- 顶部 YAML-like 列表：地址、电话、营业、菜系、价位、最近访问
- 评分表：四项 + 综合
- 推荐菜 / 避雷菜（可空）
- 感受：一两段，写清楚为什么给这个分
- 照片：可选，`![描述](../../photos/<slug>/xxx.jpg)`

## CSV 字段

`data/restaurants.csv`：

| 字段 | 类型 | 说明 |
|---|---|---|
| slug | str | 与文件名一致 |
| name | str | 店名 |
| area | str | 地区英文 slug |
| area_cn | str | 地区中文 |
| cuisine | str | 菜系，分号分号 |
| price | str | $ / $$ / $$$ / $$$$ |
| taste | float | 0–10 |
| environment | float | 0–10 |
| service | float | 0–10 |
| value | float | 0–10 |
| overall | float | 加权后综合 |
| last_visited | date | YYYY-MM-DD |
| must_order | str | 必点菜，分号分隔 |
| url | str | 官网/OpenRice 链接 |

## 主题列表写法

`lists/<主题>.md` 是一个分类视图，不是新内容。格式：

```markdown
# 早茶 Dim Sum

按综合评分降序。

| # | 店 | 地区 | 分 | 必点 |
|---|---|---|---|---|
| 1 | [新兴食家](../restaurants/kennedy-town/sun-hing.md) | 坚尼地城 | 7.5 | 流沙包、风爪、虾饺、炸鲜奶 |
```

## 评分原则

- 吃过两次以上才打综合分，一次性的只写感受不打分。
- 分数会随时间调整，不追求"客观"，追求"下次自己翻能信"。
- 避雷菜只写自己点过且觉得不行的，不道听途说。
