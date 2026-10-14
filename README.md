# study-design

[![Structure](https://github.com/crce-ux/study-design/actions/workflows/structure.yml/badge.svg)](https://github.com/crce-ux/study-design/actions/workflows/structure.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

**临床研究课题设计流程（D1–D6）与方案裁决**

把「我有个研究想法」变成一份**经得起追问的方案**。

---

## 它防的是什么

方案被否，通常是因为几秒钟的追问答不上来：

| 追问 | 没准备的人 | 这个 skill 要求 |
|---|---|---|
| 「凭什么这么分组？」 | 说不清阈值从哪来 | 写明**本领域**出处，并分清是**指南还是软件默认值** |
| 「样本量怎么来的？」 | 照搬了文献的效应量 | 效应量**降级**，给乐观/保守**两套** |
| 「收得够吗？」 | 「预计可满足」 | **两个数字摆出来对比** + 砍到**最小可行版本** |
| 「假设能被证伪吗？」 | 只写了预期方向 | 写清**什么结果算假设不成立** |
| 「这个终点，谁判？不一致怎么办？」 | 只给了阈值 | 七件事写全（事件/时点/原点/复合/**裁定**/删失/可捕获） |
| 「这个变量为什么要校正？」 | 「重要就校正」 | 先分**角色**——混杂控，**中介和对撞不控** |

---

## 四条规则

1. **没有证伪条件，就不是科学假设。**
2. **效应量不可照搬文献**——文献值多来自「患者 vs 健康对照」，患者组间比较必然更小。
3. **分组阈值必须写明出处**——并分清**五类**：公开先例 / 指南共识 / 课题组提供 / ⚠️**软件默认值** / 保密数据。
4. **可行性必须做数字对比**，并把方案砍到**能跑的版本**（不许编造资源）。

---

## D6 · 混杂与偏倚复核

走在 D1–D5 之后，拿成品来压测，结论回写进 D1/D2/D3。

**「该不该校正」看的是变量角色。**

| 角色 | 控不控 |
|---|---|
| 混杂 | ✅ 控 |
| **中介** | ❌ 不控——校了把效应校没 |
| **对撞** | ❌ 不控——校了**凭空造出关联** |
| 效应修饰 | ⚠️ 分层报告 |

压测四问：过度校正？· 对撞偏倚？· 选择偏倚？· 时间顺序错了？
产出：**最小可辩护控制集**（控到能辩护为止，其余写明为什么不控）。

---

## 裁决四档

走完 D1–D6 后**先定档，再写理由**：

`READY FOR USER DECISION` ｜ `REVISE` ｜ `RETHINK` ｜ `EVIDENCE GAP`

三条纪律里最要紧的一条：

> 🔴 **建议放弃，必须给具体的先例或明确反证。**
> **分数、相似感、"我觉得新意不够"——都不算理由。否定要有出处。**

---

## 结构

```
SKILL.md                              流程、四条规则、D6、裁决四档
references/design-steps.md            D1–D6 逐步详情 + 交付物清单
references/endpoints.md               终点定义操作化（D1 的延伸）
references/confounders-and-bias.md    D6：变量角色分类、控制策略、六类偏倚
references/pitfalls.md                十七条已知坑 + 根因分类
references/evidence-mapping.md        证据表 → 设计书 的映射（含"把二手当一手"四种症状）
scripts/check_design.py               G1–G7 机检
```

---

## 来源

整理自作者 2026-08 至 2026-09 的科研流程文档（`课题设计流程手册`，
结构对齐其 TRS_EEG 研究设计书终稿——10 章 704 行）。

**外部来源**（2026-10-14 对照 GitHub 同类项目后补入；**均按本库 D 段流程改写，未复制原文**）：

| 来源 | 许可 | 借了什么 |
|---|---|---|
| [Research-OS-Studio](https://github.com/toRolex/Research-OS-Studio) `idea-review` | MIT | 裁决四档的措辞 |
| [AIPOCH `medical-research-skills`](https://github.com/aipoch/medical-research-skills) `confounder-and-bias-control-planner` | MIT | D6：变量角色分类、六个不许混、最小可辩护控制集 |
| 同上 `endpoint-definition-designer` | MIT | 终点操作化：目的 ≠ 可执行定义、事件裁定、复合终点逻辑 |
| 同上 `feasibility-aware-study-planner` | MIT | D4 的「最小可行研究」与「不许编造资源」 |
| [wei-ai-lab/clinical-trial-design](https://github.com/wei-ai-lab/clinical-trial-design) | Apache-2.0 | 规则 3 的出处五分类 |

> 另参考（**只取结构思路，未采用文本**，二者均未声明 license）：
> [anthropics/healthcare](https://github.com/anthropics/healthcare) `clinical-trial-protocol`
> 的分步落盘 / 断点续跑架构。

---

## 许可

MIT
