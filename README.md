# Xuxuan Lin’s academic homepage

英文站使用 [AcadHomepage](https://github.com/RayeRen/acad-homepage.github.io) 的 Jekyll 模板。模板许可见 `LICENSE`。

## 本地预览

双击 `_site/index.html` 可以查看随项目附带的构建结果。修改源文件后，在项目目录运行：

```sh
bundle install
bundle exec jekyll serve
```

浏览器打开 `http://localhost:4000`。

## 编辑与发布

- 个人资料和联系方式在 `_config.yml`。
- 教育经历、论文、折叠论文和奖项分别在 `_data/education.yml`、`_data/publications.yml`、`_data/side_paper.yml`、`_data/awards.yml`。
- 首页在 `_pages/about.md`。首页按顺序展示前五篇论文，`publications.html` 展示完整列表。
- 论文配图和 PDF 分别放在 `files/IMG/` 和 `files/PDF/`。
- 发布到 GitHub Pages 时，将本目录的源码放在目标仓库根目录，在 Settings → Pages 选择对应分支和 `/(root)`。本地构建目录 `_site/` 已列入 `.gitignore`。
