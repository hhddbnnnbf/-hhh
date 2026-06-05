# 图片格式转换 PWA

本地图片格式互转工具，支持 JPG / PNG / WebP，可安装到手机主屏幕。

## 文件结构

```
image-converter/
├── index.html      # 主页面
├── manifest.json   # PWA 配置
├── sw.js           # Service Worker（离线缓存）
├── icons/
│   ├── icon-192.png
│   └── icon-512.png
└── README.md
```

## 部署到 Vercel（免费，推荐）

1. 注册 https://vercel.com（用 GitHub 账号登录最方便）
2. 点击 "Add New Project" → "Browse" 上传整个文件夹
   - 或者把文件夹拖拽到 Vercel 页面
3. 点击 Deploy，等几秒钟
4. 得到一个 https://xxx.vercel.app 的链接

## 安装到 iPhone 主屏幕

1. 用 Safari 打开你的 Vercel 链接
2. 点击底部分享按钮（方框+箭头图标）
3. 选择「添加到主屏幕」
4. 点击「添加」完成

之后就可以像普通 App 一样从主屏幕打开，全屏显示，离线也能用。

## 功能

- 支持格式：JPG、PNG、WebP、BMP、GIF → JPG / PNG / WebP
- 可调节输出质量（10%~100%）
- 批量处理多张图片
- 全程本地处理，图片不上传服务器
- 离线可用（Service Worker 缓存）
