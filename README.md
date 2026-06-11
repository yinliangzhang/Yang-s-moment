# 万里茶道 · 数据看板

老杨万里茶道 IP 的双平台数据看板 + 战略资产合集。纯静态站点（16 个自包含 HTML，无构建、无外部依赖），首页 `index.html` 为导航中枢。

## 内容

- **主看板**：起号期驾驶舱（双平台横向对比）
- **战略**：战略看板·麦肯锡版 · 张老师·战略地图 · 杨老师·战略地图
- **下钻**：小红书单篇 ×5 · 视频号单条 ×4
- **文档**：三周战报

## 部署到 Netlify

### 方式一 · GitHub 自动部署（推荐，改完一推送自动更新）
1. 把本仓库推到 GitHub
2. 登录 [Netlify](https://app.netlify.com) → Add new site → Import an existing project → 选本仓库
3. 构建设置留空（Publish directory = `.`，已由 `netlify.toml` 指定），Deploy
4. 之后每次 `git push`，Netlify 自动重新部署

### 方式二 · 直接拖（最快，无需 GitHub）
把整个文件夹拖到 [app.netlify.com/drop](https://app.netlify.com/drop)

## 说明

- 所有页面靠**相对路径**互链，必须整体部署，不可拆分单页。
- 字体已全部改为系统字体栈，**无 Google Fonts 依赖**，中国大陆访问正常。
- 如需**访问密码**：Netlify 免费版不含站点密码，可在 `index.html` 注入 JS 密码门实现。
