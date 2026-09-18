# The chicken lays eggs 🐔🥚

> 一个从零开始的小项目。先放了个网页起点，以后可以换成 / 加上可执行程序。

## 这是什么

目前仓库里是一个**最简单的网页起点**（`index.html`），打开就能看到效果，
不需要安装任何东西。你可以把它当作占位，慢慢改成自己真正想要的东西。

## 目录结构

```
The-chicken-lays-eggs/
├── index.html      # 网页入口，双击即可在浏览器打开
├── .gitignore      # 告诉 Git 哪些文件不要提交
└── README.md       # 你正在看的说明
```

## 如何预览（网页）

直接用浏览器打开 `index.html` 即可。
或者在该文件夹下运行一个本地服务器：

```bash
# 如果你装了 Python
python -m http.server 8000
# 然后浏览器访问 http://localhost:8000
```

## 你接下来可以做的方向

- **继续做网页**：在 `index.html` 里加内容，或新建 `style.css` / `script.js`。
- **改成可执行程序**：新建 `main.py`（Python）或 `main.c` 等，删掉不想要的网页文件即可。
- **写文档**：在这里补充项目说明、用法、设计思路。

## Git 基本流程（以后每天都会用到）

```bash
git status        # 看改了哪些文件
git add .         # 把改动加入暂存区
git commit -m "说明这次改了什么"   # 提交到本地
git push          # 推送到 GitHub
```

> 小贴士：每次写一段就 `add` + `commit` 一次，别等攒一大堆再提交，
> 这样以后回看历史会很清楚。
