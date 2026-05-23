# Source Index

## Default query mode

For direct character build questions, default to aggregated lookup:

0. `character-coverage-index.md`
1. `steam-guide.md`
2. `jump-guide.md`
3. `bilibili-guide.md`
4. `xiaoheihe-guide.md`
5. `epic-guide.md`
6. `build-site-guide.md`
7. `term-glossary.md`

Only add `wiki-notes.md` when the user is asking for mechanics, unlocks, or factual clarification.

Use `character-coverage-index.md` first to skip sources that obviously do not cover the requested character.

For broader non-character strategy questions, prefer:

1. `steam-notes.md`
2. `bilibili-general.md`
3. `wiki-notes.md` only when factual clarification is needed

## jump-guide.md

- Source type: your manually curated Chinese notes
- Best for:
  - character-specific build advice
  - early/mid/late game routing
  - stat priority
  - common failure points
- Always include this source for almost all direct "这个角色怎么玩" questions
- But skip it when `character-coverage-index.md` marks the character as not covered here

## wiki-notes.md

- Source type: Wiki / objective reference
- Best for:
  - character mechanics
  - unlock conditions
  - base traits
  - terminology and factual clarification
- Use only when the user asks "这个角色机制是什么" or when you need to verify a fact

## steam-guide.md

- Source type: Steam Community guide organized from the English original
- Best for:
  - role-specific build routes
  - build comparisons
  - route and weapon transition ideas
- Include this source first for character queries whenever it has usable notes
- This is the highest-priority practical source for character打法

## steam-notes.md

- Source type: Steam Community general notes organized from the English original
- Best for:
  - broad D5 strategy
  - general stat heuristics
  - item and economy ideas
  - elite / boss handling
- Use this when the user asks broader strategy questions rather than one specific character
- This is the Steam-side companion file to `steam-guide.md`

## bilibili-guide.md

- Source type: cleaned Bilibili long-form character guide
- Best for:
  - per-character build routes
  - weapon recommendations
  - difficulty / 操作 / 规划 / 运气评分
  - long-form practical notes preserved from the original article
- Include this source for direct character build questions whenever it has the character
- User-facing output should treat this as part of `B站攻略`, not expose the file name

## xiaoheihe-guide.md

- Source type: cleaned Xiaoheihe long-form character guide
- Best for:
  - per-character build routes
  - concise weapon recommendations
  - compact stat priority
  - short practical route summaries
- Include this source for direct character build questions whenever it has the character
- User-facing output should label this source as `小黑盒攻略`

## bilibili-general.md

- Source type: cleaned Bilibili general guide notes
- Best for:
  - mixed-weapon rules
  - stat priority heuristics
  - general item advice
  - elite / boss handling
- Use this as supplementary context when the user asks broader strategy questions rather than one specific character

## epic-guide.md

- Source type: editorial / media guide
- Best for:
  - media-style role recommendations
  - role highlights
  - unlock summaries
- Important:
  - user-facing output must label this source as `Epic攻略`
  - only show `Epic攻略` when the character has a direct Epic entry
  - if there is no direct Epic entry, omit `Epic攻略` instead of guessing

## build-site-guide.md

- Source type: build site / editorial summary
- Best for:
  - tier / ranking information
  - structured build fields like strengths, weaknesses, stat priority, and stage-by-stage plans
- Include this source when available for character queries
- This is a supplementary source that often fills gaps left by `jump-guide.md` and `steam-guide.md`
- Important:
  - user-facing output must label this source as `Brotato Builds攻略`

## character-coverage-index.md

- Source type: local source-coverage map
- Best for:
  - skipping irrelevant files before reading them
  - quickly deciding whether `jump-guide.md` / `xiaoheihe-guide.md` / `epic-guide.md` can be ignored
  - speeding up normal character lookups
- Read this before expanding to secondary sources

## term-glossary.md

- Source type: local Chinese/English terminology map
- Best for:
  - normalizing role names
  - normalizing weapon and item names
  - normalizing stat names
  - avoiding mixed Chinese/English output
- Use this before finalizing the answer text
- Default output should prefer Chinese names

## source-links.md

- Source type: original source URL list
- Best for:
  - users asking where the guides came from
  - users asking for original article or video addresses
  - tracing a visible source label like `Steam攻略` or `Epic攻略` back to its origin
- Do not include these links in normal character build answers

## Conflict rules

- Do not hide source differences. Show them.
- Prefer the newest source when version changes are likely.
- Prefer objective references for facts and community references for playstyle suggestions.
- If two build suggestions conflict, present them as alternatives instead of forcing one answer.
- If a source looks old or clearly version-sensitive, say so.
