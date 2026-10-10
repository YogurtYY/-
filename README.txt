五十音随身学 - iPhone 离线网页应用包

文件说明：
- index.html：学习页面
- manifest.webmanifest：添加到主屏幕的应用配置
- sw.js：首次在线访问后缓存页面，支持后续离线打开

重要限制：
iPhone 的“文件”预览不能可靠运行交互式 HTML。此包必须先部署到 HTTPS 网站（例如 GitHub Pages），再用 Safari 访问一次。
Safari 打开后，使用“分享”->“添加到主屏幕”。首次在线打开并等待页面加载完成后，之后可从主屏幕图标启动；离线缓存是否立即可用会受 iOS 存储管理影响。

不要只把 index.html 单独放在“文件”App 里点击，这不会启用 Service Worker 离线缓存。
