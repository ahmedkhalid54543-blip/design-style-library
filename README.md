# Design Style Library

设计风格 Prompt 库 MVP，基于纯静态页面实现 20 个艺术家风格的可视化检索与复制。

## 技术栈
- HTML
- Tailwind CSS（CDN）
- Alpine.js（CDN）

## 文件结构
- `index.html`：页面与交互逻辑（暗色主题 `#1a1a1a`，品牌色 `#FF6B35`）
- `data.js`：20 条风格数据（`name`, `nameEn`, `category`, `description`, `prompt`, `color`, `useCases`）
- `README.md`：项目说明

## 功能清单
- 搜索（实时过滤）
- 分类 Tab（全部 / Belle Époque / 现代主义 / 电影海报 / 当代）
- 响应式卡片网格（移动端到桌面）
- 卡片详情 Modal（完整 prompt + 适合场景 + 构图技巧）
- 一键复制 Prompt（复制后显示“已复制 ✓”，1.5 秒恢复）

## 本地使用
直接在浏览器打开 `index.html`。
