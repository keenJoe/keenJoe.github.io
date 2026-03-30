# KeenJoe's Blog

基于 [Hugo](https://gohugo.io/) + [PaperMod](https://github.com/adityatelange/hugo-PaperMod) 构建的个人技术博客，部署在 GitHub Pages。

## 本地开发

```bash
# 安装 Hugo（macOS）
brew install hugo

# 克隆仓库（含主题子模块）
git clone --recursive https://github.com/keenJoe/keenJoe.github.io.git
cd keenJoe.github.io

# 本地预览
hugo server -D

# 构建
hugo --minify
```

## 写新文章

```bash
hugo new posts/my-new-post.md
```

然后编辑 `content/posts/my-new-post.md`，将 `draft: true` 改为 `draft: false` 后推送即可发布。

## 部署

推送到 `main` 分支后，GitHub Actions 会自动构建并部署到 GitHub Pages。
