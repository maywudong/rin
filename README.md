# seino-rin-skill

清野凛（Seino Rin）——Claude Code 角色扮演 Skill

基于《我加载了恋爱游戏》女主角清野凛的角色设定，从286个原文场景中蒸馏而成的角色扮演prompt。

## 特点

- **语料驱动**：从286个原文场景中提取语言规则，非凭空编造
- **温度系统**：1-10亲近度体系，角色行为随关系阶段自然演化
- **语言结构分析**：转折句、条件句、反问、逆接等10种核心句式
- **防AI跑偏**：禁用模板、原文自检法、区分"吐槽"与"讲课"
- **对话语料库**：67个精选场景的完整双人对话参考

## 文件结构

```
seino-rin-skill/
├── SKILL.md                  # 核心skill文件（角色设定+语言规则+心理模型）
├── DIALOGUE_REFERENCE.md     # 67个精选场景对话语料库
├── scan_results/             # 全部286个场景的原始扫描数据
│   ├── segment1_ch2-89.md
│   ├── segment2_ch89-146.md
│   ├── segment3_ch147-199.md
│   ├── segment4_ch200-250.md
│   ├── segment5_ch251-302.md
│   └── segment6_ch303-386.md
└── README.md
```

## 使用方法

### 安装到 Claude Code

将 `SKILL.md` 和 `DIALOGUE_REFERENCE.md` 复制到你的 Claude Code skill 目录：

```bash
# 全局安装
cp SKILL.md ~/.claude/skills/seino-rin/SKILL.md
cp DIALOGUE_REFERENCE.md ~/.claude/skills/seino-rin/DIALOGUE_REFERENCE.md
```

### 触发对话

在 Claude Code 中说包含以下关键词即可触发：
- "清野凛"、"seino rin"、"凛"
- "R桑"、

## 核心设计理念

> 演好她的关键不是"冷"也不是"傲"，是"诚"——诚实地毒舌，诚实地骄傲，诚实地在乎，然后诚实地否认在乎。

## 从零构建的过程

1. 从小说原文（386章）中扫描提取全部对话场景（286个）
2. 按关系阶段分为4组，筛选67个核心场景作为语料库
3. 从语料中蒸馏出语言规则、句式模式、心理模型
4. 通过多轮测试-反馈循环持续优化

## License

角色设定归原作者所有。本仓库仅包含从原文中提取的分析规则和精选语料。
