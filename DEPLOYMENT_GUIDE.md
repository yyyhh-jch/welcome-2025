# 🚀 部署指南：发布到GitHub Pages

## 📋 简单步骤

### 1️⃣ 上传到GitHub
1. 打开 [GitHub.com](https://github.com) 并登录
2. 点击右上角的 `+` → `New repository`
3. 仓库名称建议填写：`yyyhh-jch-residence` 或 `residence-website`
4. 选择 `Public`（这样别人才能访问）
5. 不要勾选 "Add a README file"（我们已经有了）
6. 点击 `Create repository`

### 2️⃣ 上传文件
有两种方法：

**方法A：网页上传（简单）**
1. 在新创建的仓库页面，点击 `uploading an existing file`
2. 把整个 `residence` 文件夹里的所有文件拖拽到页面上
3. 写个提交信息，比如："Add YYYHH & JCH residence website"
4. 点击 `Commit changes`

**方法B：命令行（如果您熟悉）**
```bash
git remote add origin https://github.com/您的用户名/您的仓库名.git
git branch -M main
git push -u origin main
```

### 3️⃣ 启用GitHub Pages
1. 在仓库页面，点击 `Settings`
2. 左侧菜单找到 `Pages`
3. 在 "Source" 下选择 `Deploy from a branch`
4. Branch 选择 `main` 或 `master`
5. 文件夹选择 `/ (root)`
6. 点击 `Save`

### 4️⃣ 访问您的网站！
等待2-5分钟，您的网站就会在以下地址可用：
```
https://您的GitHub用户名.github.io/您的仓库名/
```

## 🎯 就是这么简单！

**当前您的文件夹结构：**
```
residence/
├── index.html          ✅ 主页面
├── styles.css          ✅ 样式文件  
├── logo.png           ✅ Logo图片
├── qr-codes/          ✅ QR码文件夹
│   ├── floor_1.jpg    ✅ 所有QR码
│   └── ...
└── 其他文件            ✅ 说明文档等
```

**上传后别人就能通过网址看到您的网站了！**

## 🔄 以后更新QR码

更新很简单：
1. 替换 `qr-codes/` 文件夹中的图片
2. 重新上传到GitHub（或者用git push）
3. 网站自动更新！

## 💡 小贴士

- 仓库名会成为网址的一部分，所以起个好记的名字
- 确保选择 `Public` 才能让别人访问
- 第一次部署可能需要等几分钟
- 每次更新文件后，网站会自动更新（可能需要几分钟）