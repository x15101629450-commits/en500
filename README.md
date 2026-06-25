# 500 常用英语单词

单页静态网站：500 个常用英语单词，支持搜索、发音、高亮、回收站。纯 HTML，无需构建。

## 本地预览

直接用浏览器打开 `index.html`，或：

```bash
python3 -m http.server 8080
# 访问 http://localhost:8080
```

## 部署到 GitHub Pages（外网访问）

1. 在 GitHub 新建仓库，例如 `en500`（Public）
2. 本地 push：

```bash
cd en500
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin git@github.com:x15101629450-commits/en500.git
git push -u origin main
```

3. 仓库 **Settings → Pages → Source** 选 **GitHub Actions**
4. 等 Actions 部署完成，访问：

```
https://x15101629450-commits.github.io/en500/
```

## 说明

- 数据和学习进度（高亮、回收站）保存在浏览器 `localStorage`
- 发音功能依赖浏览器 `speechSynthesis`（Chrome / Safari 支持较好）
