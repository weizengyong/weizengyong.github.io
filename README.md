# weizengyong.github.io

个人网站与 Markdown 文章博客，由 GitHub Pages 的 Jekyll 构建并发布。

## 发表文章

1. 复制 `_drafts/article-template.md`，放入 `_posts` 目录。
2. 将文件命名为 `年-月-日-英文标题.md`，例如 `2026-10-26-my-first-post.md`。日期必须使用 `YYYY-MM-DD` 格式；文件名中的英文标题会成为网址的一部分。
3. 修改文件开头的 `title`、`description` 和 `tags`，然后用 Markdown 写正文。
4. 提交并推送到 `main` 分支。GitHub Pages 发布完成后，文章会自动显示在 [文章列表](https://weizengyong.github.io/articles/) 中。

也可以直接在 GitHub 仓库网页中打开 `_posts`，点击 **Add file → Create new file**，按上述规则创建 Markdown 文件并提交。

文章网址形如 `https://weizengyong.github.io/articles/2026/10/26/my-first-post/`。如需在文章中使用图片，可将图片放在 `assets/images/`，并在 Markdown 中写 `![图片说明](/assets/images/图片文件名.png)`。

`_drafts` 中的模板不会发布；只有 `_posts` 中符合命名规则并带有 YAML 头信息的文章会出现在列表中。

## 本地预览

安装 Ruby、Bundler 与 GitHub Pages 依赖后，在仓库目录执行 `bundle exec jekyll serve`，访问 `http://localhost:4000`。直接用简单 HTTP 文件服务器不能渲染 Jekyll 的文章列表和 Markdown。

## 网站结构

- `index.html`：个人主页
- `articles.html`：自动生成文章列表，发布网址为 `/articles/`
- `_layouts/post.html`：文章页面模板
- `_posts/`：已发表文章
- `_drafts/article-template.md`：未发布的写作模板
- `style.css`：网站样式

发布源为 `main` 分支的仓库根目录。GitHub Pages 会在推送后自动构建。
