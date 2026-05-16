# AGENT.md

本仓库用于维护可通过 GitHub Pages 播放的网页 PPT。后续新建、修改 PPT 时，请遵守以下规则。

## 新建 PPT 规则

1. 每组 PPT 使用独立目录，目录内保留自己的 `index.html` 和资源文件。
2. 不改变既有 PPT 目录结构，除非用户明确要求。
3. 新建 PPT 时必须同步更新根目录 `index.html`：
   - 在 PPT 列表中新增一张卡片。
   - 填写中文标题、简短描述、日期。
   - “打开 PPT”按钮链接到对应目录的 `index.html`。
   - 如果 PPT 基于外部文章、网页或资料生成，必须加入外部来源链接，并使用 `target="_blank"` 与 `rel="noopener noreferrer"`。
   - 同步更新页面顶部总数、`aria-label` 中的总数，以及页脚 `Last updated` 日期。
4. 更新 `index.html` 后检查所有本地 PPT 链接都能指向存在的文件。
5. 不要提交 `qa/` 目录；这些目录已由 `.gitignore` 忽略。
6. 保留根目录 `.nojekyll`，以便 GitHub Pages 按静态文件发布。

## 内容安全

1. PPT 中出现家庭 IP、账号、手机号、访问令牌等敏感信息时，提交前必须脱敏。
2. 如果发现敏感信息已经进入 Git 历史，先暂停新增内容，优先清理历史并强推修复。
