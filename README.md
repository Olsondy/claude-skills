# My Skills - Claude 插件集

这是一个自定义的 Claude Skill 插件集合，用于扩展 Claude 的能力。

## 📁 目录结构

```
my-skills/
├── .claude-plugin/
│   └── marketplace.json      # 核心：插件市场清单
├── plugins/
│   └── linear-design/        # Linear Design 插件
│       ├── .claude-plugin/
│       │   └── plugin.json   # 插件描述
│       └── skills/
│           └── linear-design/
│               └── SKILL.md  # Skill Prompt 内容
└── README.md                 # 本文件
```

## 🚀 已安装插件

### 1. Linear Design

**版本**: 1.0.0
**作者**: Your Name
**描述**: 帮助设计符合 Linear 风格的用户界面和组件

**功能**:
- UI 设计指导
- 组件设计规范
- 设计系统咨询
- Linear 风格实现

**使用方法**:
1. 在 Claude 中调用 `/linear-design` skill
2. 描述你的设计需求
3. 获取符合 Linear 风格的设计建议和代码示例

## 📦 添加新插件

1. 在 `plugins/` 目录下创建新的插件文件夹
2. 创建 `.claude-plugin/plugin.json` 配置文件
3. 在 `skills/` 目录下添加你的 SKILL.md 文件
4. 在 `.claude-plugin/marketplace.json` 中注册插件

### 插件配置模板

```json
{
  "id": "your-plugin-id",
  "name": "Your Plugin Name",
  "description": "Plugin description",
  "version": "1.0.0",
  "author": "Your Name",
  "skills": [
    {
      "name": "skill-name",
      "description": "Skill description"
    }
  ],
  "capabilities": ["capability1", "capability2"],
  "tags": ["tag1", "tag2"]
}
```

## 🔧 配置说明

### marketplace.json
这是插件市场的核心配置文件，列出了所有可用的插件。

### plugin.json
每个插件的描述文件，定义了插件的能力、技能和元数据。

### SKILL.md
实际的技能 Prompt 内容，定义了技能的行为和知识。

## 📝 开发指南

### 创建 Skill 的最佳实践

1. **清晰的目标**: 每个 Skill 应该有明确的用途
2. **详细的指导**: 在 SKILL.md 中提供清晰的使用说明
3. **示例**: 包含实际的使用示例
4. **版本控制**: 使用语义化版本号

### SKILL.md 结构建议

```markdown
# Skill Name

简短描述

## 核心功能
- 功能 1
- 功能 2

## 使用指南
详细的使用说明

## 示例
实际使用示例

## 注意事项
重要的使用注意事项
```

## 📄 许可证

MIT License

## 🤝 贡献

欢迎提交新的插件和改进建议！

---

**创建时间**: 2026-01-26
**维护者**: Olsond
