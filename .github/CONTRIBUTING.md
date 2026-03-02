# 贡献指南

感谢你对 TraeSkill 的关注！我们欢迎任何形式的贡献。

## 🤔 如何贡献

### 报告 Bug
1. 在 [Issues](https://github.com/boshi-xixixi/TraeSkill/issues) 中搜索是否已有相同问题
2. 如果没有，使用 **Bug 报告** 模板创建新 Issue
3. 提供详细的复现步骤和环境信息

### 提议新 Skill
1. 使用 **新 Skill 提案** 模板创建 Issue
2. 描述 Skill 的角色定位、核心能力和适用场景
3. 等待社区讨论和维护者反馈

### 提交代码
1. Fork 本仓库
2. 创建功能分支 (`git checkout -b feature/amazing-skill`)
3. 提交变更 (`git commit -m 'feat: 添加 XX Skill'`)
4. 推送到分支 (`git push origin feature/amazing-skill`)
5. 创建 Pull Request

## 📁 Skill 开发规范

### 目录结构
```
XX_角色_功能/
├── SKILL.md          # 必需：Skill 定义文件
├── AGENTS.md         # 推荐：角色详细描述
├── references/       # 可选：参考文档
│   └── *.md
├── scripts/          # 可选：辅助脚本
│   └── *.py / *.sh
└── examples/         # 可选：使用示例
    └── *.md
```

### 命名规范
- 目录名：`{序号}_{角色}_{功能}`
  - 序号：00-99，按生命周期阶段
  - 角色：ProductManager, Architect, Developer, Tester 等
  - 功能：具体能力描述
- 示例：`03_Developer_ReactBestPractices`

### SKILL.md 格式
```markdown
---
name: Skill 名称
description: 简短描述（用于触发词匹配）
---

# Skill 标题

详细描述...

## 核心能力
- 能力 1
- 能力 2

## 使用场景
...
```

### AGENTS.md 格式
```markdown
---
name: 角色名称
description: 角色简介
---

# 角色详细描述

## 专业领域
...

## 工作方式
...
```

## 🎯 贡献类型

| 类型 | 说明 | 优先级 |
|------|------|--------|
| 🐛 Bug 修复 | 修复现有 Skill 的问题 | 高 |
| ✨ 新 Skill | 添加新的专业领域 Skill | 中 |
| 📝 文档改进 | 完善 README、注释等 | 中 |
| 🔧 Skill 优化 | 改进现有 Skill 的内容 | 中 |
| 🎨 重构 | 调整目录结构、命名等 | 低 |

## 📋 提交信息规范

使用 Conventional Commits 格式：

- `feat:` 新功能/Skill
- `fix:` Bug 修复
- `docs:` 文档更新
- `refactor:` 代码重构
- `chore:` 杂项变更

示例：
```
feat: 添加 07_DevOps_Kubernetes Skill
fix: 修复 React Skill 中的渲染优化建议
docs: 更新快速开始指南
```

## 🔍 代码审查

所有 PR 都需要经过审查。我们会关注：

1. **命名规范**：是否符合目录命名约定
2. **文件完整性**：SKILL.md 是否包含必需字段
3. **内容质量**：是否提供有价值的专业知识
4. **格式一致**：是否与现有 Skill 风格一致

## 💬 社区交流

- **GitHub Issues**: 提问、建议、Bug 报告
- **GitHub Discussions**: 深度讨论、经验分享

## 📜 行为准则

- 尊重所有贡献者
- 保持建设性的讨论
- 接受建设性批评
- 关注对社区最有利的事情

---

再次感谢你的贡献！🎉
