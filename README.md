# weizengyong.github.io

一个无需构建工具的个人网站，可直接由 GitHub Pages 发布。

## 本地预览

在仓库目录运行 `python -m http.server 8000`，然后访问 `http://localhost:8000`。

## 发布到 GitHub Pages

1. 在 GitHub 创建公开仓库 `weizengyong.github.io`。
2. 将本目录推送到该仓库的默认分支。
3. 在仓库的 **Settings → Pages** 中选择 **Deploy from a branch**，分支选默认分支，目录选 **/(root)**。
4. 发布后访问 `https://weizengyong.github.io/`。

网站文案与项目链接在 `index.html` 中修改；样式在 `style.css` 中修改。GitHub Pages 会直接读取仓库根目录的 `index.html`。
