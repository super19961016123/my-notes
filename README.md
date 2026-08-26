# 我的笔记 · 个人知识库

一个单文件、全端自适应的个人笔记网站。部署在 GitHub Pages，手机、平板、电脑打开同一网址即可阅读。

## 项目结构

```
personal-notes-site/
├── index.html   # 唯一网页文件：样式 + 数据 + 逻辑全部内联
└── README.md
```

## 如何更新笔记

**你不需要写任何代码。** 把整理好的笔记发给豆包，豆包会：

1. 编辑 `index.html` 底部 `SITE.categories` 数据块（新增/修改分类和笔记）
2. 本地预览确认排版
3. `git commit` 并 `git push` 到 GitHub 主分支
4. GitHub Pages 自动重新构建，通常 1 分钟内网址即可看到最新内容

## 排版与样式调整

同样告诉豆包即可，例如：

- 新增/重命名/删除分类
- 调整字号、行距、主题色、深浅色
- 修改页头标题、站点名称

## 本地预览

```bash
cd personal-notes-site
python3 -m http.server 8000
# 浏览器打开 http://localhost:8000
```

## 部署说明

站点托管于 GitHub Pages：

- 仓库：`<你的用户名>/<仓库名>`
- 设置 → Pages → Deploy from a branch → 选择 `main` 分支根目录
- 访问地址：`https://<你的用户名>.github.io/<仓库名>/`
