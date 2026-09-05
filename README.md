# 产品经理思维工坊（PM Thinking Workshop）

> 用「女娲」蒸馏顶级产品大脑，把每次产品决策变成一场**多视角思维圆桌**。
> 项目名：super PM —— 你不是一个人在做产品决策。
>
> 📌 **引用说明**：本仓库引用了开源项目 **[女娲 · Skill造人术（nuwa-skill）](https://github.com/alchaincyf/nuwa-skill)**
> （MIT © 花叔，https://github.com/alchaincyf ）——本仓库的产品大师人物思维技能由**女娲蒸馏引擎**生成，
> 女娲本体以 **git submodule** 方式引入（`skills/nuwa-skill/`）。第三方引用与许可详情见
> [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)。

---

## 这是什么

本仓库把两样东西组合在一起：

1. **[女娲 · Skill造人术](https://github.com/alchaincyf/nuwa-skill)**（已下载至 `skills/nuwa-skill/`）
   一个开源的认知蒸馏引擎：深度调研任何人的思维方式（心智模型、决策启发式、表达 DNA），
   蒸馏成「可运行的人物 Skill」——相当于给 AI 装上一个真实人物的思维操作系统。

2. **思维工坊（workshop/）**
   一条完整的**产品工作流**（见 `workshop/工作流程.md`）：
   **输入需求 → 需求分析 → AI 产品规划 → 专家团独立评审 → 交锋讨论 → 最终决策**。
   专家团 = 产品大师（乔布斯/张小龙/雷军的人物思维）+ 职能专家（商业/技术/体验/增长）
   + 用户代表（挑刺者）+ 成本中心（投入产出把关），各自用**自己的镜片**评审方案，
   最后由你拍板，AI 整理成决策与行动项。

> 一句话：**女娲负责「造大脑」，工坊负责「开会」。**

---

## 目录结构

```
super PM/
├── README.md                        # 本文件
├── skills/
│   ├── nuwa-skill/                  # 女娲造人术（git submodule → 原仓库，需 update --init 获取内容）
│   │   ├── SKILL.md                 # 女娲本体的运行指令
│   │   ├── references/              # 蒸馏方法论（模板/框架/保真度记分卡）
│   │   ├── scripts/                 # 调研工具脚本
│   │   └── examples/                # 已蒸馏人物样例（乔布斯/张一鸣/芒格/费曼…）
│   └── personas/                    # ★ 思维委员人物库（蒸馏成品存放区）
│       ├── steve-jobs-perspective/  # ✅ 现成可用：乔布斯（复制自女娲 examples）
│       └── …                        # 未来：zhang-xiaolong-perspective/ lei-jun-perspective/
├── workshop/                        # ★ 工坊运行区（产品工作流）
│   ├── 工作流程.md                  # ★ 主流程 SOP：六阶段 + 资料缺口协议
│   ├── README.md                    # 工坊入口与快速开始
│   ├── committee/                   # 专家名册
│   │   ├── README.md                #   名册总览
│   │   ├── personas/                #   产品大师（乔布斯✅/张小龙✅/雷军✅）
│   │   └── roles/                   #   职能专家 + 用户代表 + 成本中心
│   ├── templates/                   # 00-需求输入 … 06-复盘记录 阶段模板
│   └── sessions/                    # 每场工坊产出归档（本地维护；案例默认不入库，见 .gitignore）
└── docs/
    └── 蒸馏手册.md                  # 用女娲给新人物「造大脑」的作战指南
```

---

## 快速开始

把这条指令发给任意 AI（DeepSeek/Claude/Cursor 等），替换需求即可：

```
进入产品思维工坊，执行标准工作流程：
1. 读取 workshop/工作流程.md，按六阶段执行；
2. 读取 workshop/committee/README.md 点专家团；
3. 每阶段产物写入 workshop/sessions/<今天日期>-<主题>/ 对应文件；
4. 需要资料时按「资料缺口协议」处理（问用户 → 搜电脑文档 → 联网检索）；
5. 我的需求是：<粘贴原始需求>
```

流程一览：**需求输入(00) → 需求分析(01) → 产品规划(02) → 专家独立评审(03)
→ 交锋讨论(04) → 最终决策(05)**，落地后可选复盘(06)。

专家团当前阵容：

| 类别 | 成员 | 状态 |
|------|------|------|
| 产品大师 | 乔布斯 | ✅ 完整蒸馏可用 |
| 产品大师 | 张小龙 / 雷军 | ✅ 完整蒸馏可用（2026-09-05） |
| 职能专家 | 商业/技术/体验/增长 | 🎭 AI 扮演 |
| 用户与成本 | 用户代表（挑刺者）/ 成本中心 | 🎭 AI 扮演 |

---

## 理念

- **女娲造的不是人，是镜子**：用另一个人的眼睛看自己的问题，不是模仿，是拓展思维边界。
- **好产品是辩论出来的**：克制派（张小龙）与极致派（乔布斯）对同一方案的看法往往相反，
  而真实决策正是在这种张力中收敛出来的。
- **每个视角都有盲区**：委员会里永远要问一句「这位委员在这个问题上帮不了什么」。

---

## 女娲更新

女娲本体以 **git submodule** 引入，指向 [alchaincyf/nuwa-skill](https://github.com/alchaincyf/nuwa-skill)（MIT © 花叔）。

克隆本仓库后，先初始化子模块拿到女娲内容：

```bash
git submodule update --init --recursive
```

将女娲更新到最新版：

```bash
git -C skills/nuwa-skill checkout main
git -C skills/nuwa-skill pull --ff-only
```

> 第三方引用与许可详情见 [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)。

---

## 致谢

- [alchaincyf/nuwa-skill（女娲）](https://github.com/alchaincyf/nuwa-skill) — 认知蒸馏引擎
- 蒸馏方法论详见 `skills/nuwa-skill/references/`
