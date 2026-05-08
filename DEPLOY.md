# GitHub 发布指引（手机可打开）

这个项目是纯静态网页，最适合用 **GitHub Pages** 发布。

## 一、发布前确认

请确认以下文件都在项目目录中：

- `index.html`
- `assets/music.m4a`
- `assets/photos/01.jpg` ~ `10.jpg`

项目目录：

`/Users/link/.openclaw/workspace-main/love-letter-mobile`

## 二、上传到 GitHub

### 方式 A：网页手动上传（最简单）

1. 打开 GitHub，新建一个仓库
   - 例如仓库名：`love-letter-mobile`
2. 进入仓库首页
3. 点击 **Add file** → **Upload files**
4. 把整个 `love-letter-mobile` 文件夹里的内容拖进去
   - 注意：是把 **文件夹里的内容** 上传，不是再套一层 `love-letter-mobile/`
5. 提交保存（Commit changes）

### 方式 B：Git 命令上传

```bash
cd /Users/link/.openclaw/workspace-main/love-letter-mobile
git init
git add .
git commit -m "init love letter site"
git branch -M main
git remote add origin 你的仓库地址
git push -u origin main
```

## 三、开启 GitHub Pages

1. 打开 GitHub 仓库
2. 点 **Settings**
3. 左侧找到 **Pages**
4. 在 **Build and deployment** 里设置：
   - **Source**：Deploy from a branch
   - **Branch**：`main`
   - 文件夹：`/ (root)`
5. 点击 **Save**

等几十秒到几分钟，GitHub 会生成一个公开链接。

链接通常类似：

`https://你的用户名.github.io/love-letter-mobile/`

## 四、手机打开

生成链接后：

- 直接把链接发到自己微信/QQ/短信
- 在手机浏览器打开即可
- 建议用手机先完整试玩一遍，确认：
  - 图片显示正常
  - 音乐能否播放
  - 三关按钮点击正常

## 五、注意事项

### 1. 音乐播放
手机浏览器通常要求用户手动点击后才能播放音乐，所以这是正常的。

### 2. 仓库公开性
如果你用 GitHub Pages 免费版，通常需要公开仓库。
如果不想让别人轻易看到源码，可以：
- 先临时公开发布
- 或后面换 Vercel / Netlify / Cloudflare Pages

### 3. 不要上传本机绝对路径资源
当前项目已经改成项目内相对路径，可直接用于 GitHub Pages。

## 六、推荐仓库名

你可以用这些名字：

- `love-letter-mobile`
- `for-tanghuihui`
- `private-love-letter`
- `our-love-game`

如果你想更低调一点，建议：

- `our-little-page`
- `memo-page`
- `summer-note`
