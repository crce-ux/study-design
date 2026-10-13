# study-design

[![Structure](https://github.com/crce-ux/study-design/actions/workflows/structure.yml/badge.svg)](https://github.com/crce-ux/study-design/actions/workflows/structure.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

**临床研究课题设计流程（D1–D5）与方案裁决**

把「我有个研究想法」变成一份**经得起追问的方案**。

---

## 它防的是什么

方案被否，通常不是因为想法不好，而是因为几秒钟的追问答不上来：

| 追问 | 没准备的人 | 这个 skill 要求 |
|---|---|---|
| 「凭什么这么分组？」 | 说不清阈值从哪来 | 写明出处（Kane / TRRIP / 中国专家共识） |
| 「样本量怎么来的？」 | 照搬了文献的效应量 | 效应量**降级**，给乐观/保守**两套** |
| 「收得够吗？」 | 「预计可满足」 | **两个数字摆出来对比** |
| 「假设能被证伪吗？」 | 只写了预期方向 | 写清**什么结果算假设不成立** |

---

## 四条铁律

1. **没有证伪条件，就不是科学假设。**
2. **效应量不可照搬文献**——文献值多来自「患者 vs 健康对照」，患者组间比较必然更小。
3. **分组阈值必须写明出处。**
4. **可行性必须做数字对比。**

---

## 裁决四档

走完 D1–D5 后**先定档，再写理由**：

`READY FOR USER DECISION` ｜ `REVISE` ｜ `RETHINK` ｜ `EVIDENCE GAP`

三条纪律里最要紧的一条：

> 🔴 **建议放弃，必须给具体的先例或明确反证。**
> **分数、相似感、"我觉得新意不够"——都不算理由。说"不行"要有出处，感觉不算。**

---

## 结构

```
SKILL.md                            流程、四条铁律、裁决四档
references/design-steps.md          D1–D5 逐步详情 + 交付物清单
references/pitfalls.md              十一条已知坑 + 根因分类
references/evidence-mapping.md      证据表 → 设计书 的映射（含"把二手当一手"四种症状）
```

---

## 来源

整理自作者 2026-08 至 2026-09 的科研流程文档（`课题设计流程手册`，
结构对齐其 TRS_EEG 研究设计书终稿——10 章 704 行）。

裁决四档的措辞借鉴 [Research-OS-Studio](https://github.com/toRolex/Research-OS-Studio)
的 `idea-review`（MIT）。

---

## 许可

MIT
