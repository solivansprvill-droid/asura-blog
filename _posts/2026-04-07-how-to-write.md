---
layout: post
title: 如何在 Asura Blog 上写文章
date: 2026-04-07 11:00:00 +0800
categories: [教程, 指南]
tags: [写作, GitHub]
author: Solivan
---

# 如何在 Asura Blog 上写文章

这是一个详细的教程，教您如何在 Asura Blog 上发布文章。

## 步骤 1：准备您的文章

首先，准备您想要发布的文章内容。您可以使用 Markdown 格式编写。

## 步骤 2：创建文件

在 `_posts` 目录下创建一个新的 Markdown 文件。文件名必须遵循以下格式：

```
YYYY-MM-DD-title-of-post.md
```

例如：
- `2026-04-07-my-first-post.md`
- `2026-04-08-hello-world.md`

## 步骤 3：添加元数据

在文件的最顶部，添加 YAML 前置元数据（Front Matter）：

```yaml
---
layout: post
title: 您的文章标题
date: 2026-04-07 10:00:00 +0800
categories: [分类1, 分类2]
tags: [标签1, 标签2]
author: 作者名
---
```

### 元数据说明

| 字段 | 说明 | 示例 |
|------|------|------|
| `layout` | 布局类型 | `post` |
| `title` | 文章标题 | `我的第一篇文章` |
| `date` | 发布日期和时间 | `2026-04-07 10:00:00 +0800` |
| `categories` | 文章分类 | `[技术, 教程]` |
| `tags` | 文章标签 | `[Jekyll, GitHub]` |
| `author` | 作者名 | `Solivan` |

## 步骤 4：编写文章内容

在元数据下方，使用 Markdown 格式编写您的文章内容。

### Markdown 基本语法

```markdown
# 一级标题
## 二级标题
### 三级标题

**粗体文本**
*斜体文本*

- 列表项 1
- 列表项 2
- 列表项 3

1. 有序项 1
2. 有序项 2
3. 有序项 3

[链接文本](https://example.com)

![图片描述](image-url)

> 引用文本

\`\`\`python
# 代码块
print("Hello, World!")
\`\`\`
```

## 步骤 5：推送到 GitHub

完成文章后，将文件推送到 GitHub 仓库：

```bash
git add _posts/2026-04-07-my-post.md
git commit -m "Add new post: My Post Title"
git push origin main
```

## 步骤 6：等待发布

GitHub Pages 会自动构建您的博客。通常需要 1-2 分钟。之后，您的文章就会在博客上显示！

## 提示和技巧

### 使用草稿

如果您想保存文章但不想发布，可以将文件放在 `_drafts` 目录中：

```bash
mkdir -p _drafts
# 将文件移到 _drafts 目录
```

### 添加图片

将图片放在 `assets/images/` 目录中，然后在文章中引用：

```markdown
![描述]({{ site.baseurl }}/assets/images/image-name.jpg)
```

### 使用代码高亮

Jekyll 支持多种编程语言的代码高亮：

\`\`\`javascript
function hello() {
  console.log("Hello, World!");
}
\`\`\`

### 本地预览

在推送前，您可以在本地预览博客：

```bash
bundle exec jekyll serve
# 访问 http://localhost:4000
```

## 常见问题

**Q: 文章发布后多久会显示？**  
A: 通常 1-2 分钟。如果没有显示，请检查文件名和元数据格式。

**Q: 我可以编辑已发布的文章吗？**  
A: 可以。编辑文件后推送，GitHub Pages 会自动更新。

**Q: 如何删除文章？**  
A: 从 `_posts` 目录中删除文件，然后推送到 GitHub。

---

祝您写作愉快！
