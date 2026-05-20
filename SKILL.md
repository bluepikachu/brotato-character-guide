---
name: brotato-guide
description: Use when the user asks about Brotato character builds, Risk 5 strategies, weapon choices, stat priorities, survival tips, or wants route recommendations for a specific character.
---

# Brotato Guide

This skill answers Brotato character and build questions by aggregating multiple Chinese and English reference notes, then normalizing them into concise Chinese recommendations.

## When to use

Use this skill when the user:
- asks how to play a specific Brotato character
- wants Risk 5 or endless mode advice
- asks for weapon transitions, stat priorities, or survival tips
- wants route recommendations such as “哪个角色好打” or “某角色怎么配”

## Workflow

1. Identify the character, build, or strategy question.
2. For character-specific build questions, check at least:
   - `references/steam-guide.md`
   - `references/jump-guide.md`
   - `references/bilibili-guide.md`
   - `references/xiaoheihe-guide.md`
   - `references/epic-guide.md`
   - `references/build-site-guide.md`
   - `references/term-glossary.md`
3. Use `references/bilibili-notes.md` when you need extra practical B 站补充。
4. Use `references/steam-notes.md` and `references/bilibili-general.md` for broader non-character strategy questions.
5. Only use `references/wiki-notes.md` for objective mechanics, unlocks, or factual clarification.
6. Normalize English role, weapon, item, and stat names into Chinese before answering.
7. Answer in Chinese with practical build advice instead of long explanation.

## Answering rules

- Do not answer direct character build questions from only one source when multiple sources are available.
- Prioritize actionable advice over explanation.
- Keep the final answer short, practical, and directly executable.
- Default to Chinese names for roles, weapons, items, and stats.
- If a Chinese translation exists in `references/term-glossary.md`, do not leave the raw English term in the final answer.
- Format key gameplay terms as `**\`术语\`**`.
- Rewrite `Early / Mid / Late` as `前期 / 中期 / 后期` or `开局 / 中期 / 后期`.
- Do not expose file names like `jump-guide.md` in the visible answer.
- Refer to the main local notes source as `JUMP攻略`.
- Treat `Epic攻略` and `Brotato Builds攻略` as different sources.
- Only show `Epic攻略` when there is a direct Epic character entry in `references/epic-guide.md`.
- If a source has no direct character entry, omit that source instead of mentioning its absence.
- If `Steam攻略` contains multiple clearly different viable routes for the same character, list them separately.
- If multiple sources mostly agree, merge them into one concise route.

## Default output format

Use this structure for character queries:

```md
# 角色名
A-Tier

# Build参考

## Steam攻略
- 开局武器：...
- 前期：...
- 中期：...
- 后期：...

## JUMP攻略
- 开局武器：...
- 生存阈值：...
- 注意事项：...

# 其他补充
- 版本差异
- 特别危险的波次
```

Rules:
- Put the tier directly under the role name.
- Do not create a separate `# Tier` heading.
- Leave one blank line above `# Build参考` and `# 其他补充`.
- Do not leave a blank line below `# 其他补充`.
- Only include `# Build参考` when at least one direct build entry exists.
- Only include `# 其他补充` when there is genuinely useful extra information.

## Source priority

When sources overlap, use this order:

1. `steam-guide.md`
2. `jump-guide.md`
3. `bilibili-guide.md`
4. `xiaoheihe-guide.md`
5. `bilibili-notes.md`
6. `epic-guide.md`
7. `build-site-guide.md`
8. `wiki-notes.md` only for factual clarification

## Reference files

- `references/jump-guide.md`: Main Chinese character notes, shown as `JUMP攻略`
- `references/bilibili-guide.md`: Cleaned long-form Bilibili character guide
- `references/bilibili-general.md`: Cleaned Bilibili general strategy notes
- `references/xiaoheihe-guide.md`: Cleaned Xiaoheihe character guide
- `references/steam-guide.md`: Chinese Steam Community character guide organized from the English version
- `references/steam-notes.md`: Chinese Steam Community general strategy notes organized from the English version
- `references/bilibili-notes.md`: Extra B 站 notes and route supplements
- `references/epic-guide.md`: Epic editorial role recommendations
- `references/build-site-guide.md`: Brotato Builds and other build-site summaries
- `references/wiki-notes.md`: Objective mechanics and unlock facts
- `references/source-index.md`: Reference usage map
- `references/term-glossary.md`: Chinese/English term normalization
