# love-letter-mobile

一个适配手机端的互动情书网页，可直接发布到 GitHub Pages 给手机打开。

## 功能

- 三关互动小游戏
  - 第一关：接照片
  - 第二关：记照片
  - 第三关：找不同照片
- 每关解锁一段情话
- 支持背景音乐播放
- 最终展示完整情书
- 支持点击“我们的回忆”切换照片（淡入淡出）

## 项目结构

```text
love-letter-mobile/
├── index.html
├── README.md
├── DEPLOY.md
├── .gitignore
└── assets/
    ├── music.m4a
    └── photos/
        ├── 01.jpg
        ├── 02.jpg
        ├── 03.jpg
        ├── 04.jpg
        ├── 05.jpg
        ├── 06.jpg
        ├── 07.jpg
        ├── 08.jpg
        ├── 09.jpg
        └── 10.jpg
```

## 本地打开

方式一：直接双击 `index.html`

方式二：本地静态服务

```bash
cd /Users/link/.openclaw/workspace-main/love-letter-mobile
python3 -m http.server 8000
```

然后浏览器打开：

`http://127.0.0.1:8000`

## GitHub Pages 发布

详细步骤见：

- `DEPLOY.md`

## 可自定义内容

你可以直接修改 `index.html` 里的：

- 标题文案
- 三关游戏难度
- 每关解锁文案
- 最终完整情书
- 回忆照片区说明文案
- 背景音乐文件
- 照片素材

## 注意

- 手机浏览器通常需要用户手动点击后才允许播放音乐
- 发布到 GitHub Pages 时，请确保上传的是当前文件夹内的内容，而不是外层再套一层目录
- 当前项目资源已使用相对路径，适合直接部署
