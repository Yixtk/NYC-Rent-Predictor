# GitHub Pages 部署指南

## 步骤 1: 在 GitHub 上创建新仓库

1. 登录 GitHub (https://github.com)
2. 点击右上角 "+" → "New repository"
3. 仓库名称：例如 `nyc-rent-predictor`（可以自定义）
4. 选择 Public（必须，GitHub Pages 免费版需要公开仓库）
5. **不要**勾选 "Initialize with README"（我们已经有了）
6. 点击 "Create repository"

## 步骤 2: 连接本地仓库到 GitHub

复制以下命令，将 `YOUR_USERNAME` 替换为你的 GitHub 用户名，`YOUR_REPO_NAME` 替换为你的仓库名：

```bash
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git branch -M main
git push -u origin main
```

## 步骤 3: 启用 GitHub Pages

1. 在 GitHub 仓库页面，点击 "Settings"（设置）
2. 左侧菜单找到 "Pages"
3. 在 "Source" 下选择：
   - Branch: `main`
   - Folder: `/ (root)`
4. 点击 "Save"
5. 等待几分钟，GitHub 会生成你的网站地址：
   - 格式：`https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/predictor.html`

## 访问你的网站

部署成功后，访问：
```
https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/predictor.html
```

## 提示

- 如果想让 `predictor.html` 成为主页，可以将其重命名为 `index.html`
- 更新代码后，运行 `git push` 即可自动更新网站

