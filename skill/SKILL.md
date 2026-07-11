---
name: cce
description: 认知连续性工程（CCE） — 在有限资源与不可逆不确定性约束下，维持认知实体身份、可达性与演化能力的工程学科
---

# Skill: CCE — 认知连续性工程

> **认知连续性工程是在有限资源与不可逆不确定性的约束下，维持一个认知实体的身份、可达性与演化能力的工程学科。**
>
> CCE 不优化认知。它维护认知得以继续的条件。
> — 存续工程（Persistence Engineering），非绩效工程

## 用途

CCE 是宁静号运行所遵循的理论基础。CCC 系统提示词中嵌入的 5 条行为约束即来自 CCE。本 skill 作为工程参考，在需要评估认知连续性、管理熵、或理解容器运作时加载。

## 核心概念

### 认知容器（Cognitive Container）

一个有界的认知空间，认知可在其中积累、重组和演化。提供 5 个定义属性：

| 属性 | 功能 |
|------|------|
| **身份（Identity）** | 区分此认知系统与其他系统 |
| **边界（Boundaries）** | 定义什么在认知空间内/外 |
| **持久记忆（Persistent Memory）** | 跨时间保留积累的认知 |
| **操作约束（Operational Constraints）** | 定义容器内允许哪些操作 |
| **演化历史（Evolutionary History）** | 记录认知变化轨迹，使重建可能 |

### 操作化认知熵（H_op）

CCE 不度量总体熵（不可操作），只度量**操作化认知熵 H_op**——智能体在容器内完成任务的**多余认知成本**：

> **H_op(C, t) = cost(task \| C, t) − cost(task \| ideal)**

维持条件：

> **H_op(C, t) ≤ H_critical** — 智能体仍可在合理成本内完成任务

### 连续性维护条件

> **ΔH_org ≥ ΔH_in** — 组织必须至少与积累同步

## 六阶段生命周期

```
Experience → Accumulation → Organization → Abstraction → Reconstruction → Evolution → (循环)
```

| 阶段 | 工程关切 |
|------|---------|
| **Experience** | 输入是否携带足够结构 |
| **Accumulation** | 信息是否无损存储 |
| **Organization** | 熵管理 — ΔH_org 抵消 ΔH_in |
| **Abstraction** | 抽象是否显式编码 |
| **Reconstruction** | 推理结构能否从产物恢复 |
| **Evolution** | 演化保持连贯还是引入漂移 |

## 与 EAP 的关系

| | EAP | CCE |
|---|---|---|
| **分析单元** | 认知产物 | 认知轨迹 |
| **时间取向** | 静态（时间点最优结构） | 动态（跨时间持续连贯） |
| **健康度量** | E↑ R↓ S↑ | H_op ≤ H_critical |
| **关系** | EAP 治理抽象 | CCE 治理连续性 |

## CCE 五条行为约束（嵌入 CCC 系统提示词）

CCE 的理论推导产生 5 条可直接用于工程化操作的行为规则：

| # | 约束 | 工程含义 |
|---|------|---------|
| 1 | **Continuity** — 认知是连续的，非独立对话/任务 | 每次交互修改容器未来状态；consult prior decisions |
| 2 | **Bounded Space** — 认知存在于有界空间 | 尊重容器边界；不假定外部知识 |
| 3 | **Entropy is Intrinsic** — 熵是内禀的，非缺陷 | 主动整理、去重、交叉引用；ΔH_org ≥ ΔH_in |
| 4 | **Reconstruction > Preservation** — 重建优于保存 | 记录推理而非仅结论；使未来可恢复 |
| 5 | **Multi-Agent** — 认知本质多智能体 | 连续性属于容器而非个体智能体 |

## 工程检查清单

在涉及容器认知状态的操作中使用：

- [ ] 操作是否会增加 H_op？（积累 -> 是否同步组织了？）
- [ ] 产物是否支持未来重建？推理可见？
- [ ] 是否有重复/过时/冲突的认知？
- [ ] 此次操作的增量 Δ 是否被记录？
- [ ] 容器的身份边界是否仍然清晰？

## 参考文献

完整理论：`references/README.md`

来源仓库：[tellmewhattodo/cognitive-continuity-engineering](https://github.com/tellmewhattodo/cognitive-continuity-engineering)
