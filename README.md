# KeenJoe's Blog

基于 [Hugo](https://gohugo.io/) + [Hextra](https://github.com/imfing/hextra) 构建的个人技术博客，部署在 GitHub Pages。

## 本地开发

```bash
# 安装 Hugo（macOS）
brew install hugo

# 克隆仓库
git clone https://github.com/keenJoe/keenJoe.github.io.git
cd keenJoe.github.io

# 本地预览
hugo server -D

# 构建
hugo --minify
```

## 写新文章

在 `content/blog/` 目录下创建 Markdown 文件：

```bash
hugo new content/blog/my-new-post.md
```

编辑文章内容，将 `draft: true` 改为 `draft: false` 后推送即可发布。

## 部署

推送到 `main` 分支后，GitHub Actions 会自动构建并部署到 GitHub Pages。
