# Historycat 霓虹点唱机

复古未来主义(Retro-Futurism)风格的单文件音乐电台。纯静态 HTML + JS,无任何依赖。

- 曲目存放于 Cloudflare R2 桶 `historycat-music`(公共域名 `https://pub-026f390d9c0e47ab9667d692eab108d9.r2.dev`)
- 播放直链使用 R2 上的**原文件名**(含日期与 `(1)` 后缀,经 `encodeURIComponent` 编码);界面展示名已去掉日期前缀
- 功能:播放/暂停、上一首/下一首、进度拖动、音量、随机播放、单曲循环、空格键快捷播放
- 字体:Orbitron + JetBrains Mono(Google Fonts,需联网)

## 本地打开

直接双击 `index.html`,或经任意静态服务器托管。

## 部署

推送到 GitHub 后开启 **Settings → Pages → Deploy from a branch (main, root)** 即可上线。
