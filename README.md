## 个人主页

> 探索未知，代码为舟

一个现代化的个人主页，采用 Vue 3 + 深色科技主题设计。

**目标主页地址：** [https://roskyrie.github.io/home/](https://roskyrie.github.io/home/)

此地址需要将本项目部署到 GitHub 账号 `roskyrie` 下的 `home` 仓库后才会生效。

## 特性

- **Vue 3 驱动** - 数据驱动的响应式页面
- **深色科技主题** - 粒子动画背景 + 霓虹光效
- **响应式设计** - 完美适配桌面端与移动端
- **滚动动画** - Intersection Observer 实现的入场动画
- **打字机效果** - 动态切换的标题文字

## 技术栈

- Vue 3 (CDN)
- 原生 CSS3 (Grid + Flexbox)
- Canvas 粒子动画
- Remix Icon 图标库

## 快速开始

```bash
# 本地预览
npx serve . -p 3000

# 或使用 Python
python -m http.server 3000
```

## 部署支持

本项目支持以下静态托管平台一键部署：

| 平台 | 配置文件 | 说明 |
|------|----------|------|
| GitHub Pages | `.github/workflows/deploy.yml` | 推送自动部署 |
| Vercel | `vercel.json` | 导入仓库即可 |
| Netlify | `netlify.toml` | 导入仓库即可 |
| EdgeOne Pages | `edgeone.json` | 腾讯云 EdgeOne |

### GitHub Pages 部署

1. 登录 `roskyrie` 账号，在该账号下创建或 Fork 名为 `home` 的仓库，并上传本项目
2. 启用 GitHub Pages (Settings → Pages → Source: GitHub Actions)
3. 推送到 `master` 或 `main` 分支，自动触发部署；如果是 Fork，先在 Actions 页面启用工作流
4. 在 Actions 中确认部署成功，再访问 [个人主页](https://roskyrie.github.io/home/)

GitHub Pages 项目站点的默认地址由仓库所属账号和仓库名决定。仅修改本文件或 `package.json` 不会改变线上地址；需要目标仓库实际属于 `roskyrie`。迁移完成后，本地远程地址应改为 `https://github.com/roskyrie/home.git`。

### Vercel 部署

```bash
# 安装 Vercel CLI
npm i -g vercel

# 部署
vercel
```

### Netlify 部署

1. 连接 GitHub 仓库
2. 构建命令留空，发布目录填 `.`

## 项目结构

```
├── index.html          # 主页面 (Vue 3)
├── static/
│   └── css/
│       └── index.css   # 样式文件
├── vercel.json         # Vercel 配置
├── netlify.toml        # Netlify 配置
├── edgeone.json        # EdgeOne 配置
├── package.json        # 项目配置
└── .github/
    └── workflows/
        └── deploy.yml  # GitHub Actions 部署
```

## 自定义

修改 `index.html` 中的数据对象即可自定义内容：

```javascript
const site = reactive({
    name: '未寻',           // 站点名称
    slogan: '探索未知，代码为舟'
});

const profile = reactive({
    avatar: '...',         // 头像 URL
    title: '...',          // 职位
    bio: '...'             // 简介
});
```

## 外部 API

- [一言](https://hitokoto.cn/) - 随机名言
- [今日诗词](https://www.jinrishici.com/) - 古诗词
- [不蒜子](http://busuanzi.ibruce.info/) - 访客统计

## License

[MIT License](LICENSE)

Copyright (c) 2019-present 未寻

本项目采用 MIT 协议开源，您可以：
- ✅ 商业使用
- ✅ 修改代码
- ✅ 分发副本
- ✅ 私人使用

唯一要求是在副本中保留版权声明和许可声明。
