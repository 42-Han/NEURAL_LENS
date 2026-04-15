# Neural Lens Recon

一个基于 AI 深度估计和 Three.js 的 3D 点云渲染项目，将普通图片转换为具有科技感的 3D 字符云效果。

## ✨ 功能特点

- 🤖 **AI 深度估计** - 使用 Hugging Face Transformers 进行实时深度估计
- 🎨 **3D 字符云** - 将图像转换为由字符组成的 3D 点云
- 📱 **响应式设计** - 适配不同屏幕尺寸
- 🌐 **国内镜像支持** - 自动检测可用的模型源，无需 VPN
- 💾 **导出功能** - 支持导出为 PNG、JPEG 和 GIF 格式
- ⚡ **实时渲染** - 使用 Three.js 实现流畅的 3D 交互

## 🚀 快速开始

### 方法一：直接访问

1. **main 分支**（原始版本）：
   - 访问 [GitHub Pages](https://42-Han.github.io/dianyu)

2. **mirror 分支**（国内镜像版本）：
   - 访问 [Mirror 版本](https://42-Han.github.io/dianyu/mirror)

### 方法二：本地运行

1. **克隆项目**
   ```bash
   git clone https://github.com/42-Han/dianyu.git
   cd dianyu
   ```

2. **启动本地服务器**
   ```bash
   # 使用 Python
   python3 -m http.server 8080
   
   # 或使用 Node.js
   npx http-server -p 8080
   ```

3. **访问项目**
   - 打开浏览器，访问 `http://localhost:8080`

## 📖 使用说明

### 1. 上传图片
- 点击 "UPLOAD IMAGE" 按钮选择本地图片
- 或直接拖放图片到上传区域

### 2. 调整参数
- **Scale** - 调整点云的整体大小
- **Density** - 调整字符的密度
- **Speed** - 调整动画速度
- **Depth** - 调整深度效果强度
- **Font Size** - 调整字符大小

### 3. 自定义字符
- 在输入框中输入自定义字符（最多 10 个）
- 点击 "UPDATE CHARS" 更新字符集

### 4. 导出结果
- 点击 "EXPORT" 按钮打开导出面板
- 选择导出格式（PNG、JPEG、GIF）
- 输入文件名，点击对应格式按钮导出

## 🛠️ 技术栈

| 技术 | 版本 | 用途 |
|------|------|------|
| Three.js | 0.160.0 | 3D 渲染引擎 |
| Transformers.js | 3.0.0 | AI 深度估计 |
| JavaScript | ES6+ | 核心逻辑 |
| HTML5/CSS3 | - | 界面布局 |
| GIF.js | 0.2.0 | GIF 动画生成 |

## 🌐 国内镜像配置

项目的 `mirror` 分支包含自动镜像检测功能：

1. **自动检测** - 按顺序尝试多个镜像源
2. **智能回退** - 当镜像不可用时自动回退到官方源
3. **无需配置** - 用户无需手动设置，系统会自动处理

## 📁 项目结构

```
dianyu/
├── index.html          # 主页面
├── index_副本.html     # 测试副本
└── README.md           # 项目说明
```

## 🎯 分支管理

- **main** - 定版版本，使用原始 Hugging Face 源
- **mirror** - 镜像版本，支持国内访问

## 🔧 开发指南

### 本地开发
1. 克隆项目到本地
2. 启动本地服务器
3. 修改代码并实时预览

### 部署
- **GitHub Pages** - 直接部署到 GitHub Pages
- **Vercel** - 使用 Vercel 快速部署
- **Netlify** - 支持自动部署

## 📄 许可证

MIT License

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

## 📞 联系

- GitHub: [42-Han](https://github.com/42-Han)

---

**Neural Lens Recon** - 用 AI 技术重新定义图像的视觉表现 🎭