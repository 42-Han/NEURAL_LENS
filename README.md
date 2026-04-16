# Neural Lens Recon

一个基于 AI 深度估计和 Three.js 的 3D 点云渲染项目，将普通图片转换为具有科技感的 3D 字符云效果。

## ✨ 功能特点

- 🤖 **AI 深度估计** - 使用 Hugging Face Transformers 进行实时深度估计，创建 3D 效果
- 🎨 **3D 字符云** - 将图像转换为由字符组成的 3D 点云，支持自定义字符集
- �️ **轮廓检测** - 启用轮廓模式，突出图像的边缘特征
- 🎭 **科技感 UI** - 现代化的玻璃态界面，具有流畅的动画效果
- � **自定义颜色** - 支持自定义背景颜色和点/字符颜色
- 📱 **响应式设计** - 适配不同屏幕尺寸，提供良好的用户体验
- 💾 **多格式导出** - 支持导出为 PNG（透明背景）、JPEG、SVG、GIF 和视频格式
- ⚡ **实时渲染** - 使用 Three.js 实现流畅的 3D 交互和动画效果
- 🌐 **模型缓存** - 模型首次下载后会缓存到浏览器，后续无需重复下载

## 🚀 快速开始

### 方法一：本地运行

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

### 方法二：在线访问

- **main 分支**（原始版本）：
  - 访问 [GitHub Pages](https://42-Han.github.io/dianyu)

## 📖 使用说明

### 1. 上传图片
- 点击 "INITIALIZE SCANNER" 按钮选择本地图片
- 或点击侧边栏的 "RE-UPLOAD SOURCE" 按钮重新上传图片

### 2. 核心功能

#### 3D 深度模式
- 勾选 "ENABLE 3D DEPTH" 启用 3D 深度效果
- 使用 "Z-Intensity" 滑块调整深度效果强度
- 首次启用时会下载 AI 深度估计模型（约 100MB）
- 模型会缓存到浏览器，后续使用无需重新下载

#### 轮廓模式
- 勾选 "ENABLE CONTOUR" 启用轮廓检测
- 选择点/字符颜色，突出图像的边缘特征

### 3. 参数调整

- **Stride** - 调整点云的密度（值越小密度越高）
- **Diffuse** - 调整点云的扩散程度
- **Flicker** - 调整点云的闪烁动画速度
- **Point Size** - 调整点/字符的大小

### 4. 自定义字符
- 在 "Custom Chars" 输入框中输入自定义字符（最多 10 个）
- 点击 "UPDATE CHARS" 更新字符集
- 支持选择不同的字符模式：Random、Custom、None

### 5. 导出功能
- 点击 "EXPORT" 按钮打开导出面板
- 输入文件名
- 选择导出格式：
  - **PNG** - 透明背景
  - **JPG** - 包含背景颜色
  - **SVG** - 矢量格式
  - **GIF** - 3 秒动画
  - **VIDEO** - 录制视频

## 🛠️ 技术栈

| 技术 | 版本 | 用途 |
|------|------|------|
| Three.js | 0.160.0 | 3D 渲染引擎 |
| Transformers.js | 3.0.0 | AI 深度估计 |
| JavaScript | ES6+ | 核心逻辑 |
| HTML5/CSS3 | - | 界面布局和样式 |
| GIF.js | 0.2.0 | GIF 动画生成 |
| MediaRecorder API | - | 视频录制 |

## 📁 项目结构

```
dianyu/
├── index.html          # 主页面（包含所有代码）
└── README.md           # 项目说明
```

## 🎯 分支管理

- **main** - 定版版本，使用原始 Hugging Face 源
- **mirror** - 镜像版本，支持国内访问（自动检测镜像源）

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