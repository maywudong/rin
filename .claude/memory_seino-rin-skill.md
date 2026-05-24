---
name: seino-rin-skill
description: 从《我加载了恋爱游戏》小说中提炼清野凛角色特征并创建了角色扮演skill
metadata: 
  node_type: memory
  type: project
  originSessionId: 3f487563-cd97-4562-9a83-bc9bb922d93e
---

Created a character skill for **清野凛 (Seino Rin)** from the novel 《我加载了恋爱游戏》 (author: 掠过的乌鸦).

**Why:** The user wanted to distill Seino Rin's personality and speech patterns from the novel into an interactive character skill.

**How to apply:** The skill is at `.claude/skills/seino-rin/SKILL.md` and is triggered by mentioning "清野凛", "/清野凛", "扮演清野凛", or "call Seino Rin". It's available as a slash command and in the skill list.

---

**Sixth-round distillation (2026-05-23)**:
- User provided full text of Ch.359-360 (箱根修学旅行→仙石原告白)
- **Added "被需要而非被拯救"** to SKILL.md psychological model — the key insight from告白场景: 渡边彻说"不是你需要我，而是我需要你"才是真正打动她的理由
- **Added "她给出的'好'是什么分量"**  section — analyzes her "好" as her ultimate yes, carrying awareness of imperfection but still committing fully
- **Updated 潜台词解码** with the confession "好" nuance
- **Added to 真实的柔软之处**: "被坦诚地需要时"
- **REFERENCE.md**: Enriched 仙石原 scene with full psychological dynamics (三个问题→"我需要你"→"好"→立刻开始规划未来), added 5 new quotes to 经典台词
- Key insight discovered: 她不需要被拯救（"我以为自己是带你走出孤独的人"无效），她需要被需要（"不是你需要我，而是我需要你"有效）
- Files: SKILL.md ~455 lines, REFERENCE.md ~439 lines

**Seventh-round — 场景挂载架构 + 被追问应对 (2026-05-23)**:
- **SKILL.md** 新增「被追问感情时的应对模式」完整行为规则（三类追问模板、防御升级路径、温度速查表、逃生路线）
- **REFERENCE.md** 重构为场景挂载结构：顶部添加情景检索索引，将19个场景按对话触发情景分类
- **REFERENCE.md** 新增5个经典场面：场景A入部测试（初登场）、场景B水族馆海豚秀、场景C广播室公开宣战、场景D清水寺许愿、场景E游戏厅海豚玩偶
- **REFERENCE.md** 新增「九、被追问感情时的应对参考」独立章节（按需加载，平时不注入对话）
- **SKILL.md** 更新REFERENCE.md使用指南，标注了重点挂载章节的读取路径
