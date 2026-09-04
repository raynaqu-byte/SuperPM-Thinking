# 第三方引用说明（Third-Party Notices）

> 本仓库引用、内嵌或改写了以下第三方开源成果。遵守各上游许可并在此明确声明，
> 是本仓库公开分发的前提。如有遗漏或疑问，欢迎提 issue 指正。

---

## 1. 女娲 · Skill造人术（nuwa-skill）

- **项目**：女娲 · Skill造人术 —— 认知蒸馏引擎（把真实人物的思维方式蒸馏成可运行的人物 Skill）
- **上游仓库**：<https://github.com/alchaincyf/nuwa-skill>
- **作者**：花叔（Huashu，GitHub: alchaincyf）
- **许可**：MIT License，Copyright (c) 2026 Huashu（完整许可文本见上游 `skills/nuwa-skill/LICENSE`）
- **引入方式**：**git submodule**，挂载于本仓库 `skills/nuwa-skill/`，内容不随本仓库复制分发，
  克隆后需执行 `git submodule update --init --recursive` 获取。

### 本仓库对女娲的引用与使用

- `docs/蒸馏手册.md`：女娲的本地化操作指引（造脑指南）。
- 本仓库的**产品大师人物思维技能**（乔布斯 / 张小龙 / 雷军，位于 `skills/personas/`
  与 `workshop/committee/personas/`）是**使用女娲蒸馏引擎产出 / 按女娲方法整理**的成果，
  其中乔布斯素材整理自女娲公开 examples；各技能的原始研究素材（公开采访、文章、发言等）
  版权归原作者或发布者所有，出处均标注在各技能内 `references/` 文件中，仅用于研究性思维蒸馏。
- 女娲本体及其完整 examples（张一鸣、Karpathy、Trump、MrBeast、张雪峰 等）不在本仓库内，
  以 submodule 指向 [alchaincyf/nuwa-skill](https://github.com/alchaincyf/nuwa-skill) 获取。

### 合规要点

对女娲及其衍生素材的任何使用与再分发，均须保留上游 MIT LICENSE 与版权声明，
并注明出处为女娲（nuwa-skill, © 花叔）。

---

## 2. 人物公开素材（研究引用）

各人物技能内的调研素材均来自公开渠道（发布会、访谈、书籍、文章、推文等），
版权归原作者 / 发布者所有，出处已在各技能 `references/` 内标注；
本仓库不主张对上述公开素材的任何权利，仅将其用于思维蒸馏与教育演示目的。

---

*本说明随仓库内容同步维护。*
