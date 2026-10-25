# AURA · 3D 光影计算器

一台放在浏览器里的实体质感桌面计算器。使用 Three.js / WebGL2 实时渲染，按键、屏幕、材质与光影都不是图片贴图。

**[在线体验 →](https://kiriusss.github.io/aura-3d-calculator/)**

[![AURA 3D 计算器预览](preview.png)](https://kiriusss.github.io/aura-3d-calculator/)

## 特性

- **实体建模**：圆角金属机身、哑光面板、象牙白键帽、琥珀色功能键与铜色细节。
- **真实光影**：HDR 工作室环境、PBR 材质、ACES 色调映射、软阴影、接触阴影、泛光与实时屏幕自发光。
- **可触摸的按键**：20 个独立 3D 键帽，支持悬停微亮、按下回弹、程序化机械按键音，以及设备支持时的触感反馈。
- **完整计算能力**：四则运算、小数、百分比、正负号、退格、清零、连续运算与除零错误处理。
- **键盘可用**：数字、`+ - * /`、`Enter`、`Esc`、`Backspace`、`%`。
- **响应式**：桌面 / 平板 / 手机分别适配相机取景。
- **单文件部署**：整个应用（Three.js 运行时、样式与逻辑）都在 `index.html` 内，无后端、无第三方网络请求，可离线打开。

## 操作

| 操作 | 方式 |
| --- | --- |
| 旋转视角 | 鼠标或单指拖动 |
| 缩放 | 滚轮或双指捏合 |
| 按键 | 点击 3D 键帽，或使用键盘 |
| 重置视角 | 右上角「重置视角」 |
| 开关音效 | 右上角「声音」 |

## 技术栈

- Three.js r186
- WebGL2、PBR、PMREM、ACES Filmic Tone Mapping
- UnrealBloom 后处理、PCF 阴影、程序化接触阴影
- CanvasTexture 实时数字屏幕
- esbuild 打包为单文件 HTML
- 原生 HTML / CSS / JavaScript，无框架

## 本地运行

直接双击 `index.html` 即可，也可以：

```bash
python3 -m http.server 8000
# 打开 http://localhost:8000
```

需要支持 WebGL2 的现代浏览器（Chrome / Edge / Safari / Firefox）。

---

Designed and built with a focus on material, light and touch.
