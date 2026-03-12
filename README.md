# 秦野科创 · CVA 组织（Hexo + Stellar）

Hexo 8 站点，主题为 [hexo-theme-stellar](https://github.com/xaoxuu/hexo-theme-stellar)。首页通过 `source/_data/qxf.yml` + 自定义样式 `source/css/home.css` 渲染科技风模块（Hero、CVA、项目、时间线、联系）。

## 技术栈
- Hexo 8.x
- hexo-theme-stellar（定制首页 layout）
- 数据源：`source/_data/qxf.yml`

## 安装 & 运行
```bash
npm install
npm run dev   # http://localhost:4000
```

## 构建
```bash
npm run build
```

## 内容与样式
- 文案/模块：`source/_data/qxf.yml`
- 首页样式：`source/css/home.css`
- 主题配置：`themes/stellar/_config.yml`
- 如需回到自研主题，可把 `_config.yml` 中 `theme` 改回 `qxf-tech`

## 部署
可继续用 GitHub Pages（Settings → Pages）或在 `_config.yml` 中配置 `deploy` 后执行 `hexo deploy`。

## 部署 (GitHub Pages)
1. 仓库 Settings → Actions → General 中把 Workflow permissions 设为 **Read and write**。
2. 确认 `.github/workflows/deploy.yml` 已存在（我已创建）。
3. 每次 push 到 `main`，GitHub Actions 会自动执行：`npm ci` → `npm run build` → 将 `public/` 发布到 `gh-pages` 分支。
4. 仓库 Settings → Pages 选择来源 `gh-pages` / `root`，几分钟后即可通过 `https://qxf19.github.io/qxf19751212/` 访问。
