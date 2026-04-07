# Asura Blog

一个基于 GitHub Pages 的免费静态博客平台。

## ✨ 特点

- 📝 **简洁清爽** — 最小化设计，专注内容
- 🚀 **快速可靠** — 静态生成，由 GitHub Pages 支持
- 💰 **完全免费** — 无需付费，无广告
- 🌐 **支持自定义域名** — asura.forum
- 📱 **响应式设计** — 适配所有设备
- 🔍 **SEO 友好** — 完整的搜索引擎优化

## 🚀 快速开始

### 1. 克隆仓库

```bash
git clone https://github.com/solivansprvill-droid/asura-blog.git
cd asura-blog
```

### 2. 安装依赖

```bash
bundle install
```

### 3. 本地预览

```bash
bundle exec jekyll serve
```

访问 `http://localhost:4000` 查看博客。

### 4. 创建新文章

在 `_posts` 目录下创建文件，格式：`YYYY-MM-DD-title.md`

```markdown
---
layout: post
title: 我的第一篇文章
date: 2026-04-07 10:00:00 +0800
categories: [分类]
tags: [标签]
---

文章内容...
```

### 5. 推送到 GitHub

```bash
git add .
git commit -m "Add new post"
git push origin main
```

## 📁 项目结构

```
asura-blog/
├── _config.yml           # Jekyll 配置文件
├── _posts/               # 博客文章目录
│   ├── 2026-04-07-welcome.md
│   └── 2026-04-07-how-to-write.md
├── _drafts/              # 草稿目录（不发布）
├── assets/               # 静态资源（图片、CSS 等）
├── about.md              # 关于页面
├── archive.md            # 文章归档
├── index.md              # 首页
├── Gemfile               # Ruby 依赖
├── .gitignore            # Git 忽略文件
└── README.md             # 本文件
```

## 📝 文章元数据

| 字段 | 说明 | 示例 |
|------|------|------|
| `layout` | 布局类型 | `post` |
| `title` | 文章标题 | `我的第一篇文章` |
| `date` | 发布日期 | `2026-04-07 10:00:00 +0800` |
| `categories` | 分类 | `[技术, 教程]` |
| `tags` | 标签 | `[Jekyll, GitHub]` |
| `author` | 作者 | `Solivan` |

## 🌐 部署到 GitHub Pages

### 步骤 1：创建 GitHub 仓库

1. 访问 https://github.com/new
2. 创建仓库名称：`asura-blog`
3. 选择 "Public"
4. 点击 "Create repository"

### 步骤 2：配置本地仓库

```bash
git remote add origin https://github.com/YOUR_USERNAME/asura-blog.git
git branch -M main
git push -u origin main
```

### 步骤 3：启用 GitHub Pages

1. 进入仓库设置 (Settings)
2. 找到 "Pages" 部分
3. 选择 "Deploy from a branch"
4. 选择 "main" 分支
5. 点击 "Save"

### 步骤 4：等待部署

GitHub Pages 会自动构建您的博客。通常需要 1-2 分钟。

访问 `https://YOUR_USERNAME.github.io/asura-blog` 查看您的博客。

## 🔗 配置自定义域名

### 步骤 1：购买域名

在域名注册商（如 Namecheap、GoDaddy 等）购买 `asura.forum` 域名。

### 步骤 2：配置 DNS

在您的域名注册商中，添加以下 DNS 记录：

| 类型 | 名称 | 值 |
|------|------|-----|
| A | @ | `185.199.108.153` |
| A | @ | `185.199.109.153` |
| A | @ | `185.199.110.153` |
| A | @ | `185.199.111.153` |
| CNAME | www | `YOUR_USERNAME.github.io` |

### 步骤 3：配置 GitHub Pages

1. 进入仓库设置 (Settings)
2. 找到 "Pages" 部分
3. 在 "Custom domain" 输入 `asura.forum`
4. 勾选 "Enforce HTTPS"
5. 点击 "Save"

### 步骤 4：更新配置

编辑 `_config.yml`，将 `url` 改为：

```yaml
url: "https://asura.forum"
```

推送更改：

```bash
git add _config.yml
git commit -m "Update domain to asura.forum"
git push origin main
```

## 📚 Markdown 语法

### 标题

```markdown
# 一级标题
## 二级标题
### 三级标题
```

### 文本格式

```markdown
**粗体**
*斜体*
~~删除线~~
```

### 列表

```markdown
- 无序项 1
- 无序项 2

1. 有序项 1
2. 有序项 2
```

### 链接和图片

```markdown
[链接文本](https://example.com)
![图片描述](image-url)
```

### 代码

```markdown
`行内代码`

\`\`\`python
# 代码块
print("Hello, World!")
\`\`\`
```

### 引用

```markdown
> 这是一个引用
> 可以有多行
```

## 🛠️ 常用命令

```bash
# 安装依赖
bundle install

# 本地预览
bundle exec jekyll serve

# 构建静态网站
bundle exec jekyll build

# 清理构建文件
bundle exec jekyll clean

# 查看 Jekyll 版本
bundle exec jekyll --version
```

## 📖 更多资源

- [Jekyll 官方文档](https://jekyllrb.com/)
- [Markdown 语法指南](https://www.markdownguide.org/)
- [GitHub Pages 文档](https://docs.github.com/en/pages)

## 📄 许可证

MIT License - 详见 LICENSE 文件

## 👤 作者

**Solivan**
- 邮箱：shengli621@foxmail.com
- GitHub：[@solivansprvill-droid](https://github.com/solivansprvill-droid)

---

**最后更新：** 2026年4月7日

感谢您使用 Asura Blog！
