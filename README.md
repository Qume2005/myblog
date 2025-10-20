# 芊墨的个人博客

这是一个使用 [Hugo](https://gohugo.io/) 静态网站生成器构建的个人博客，目前使用 [Stack](https://github.com/CaiJimmy/hugo-theme-stack) 主题。

博客地址
- 博客地址：[https://blog.liqianmo.ink/](https://blog.liqianmo.ink/)

## 🚀 快速开始

### 环境要求

- [Hugo](https://gohugo.io/getting-started/installing/) 
- Git

### 本地开发

1. 克隆仓库

```bash
git clone https://github.com/qume2005/myblog.git
cd myblog
```

2. 初始化子模块

```bash
git submodule update --init --recursive
```

3. 启动开发服务器

```bash
hugo server -D
```

4. 在浏览器中访问 `http://localhost:1313`

### 构建生产版本

```bash
hugo
```

构建后的静态文件将生成在 `public/` 目录中。

## 📁 项目结构

```
myblog/
├── assets/           # 资源文件（CSS、JS、图片等）
│   └── img/
│       └── avatar.png
├── content/          # 博客内容
│   ├── cuisine/      # 美食分类
│   └── daily-tech/   # 技术日常分类
├── data/             # 数据文件
├── i18n/             # 国际化文件
├── layouts/          # 自定义布局
├── static/           # 静态资源
├── themes/           # 主题文件
│   └── stack/        # Stack 主题（作为子模块）
├── .gitignore        # Git 忽略文件
├── .gitmodules       # Git 子模块配置
├── hugo.toml         # Hugo 配置文件
└── README.md         # 项目说明文件
```

## 📝 内容组织

### 创建新文章

使用以下命令创建新文章：

```bash
hugo new content/daily-tech/your-article-name/index.md
```

或者

```bash
hugo new content/cuisine/your-article-name/index.md
```

### 文章格式

每篇文章都应该包含前置元数据（Front Matter），例如：

```markdown
+++
date = '2025-10-15T18:00:15+08:00'
draft = true
title = '文章标题'
description = '文章描述'
tags = [
    '标签1',
    '标签2',
]
categories = [
    '分类名称',
]
+++

文章内容...
```

### 内容分类

- `cuisine/` - 美食相关内容
- `daily-tech/` - 技术日常分享

## ⚙️ 配置

主要配置文件是 `hugo.toml`，包含以下主要部分：

- 网站基本信息（标题、URL、语言等）
- 主题配置
- 侧边栏配置
- 文章配置
- 页脚配置

### 主题配置

本项目使用 Stack 主题，主题相关配置存储在 `themes/stack/` 目录中。如需自定义主题，可以：

1. 修改 `themes/stack/config.yaml`
2. 在项目根目录创建 `hugo-theme-stack-config.patch` 文件记录修改
3. 更新主题后应用 patch 文件

## 🚀 部署

### GitHub Pages

1. 将仓库推送到 GitHub
2. 在 GitHub 仓库设置中启用 GitHub Pages
3. 选择 `main` 分支作为源

## 📜 许可证

本博客内容采用 [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.en) 许可证。



## 🤝 贡献

笔者能力有限，欢迎提交 Issue 为博客提供建议和纠错，感谢您的帮助

欢迎来笔者的博客仓库 Disscussions 发帖交流🩷

## 📞 联系方式

- 邮箱：qume2005@outlook.com

---

使用 ❤️ 和 Hugo 构建