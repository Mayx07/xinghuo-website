# 星火集网站部署指南

## 📁 项目文件

```
xinghuo-website/
├── index.html          # 主页（已优化SEO）
├── privacy.html        # 隐私政策
├── README.md          # 项目说明
├── package.json       # 项目配置
└── vercel.json        # Vercel部署配置
```

## 🚀 部署到Vercel（推荐）

### 方法1：通过网页界面（最简单）

1. **访问Vercel**
   - 打开：https://vercel.com
   - 点击右上角 "Sign Up" 或 "Login"

2. **使用GitHub登录**
   - 选择 "Continue with GitHub"
   - 授权Vercel访问你的GitHub

3. **导入项目**
   - 点击 "Add New..." → "Project"
   - 选择 "Import Git Repository"
   - 如果还没有上传到GitHub，选择 "Import from template" 或直接拖拽文件夹

4. **配置项目**
   - Project Name: `xinghuo` 或你喜欢的名字
   - Framework Preset: 选择 "Other"
   - Root Directory: `./`
   - 点击 "Deploy"

5. **等待部署**
   - 大约30秒-1分钟
   - 完成后会显示：✅ Deployment Ready

6. **获取网址**
   - 你会得到一个网址：`https://xinghuo.vercel.app`
   - 或者 `https://your-project-name.vercel.app`

### 方法2：通过Git（推荐长期使用）

1. **初始化Git仓库**
```bash
cd "D:\阶跃\xinghuo-website"
git init
git add .
git commit -m "Initial commit: 星火集网站"
```

2. **创建GitHub仓库**
   - 访问：https://github.com/new
   - Repository name: `xinghuo-website`
   - 设为 Public（公开）
   - 点击 "Create repository"

3. **推送到GitHub**
```bash
git remote add origin https://github.com/你的用户名/xinghuo-website.git
git branch -M main
git push -u origin main
```

4. **在Vercel导入**
   - 回到Vercel
   - 点击 "Import Project"
   - 选择你刚创建的GitHub仓库
   - 点击 "Deploy"

5. **自动部署**
   - 以后每次push到GitHub，Vercel会自动重新部署
   - 非常方便！

## 🌐 部署到其他平台

### Netlify（备选方案）

1. 访问：https://netlify.com
2. 拖拽 `xinghuo-website` 文件夹到页面
3. 完成！获得网址

### GitHub Pages（免费）

1. 在GitHub仓库设置中
2. 找到 "Pages" 选项
3. Source选择 "main" 分支
4. 保存，获得网址：`https://你的用户名.github.io/xinghuo-website`

## ✅ 部署后检查清单

- [ ] 网站能正常访问
- [ ] 移动端显示正常
- [ ] 所有链接都能点击
- [ ] 图标显示正常
- [ ] 分享到社交媒体测试

## 🔧 自定义域名（可选）

如果你购买了域名（如 xinghuo.com）：

1. 在Vercel项目设置中
2. 找到 "Domains"
3. 添加你的域名
4. 按照提示配置DNS
5. 等待生效（几分钟到24小时）

## 📊 查看统计数据

部署后，你可以在Vercel看到：
- 访问量
- 部署历史
- 性能指标

## 🆘 遇到问题？

常见问题：
1. **部署失败** - 检查文件名是否正确
2. **页面空白** - 检查浏览器控制台错误
3. **样式丢失** - 确保CDN链接可访问

## 📞 需要帮助

如果遇到任何问题，我随时可以帮你！
