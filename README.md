# 视频浏览网站

一个简单而优雅的网站，用于在线浏览视频文件。

## 功能特点

- 响应式设计，支持移动设备
- 现代化的深色主题界面
- 自定义视频控制按钮
- 显示视频时长和文件大小
- 支持全屏播放
- 使用 GitHub Pages 免费托管

## 部署步骤

### 1. 创建 GitHub 仓库

1. 访问 [github.com](https://github.com)
2. 点击 "New repository"
3. 仓库名称建议：`video-website`
4. 设置为 Public（免费版只能使用公开仓库）
5. 点击 "Create repository"

### 2. 上传文件

将以下文件上传到你的仓库：
- `index.html` - 主页面
- `张栩的自我介绍.mp4` - 视频文件
- `.github/workflows/deploy.yml` - 自动部署配置
- `package.json` - 项目配置

你可以通过以下方式上传：

**方法一：GitHub 网页界面上传**
1. 在仓库页面，点击 "Add file" → "Upload files"
2. 拖拽或选择文件上传
3. 写入提交信息，点击 "Commit changes"

**方法二：使用 Git 命令**
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/your-username/video-website.git
git push -u origin main
```

### 3. 启用 GitHub Pages

1. 在仓库页面，点击 "Settings"
2. 找到左侧菜单中的 "Pages"
3. 在 "Build and deployment" 部分：
   - Source 选择 "Deploy from a branch"
   - Branch 选择 "main"
   - Folder 选择 "/ (root)"
4. 点击 "Save"

### 4. 访问网站

部署完成后，你的网站将在以下地址可用：
```
https://your-username.github.io/video-website
```

> 提示：首次部署可能需要几分钟时间。

## 本地预览

如果你想本地预览网站，可以使用以下命令：

```bash
# 安装 Node.js（如果还没有）
# 访问 https://nodejs.org 下载并安装

# 安装依赖（可选）
npm install

# 启动本地服务器
npm run start

# 打开浏览器访问 http://localhost:8000
```

## 自定义

### 修改视频文件

1. 替换 `张栩的自我介绍.mp4` 为你的视频文件
2. 更新 `index.html` 中的视频源路径

### 修改样式

编辑 `index.html` 中的 `<style>` 部分来自定义网站外观。

### 修改标题和描述

编辑 `index.html` 中的标题和描述文本。

## 故障排除

### 视频无法播放

- 确保 video 文件已成功上传
- 检查文件名是否正确
- 确保视频格式支持（MP4 最兼容）

### 网站无法访问

- 检查 GitHub Pages 是否已启用
- 等待 5-10 分钟让部署完成
- 检查分支名称是否为 "main"

## 许可证

MIT License

## 支持

如有问题，请提交 Issue。