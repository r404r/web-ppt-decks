# Web PPT Decks

这个仓库用于托管可在浏览器中直接播放的 PPT / slide deck。每组 PPT 保持独立目录，根目录 `index.html` 作为统一播放目录。

## 在线访问

- PPT 目录页：https://r404r.github.io/web-ppt-decks/

## 当前结构

- `index.html`：所有 PPT 的入口页。
- `.nojekyll`：让 GitHub Pages 按静态站点直接发布，避免 Jekyll 处理资源路径。
- `*/index.html`：每组 PPT 的播放入口。
- `*/images/`：对应 PPT 的图片与 SVG 资源。
- `**/qa/`：生成与检查过程中的临时 QA 产物，已在 `.gitignore` 中忽略。

## 维护约定

新增 PPT 时，请同时更新根目录 `index.html`，为新 PPT 增加标题、描述、日期、打开按钮；如果 PPT 基于外部文章生成，也要加入原文链接。
