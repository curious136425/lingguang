灵光 PWA — 安装说明
================================

📦 部署方式（三选一）：

1. 【最简单】上传到任何静态服务器
   把整个文件夹上传到你的服务器（如 GitHub Pages、Vercel、Netlify）
   访问 /lingguang.html 即可

2. 【本地测试】
   cd lingguang-pwa
   python3 -m http.server 8000
   然后手机和电脑在同一WiFi下，用手机访问 http://电脑IP:8000/lingguang.html

3. 【GitHub Pages 一键部署】
   git init && git add . && git commit -m "灵光PWA"
   git push origin main
   在 Settings > Pages 中启用

📱 安装到手机：
   iPhone: Safari打开 → 分享 → 添加到主屏幕
   Android: Chrome打开 → 菜单 → 安装应用

📂 文件说明：
   lingguang.html         主App（仿真书翻页 + 记录 + 导出）
   lingguang-widget.html  桌面卡片（今日灵感摘要）
   manifest.json          PWA配置
   sw.js                  Service Worker（离线缓存）
   icon-192.png           应用图标
   icon-512.png           应用图标

🔧 数据存储：
   所有记录保存在手机浏览器本地，不经过任何服务器
   切换设备需要导出JSON备份再导入
