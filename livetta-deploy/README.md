# LIVETTA 网站部署指南

## 📦 部署包内容
- `index.html` - 主网站文件
- `vercel.json` - Vercel 配置文件(包含安全头和URL优化)

## 🚀 快速部署到 Vercel

### 方法 1: 直接上传(最简单)
1. 访问 https://vercel.com
2. 注册/登录账号
3. 点击 "Add New..." → "Project"
4. 选择 "Deploy from Files"
5. 上传整个 `livetta-deploy` 文件夹
6. 点击 "Deploy"

### 方法 2: 通过 CLI 部署
```bash
npm i -g vercel
cd livetta-deploy
vercel
```

## 🌐 域名配置

### 在 Vercel 中添加域名
1. 进入项目 Settings → Domains
2. 输入: livetta.net
3. 点击 Add

### 在 NameCheap 配置 DNS
Advanced DNS → Add New Record:

**A Record:**
- Type: A Record
- Host: @
- Value: 76.76.21.21
- TTL: Automatic

**CNAME Record:**
- Type: CNAME Record
- Host: www
- Value: cname.vercel-dns.com
- TTL: Automatic

## ⏱️ 生效时间
- DNS 生效: 5分钟 - 48小时(通常10-30分钟)
- SSL 证书: Vercel 自动配置(免费)

## ✅ 验证部署
访问以下地址检查:
- https://livetta.net
- https://www.livetta.net

## 📝 其他部署选项

### Netlify (替代方案)
1. 访问 https://netlify.com
2. 拖拽 `livetta-deploy` 文件夹到部署区
3. 在 Domain Settings 中添加自定义域名

### GitHub Pages (免费方案)
1. 创建 GitHub 仓库
2. 上传文件
3. 启用 Pages 功能
4. 配置自定义域名

## 🔧 联系信息更新
记得在网站上线后更新:
- 电话号码
- 邮箱地址
- 实际营业时间

## 📞 技术支持
如有问题,请联系 Vercel 支持或查看文档:
- Vercel 文档: https://vercel.com/docs
- NameCheap 支持: https://www.namecheap.com/support/

---
创建日期: 2024年12月14日
