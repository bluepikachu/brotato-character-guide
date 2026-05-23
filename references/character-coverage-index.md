# Character Coverage Index

用于快速判断某个角色应该查哪些来源，减少无效读取。

## Fast path

- 默认先查：`steam-guide.md` + `jump-guide.md` + `term-glossary.md`
- 如果这三者已经足够回答，就不要继续扩源

## By source

### steam-guide.md

- 覆盖范围最大
- 包含：
  - 基础角色
  - 深渊恐惧 DLC 角色
  - `驯兽师`
  - `没有付出就没有收获的免费更新` 相关说明
- 适合当作所有角色问题的第一入口

### jump-guide.md

- 覆盖基础角色 + 深渊恐惧 DLC 角色
- 当前包含：
  - `浪漫之人`
  - `水手`
  - `好奇之人`
  - `建造者`
  - `船长`
  - `生物`
  - `厨师`
- 当前不包含：
  - `驯兽师`

### bilibili-guide.md

- 覆盖基础角色 + 一批 DLC 角色
- 包含到：
  - `浪漫之人`
- 不包含：
  - `驯兽师`
- 适合在 `Steam` / `JUMP` 不够时补单角色长文细节

### xiaoheihe-guide.md

- 主要覆盖基础角色
- 额外包含：
  - `驯兽师`
- 不包含大多数 DLC 角色

### epic-guide.md

- 只覆盖少数角色
- 当前明确覆盖：
  - `全能者`
  - `农夫`
  - `幽灵`
  - `飞毛腿`
  - `医生`
  - `独臂`
  - `受虐狂`
  - `骑士`
  - `恶魔`

### build-site-guide.md

- 覆盖大量基础角色和 DLC 角色
- 适合：
  - 补 `Tier`
  - 补结构化字段
  - 在主来源缺细节时兜底
- 不要默认先查，只有在需要 `Tier` 或结构化补充时再查

## Quick skip rules

- 问 `驯兽师`：
  - 先查 `steam-guide.md`
  - 再查 `xiaoheihe-guide.md`
  - 跳过 `jump-guide.md` 和 `bilibili-guide.md`

- 问 `水手`、`好奇之人`、`建造者`、`船长`、`生物`、`厨师`：
  - 先查 `steam-guide.md`
  - 再查 `jump-guide.md`
  - 需要 `Tier` 或结构化字段时再补 `build-site-guide.md`
  - 通常跳过 `xiaoheihe-guide.md`

- 问 `德鲁伊`、`矮人`、`匪徒`、`潜水员`、`徒步旅行者`、`海盗`、`食人魔`、`浪漫之人`：
  - 先查 `steam-guide.md`
  - 再查 `jump-guide.md` 或 `bilibili-guide.md`
  - 通常跳过 `xiaoheihe-guide.md`

- 问基础角色：
  - 先查 `steam-guide.md` + `jump-guide.md`
  - 不够再补 `bilibili-guide.md` / `xiaoheihe-guide.md`
