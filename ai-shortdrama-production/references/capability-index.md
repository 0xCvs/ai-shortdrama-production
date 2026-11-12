# 能力索引（完整版）

| capability_id | 标题 | 重要度 | 意图 | 关键词 | 能力卡 |
|---|---|---|---|---|---|
| CAP-001 | 提示词失效时转用图像参考 | critical | 提示词写对了但画面不对；模型不听话；该填的没填；方向跑偏；表情不对 | 丢参考图、垫图、模型不听话、参考图、跑偏 | capabilities/resolve-by-reference.md |
| CAP-002 | 提示词精简原则 | high | 提示词越写越长；效果反而变差；不知道怎么控制细节；该写多细 | 提示词太长、精简、复杂、吃一半、跑乱 | capabilities/prompt-minimalism.md |
| CAP-003 | 静态姿势图前置 | high | 反复抽卡；姿势出不来；手部关系不对；变形 | 姿势图、抽卡、静态、一卡、构图 | capabilities/pose-first.md |
| CAP-004 | 视频参考防串脸 | critical | 视频参考串脸；角色尺寸变了；脸不一样了；参考后变假 | 视频参考、串脸、白膜、深度图、四锁、锁脸 | capabilities/video-ref-guard.md |
| CAP-005 | 多人场景重构 | high | 多人场景堆不下；人物穿模；站位穿帮；六人怎么做 | 6P、多人、16比9、画幅、写死、站位、穿模 | capabilities/multi-person-layout.md |
| CAP-006 | 尾帧衔接 | high | 两卡接不上；衔接不连续；下一卡人物变了；动作断了 | 尾帧、首帧、衔接、接缝、人物资产 | capabilities/tail-frame-handoff.md |
| CAP-007 | 抽卡补救：截可用帧 | high | 整段有穿帮；不想重跑；抽卡成本高；只有几秒能用 | 抽卡、截图、可用帧、重跑、浪费积分 | capabilities/salvage-frame.md |
| CAP-008 | 复杂设定先做主体图 | medium | 约束太多生不出来；复杂剧本；捆绑口塞；多部位 | 主体图、复杂、约束、遮眼睛 | capabilities/complex-setup-base-image.md |
| CAP-009 | 九宫格背景 + 单独主角 | medium | 群像场面；运动会；群架；九宫格 | 九宫格、群像、背景、主角 | capabilities/group-shot-background.md |
| CAP-010 | 插入画面单独生成再拼 | medium | 插入画面假；特写没感觉；单独抽卡 | 插入、7秒、单独、拼接 | capabilities/insert-shot-separate.md |
| CAP-011 | 音效替代：去掉参考音频自己写 | medium | 参考视频是外语；声音不对；叫声不会写；叠音 | 音频、音效、叫声、呼吸声、叠音 | capabilities/audio-replace.md |
| CAP-012 | 上下文窗口重置 | medium | 模型变慢；漏信息；不思考；上下文太长 | 窗口、上下文、记忆、变慢、新开 | capabilities/window-reset.md |
| CAP-013 | 封面参考法 | low | 做封面；封面人物错乱；版式难看 | 封面、参考、草图、版式 | capabilities/cover-reference.md |
