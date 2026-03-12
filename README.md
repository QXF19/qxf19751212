# 秦野科创 · CVA 组织个人科技站

纯静态网站，用于展示“秦野科创，也为改变生活”的技术理念与 CVA 组织的实践。

## 结构
- `index.html`：页面结构与文案
- `styles.css`：深色科技感样式
- `main.js`：当前年份等轻量交互

## 本地开发
```bash
# 进入项目目录
cd qxf19751212

# 启动一个本地静态服务器（任选其一）
python3 -m http.server 8000
# 或
npx serve .
```
然后访问 `http://localhost:8000` 查看页面。

## Git 操作
```bash
# 初始化（若尚未）
git init

git add .
git commit -m "feat: init qxf19751212 site"

# 远端仓库（示例）
gh repo create qxf19751212 --public --source=. --remote=origin --push
```
如果仓库已经存在，则：
```bash
git remote add origin git@github.com:<your-account>/qxf19751212.git
git push -u origin main
```

## 后续修改
- 更新 `index.html` 中的项目、时间线与文案即可。
- 若需要多页面或博客，可把结构扩展成 Hugo/VitePress 等静态站点。当前版本保持零依赖，方便快速托管到 GitHub Pages。
