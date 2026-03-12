# 秦野科创 · CVA 组织（Hexo 站点）

一个基于 Hexo + 自定义主题 `qxf-tech` 的纯静态网站，用来展示“秦野科创，也为改变生活”的理念与 CVA 组织的技术实践。

## 技术栈
- [Hexo 8](https://hexo.io/)
- 自定义主题：`themes/qxf-tech`（深色科技风、无第三方依赖）
- 站点数据集中存放在 `source/_data/qxf.yml`

## 本地运行
```bash
# 安装依赖
npm install

# 启动本地预览（默认 http://localhost:4000）
npm run dev
```

## 构建 & 发布
```bash
# 构建静态文件（输出到 public/）
npm run build

# 清理缓存/构建目录
npm run clean
```

若要部署到 GitHub Pages，可在仓库 Settings → Pages 中选择 `Actions` 或 `main / public`，或使用 Hexo Deploy（需要在 `_config.yml` 里补全 `deploy` 设置）。

## 内容管理
- 修改站点文案/模块：编辑 `source/_data/qxf.yml`
- 若需新增模块，可在 `themes/qxf-tech/layout/index.ejs` 中扩展结构
- 样式位于 `themes/qxf-tech/source/css/style.css`
- 轻量脚本位于 `themes/qxf-tech/source/js/main.js`

## 目录速览
```
qxf19751212/
├── _config.yml                # 全局配置（站点信息、主题等）
├── package.json               # npm 脚本 & 依赖
├── source/_data/qxf.yml       # 驱动首页的内容数据
└── themes/qxf-tech/           # 自定义主题
```

欢迎继续迭代：可添加博客文章、把数据拆到 CMS，或集成部署流水线。需要我扩展模块或适配其它主题，再喊我。