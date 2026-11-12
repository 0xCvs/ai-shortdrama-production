---
name: ai-shortdrama-production
description: |
  用吴明的实战方法做 AI 短剧：当提示词失效、角色串脸、多人堆不下、两卡接不上、只能抽卡时，按症状选对应的补救路径。适用于已有剧本与资产、正在生成或剪辑阶段卡住的情况。不适用于从零写剧本、也不适用于纯文本创作。
metadata:
  cangjie.generated-by: cangjie-tools v2.5.0
  cangjie.variant: single
  cangjie.bundle-id: ai-video-wuming-method
  cangjie.capability-count: 13
  cangjie.entrypoint-count: 1
---
# AI 短剧制作实战课（吴明直播） — 全书能力入口

## 触发与不触发

**适用**：与本书能力域相关的咨询与任务（见下方路由表的意图列）。
**不适用**：
- 从零写剧本、改编小说（属编剧范畴）
- 白膜的制作用什么工具、四锁的具体参数（原文未给）
- 纯文本或非视觉内容创作

## 核心原则（常驻速览，概览类问题读到这里即可回答）

1. 图像管外观与姿态，文字管动作与声音：可见信息用参考图，不可见信息才写文字
2. 提示词越复杂模型越跑偏，只写这次要发生的变化
3. 同一份提示词反复不对，说明通道选错了，不是措辞问题
4. 一次只解决一个问题：先静态定构图，再动态定运动
5. 不整段重跑，从已有结果里挑可用部分继续推进

## 能力路由（先读本表，按意图加载 1 张能力卡）

| 用户意图 | 先读 | 补读/备注 |
|---|---|---|
| 提示词写对了但画面不对；模型不听话；该填的没填；方向跑偏；表情不对 | references/capabilities/resolve-by-reference.md | references/capabilities/prompt-minimalism.md、references/capabilities/pose-first.md |
| 提示词越写越长；效果反而变差；不知道怎么控制细节；该写多细 | references/capabilities/prompt-minimalism.md | references/capabilities/resolve-by-reference.md |
| 反复抽卡；姿势出不来；手部关系不对；变形 | references/capabilities/pose-first.md | references/capabilities/complex-setup-base-image.md、references/capabilities/resolve-by-reference.md |
| 视频参考串脸；角色尺寸变了；脸不一样了；参考后变假 | references/capabilities/video-ref-guard.md | references/capabilities/multi-person-layout.md、references/capabilities/tail-frame-handoff.md |
| 多人场景堆不下；人物穿模；站位穿帮；六人怎么做 | references/capabilities/multi-person-layout.md | references/capabilities/group-shot-background.md、references/capabilities/video-ref-guard.md |
| 两卡接不上；衔接不连续；下一卡人物变了；动作断了 | references/capabilities/tail-frame-handoff.md | references/capabilities/salvage-frame.md |
| 整段有穿帮；不想重跑；抽卡成本高；只有几秒能用 | references/capabilities/salvage-frame.md | references/capabilities/tail-frame-handoff.md |
| 约束太多生不出来；复杂剧本；捆绑口塞；多部位 | references/capabilities/complex-setup-base-image.md | references/capabilities/pose-first.md |
| 群像场面；运动会；群架；九宫格 | references/capabilities/group-shot-background.md | references/capabilities/multi-person-layout.md |
| 插入画面假；特写没感觉；单独抽卡 | references/capabilities/insert-shot-separate.md | references/capabilities/salvage-frame.md |
| 参考视频是外语；声音不对；叫声不会写；叠音 | references/capabilities/audio-replace.md | references/capabilities/prompt-minimalism.md |
| 模型变慢；漏信息；不思考；上下文太长 | references/capabilities/window-reset.md | — |
| 做封面；封面人物错乱；版式难看 | references/capabilities/cover-reference.md | references/capabilities/resolve-by-reference.md |

**非能力类查询**：
- 书名/作者/章节/整书概览 → references/overview.md
- 术语解释 → references/glossary.md
- 决策规则速查（不需要原文依据时） → references/cheatsheet.md
- 完整意图与关键词索引（本表未覆盖的意图先查这里） → references/capability-index.md

## 加载规则

- 每次任务先读本文件，再按路由表加载 **1** 张能力卡；任务明确跨域时最多加载 2 张。
- 概览/书名类问题不加载能力卡，用「核心原则」与 overview.md 回答。
- 路由表与 capability-index.md 都无法命中的意图，明确告知超出本书范围，不要硬套。

## 边界与判停

- 症状不属于视觉生成类（如纯文字问题）时停止，不套用本方法
- 需要具体工具参数或量化阈值时停止，原文只有定性描述
