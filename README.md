# kb-template

一套面向人与 AI Agent 协作的通用知识库模板，包含完整的维护规则（`AGENTS.md`）与最小目录骨架，拉取后即可投入使用。

## 快速开始

1. 点击本仓库右上角 **Use this template** 创建你自己的私有仓库（或 `git clone` 后重新初始化 `git init`）。
2. 用你常用的 AI Coding Agent（OpenCode、Codex、Claude Code、Cursor 等）打开本地仓库目录。
   - Agent 会自动读取根目录下的 `AGENTS.md` 作为维护规则；若使用的工具默认读取 `CLAUDE.md`，可在根目录建立软链 `ln -s AGENTS.md CLAUDE.md`。
3. 先把你的公司、团队或个人基本情况发给 Agent，让它按规则初始化 `company/` 下的基础页面。
4. 日常使用时，直接把会议纪要、录音转写、文档、调研或想法发给 Agent，由它按 `AGENTS.md` 归位、提炼并同步更新状态与决策。

## 目录结构

```text
.
├── AGENTS.md           # 知识库维护规则（唯一规则文件）
├── company/            # 自身与组织信息（概况、战略、人员、运营）
├── clients/            # 具体客户的沟通、需求、合同与交付材料
└── projects/           # 方向探索、通用产品、跨客户研究与内部专项
    ├── active/
    ├── paused/
    └── completed/
```

## 自定义

规则全部集中在 [`AGENTS.md`](AGENTS.md) 一份文件中，可按实际使用场景直接调整：

- **个人知识库**：可将 `company/` 改为 `self/`，按需保留或移除 `clients/`。
- **团队与业务协作**：直接沿用默认的 `company / clients / projects` 三分结构。
