# 体重追踪 Weight Tracker

一个简洁优雅的体重记录应用，支持 **Android** 和 **Windows 11** 跨平台运行。

## 功能特性

- ✅ 每日体重记录
- ✅ 趋势曲线图可视化
- ✅ 7天/30天/全部数据视图切换
- ✅ 目标体重设置（双击目标卡片）
- ✅ 历史记录管理（支持删除）
- ✅ 数据本地存储（localStorage）
- ✅ PWA 支持（可安装到主屏幕）
- ✅ 响应式设计（手机/平板/桌面）
- ✅ 离线可用

## 使用方法

### Windows 11

1. **直接打开**
   - 双击 `index.html` 用浏览器打开
   - 或用 VS Code Live Server 插件运行

2. **安装为应用（推荐）**
   - 在 Edge 或 Chrome 中打开 `index.html`
   - 点击地址栏右侧的"安装"图标
   - 或点击页面底部的"安装"横幅

### Android

**方法一：通过网页访问**
1. 将应用部署到任意 Web 服务器（或用手机浏览器访问电脑上的文件）
2. 在 Chrome 中打开页面
3. 点击菜单 → "添加到主屏幕"

**方法二：本地运行**
1. 在电脑上启动本地服务器：
   ```bash
   # 使用 Python
   python -m http.server 8080
   
   # 或使用 Node.js
   npx serve .
   ```
2. 确保手机和电脑在同一局域网
3. 在手机浏览器访问 `http://电脑IP:8080`
4. 添加到主屏幕

**方法三：使用 Termux（离线）**
1. 在 Android 安装 Termux
2. 在 Termux 中安装 Node.js：`pkg install nodejs`
3. 复制应用文件到手机
4. 运行：`npx serve .`
5. 浏览器访问并安装

## 文件说明

```
weight-tracker/
├── index.html      # 主应用文件（单文件应用）
├── manifest.json   # PWA 配置
├── sw.js           # Service Worker（离线支持）
└── README.md       # 说明文档
```

## 技术栈

- **前端**: 纯 HTML/CSS/JavaScript（无框架依赖）
- **图表**: Canvas 2D 原生绘制
- **存储**: localStorage
- **PWA**: Web App Manifest + Service Worker
- **设计**: 自定义暗色主题，渐变配色

## 目标体重设置

双击"目标"卡片即可修改目标体重。

## 数据备份

数据存储在浏览器的 localStorage 中。如需备份：
1. 打开浏览器开发者工具（F12）
2. Application → Local Storage → 找到对应域名
3. 复制 `weight_tracker_data` 的值

## 自定义

如需修改配色，编辑 `index.html` 中的 CSS 变量：
```css
:root {
    --accent: #00d9ff;      /* 主色调 */
    --success: #00ff88;     /* 下降颜色 */
    --danger: #ff4466;      /* 上升颜色 */
    --bg-primary: #0f0f1a;  /* 背景色 */
}
```

## License

MIT