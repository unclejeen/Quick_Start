---
_id: 3759126427590394
status: Active
author: jee
tags: ["欢迎", "knloop"]
belongs_to: ["[[AGENTS]]", "[[welcome_to_knloop]]"]
_icon: 👋
---
# 欢迎使用 knloop

knloop 是一个本地优先的 Markdown 知识库。你所写的所有内容都以纯 `.md` 文件的形式保存在你自己的 vault 文件夹中——没有平台锁定，没有私有数据库，你的文件在任何编辑器中都可以直接打开阅读。

在这里开始记录你的想法吧……

试试一些 **Markdown 语法：**

```
# 标题
- 列表
> 引用
`行内代码`
```

## 笔记只是文件

每篇笔记都是一个带有 YAML frontmatter 的 Markdown 文件：

```markdown
---
tags: ["note", "Topic"]
author: jee
status: Active
related_to: "[[knloop]]"
---

# 示例文档
```

- **第一个 H1 标题**即为笔记标题。knloop 会在笔记列表、搜索和 wikilink 中使用它。
- frontmatter 中的 **tags（标签）** 用于组织笔记——共享同一标签的两篇笔记被视为相关。
- **关系（Relationships）** 是任何包含 `[[wikilink]]` 的 frontmatter 属性，例如 `related_to`、`belongs_to` 或 `has`。
- 文件名使用 `snake_case.md` 命名，一个文件对应一篇笔记。



## 连接你的思考

组织知识依靠的是链接和标签，而不是文件夹。在正文或 frontmatter 的任意位置使用 `[[wikilink]]` 来连接笔记：

- `[[笔记标题]]` 链接到另一篇笔记
- `[[笔记标题|显示文本]]` 使用自定义文本进行链接

knloop 会递归读取所有文件夹中的笔记，因此你可以按任意自然的方式组织 vault——笔记的意义体现在链接和属性中，而不是目录结构里。



## 与 AI 智能体协作

knloop 天生为智能体协作而设计。智能体可以读取、搜索、创建和编辑你的笔记——遵循与 \[\[AGENTS\]\] 中描述相同的约定。请将 vault 根目录下的 `AGENTS.md` 作为人类与智能体共同的规则手册。



## 开始使用

- [x] 读到这里
- [ ] 创建一篇新笔记并为它打上标签
- [ ] 用 `[[wikilink]]` 连接两篇笔记
- [ ] 浏览笔记列表和相关笔记
- [ ] 邀请智能体协助整理你的知识库

祝笔记愉快！👋
