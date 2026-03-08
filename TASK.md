# Design Style Library - 设计风格 Prompt 仓库

## 目标
做一个静态网页，让用户可视化浏览 20 个设计艺术家风格，并一键复制对应的 Lovart prompt。

## 技术栈
- 纯 HTML + Tailwind CSS (CDN) + Alpine.js (CDN)
- 数据放在 data.js 里（JSON 数组）
- 部署到 GitHub Pages

## 页面结构

### Header
- 标题：「设计风格 Prompt 库」
- 副标题：「20位传奇设计师 × Lovart 4K 生成」
- 搜索框（实时过滤）
- 分类筛选 Tab：全部 / Belle Époque / 现代主义 / 电影海报 / 当代

### 主体 Grid（响应式 3-4列）
每个风格卡片包含：
- 顶部色块（用该风格的代表色渐变，暂无图片）
- 艺术家名字（中英双语）
- 时代标签（Belle Époque / 现代主义 / 电影海报 / 当代）
- 2-3句风格描述
- Prompt 代码块（灰色背景）
- 「复制 Prompt」按钮（点击后变「已复制 ✓」，1.5秒后恢复）

### 风格卡片详情页（点击卡片展开 Modal）
- 更大的色块/占位图区域
- 完整 prompt（含 Lovart 4K 模板）
- 「适合场景」标签（海报/封面/插画等）
- 构图技巧说明

## 数据（data.js）

20个风格，按4个分类：

### Belle Époque（5个）
1. Jules Chéret - `Jules Cheret style, bright joyful colors, dynamic feminine figures, Art Nouveau poster`
2. Toulouse-Lautrec - `Toulouse-Lautrec style, flat color blocks, Japanese influence, bold silhouettes`
3. Alphonse Mucha - `Alphonse Mucha style, Art Nouveau flowing curves, ornate floral borders, decorative panels`
4. Théophile Steinlen - `Steinlen style, social realist, expressive lines, muted earthy tones`
5. Eugène Grasset - `Eugène Grasset style, Medieval Gothic aesthetic, stained glass colors, ornate lettering`

### 现代主义（5个）
6. Saul Bass - `Saul Bass style, minimalist geometric abstraction, visual metaphor, flat shapes, bold typography`
7. Cassandre - `Cassandre style, Cubist planes, dramatic perspective, Art Deco, streamlined forms`
8. Milton Glaser - `Milton Glaser style, psychedelic pop art, innovative typography, vibrant colors`
9. Josef Müller-Brockmann - `Müller-Brockmann style, Swiss grid system, mathematical precision, clean sans-serif`
10. Paul Rand - `Paul Rand style, playful geometry, clever visual puns, primary colors, simple shapes`

### 电影海报（5个）
11. Drew Struzan - `Drew Struzan style, painted realism, epic cinematic composition, nostalgic warm glow`
12. Olly Moss - `Olly Moss style, ultra-minimal, clever negative space, hidden dual imagery, 1-2 colors`
13. Tyler Stout - `Tyler Stout style, maximalist character collage, intricate details, dense composition`
14. Martin Ansin - `Martin Ansin style, Art Deco elegance, refined vintage, muted sophisticated tones`
15. Laurent Durieux - `Laurent Durieux style, visual puns, mysterious atmospheric, dreamlike surrealism`

### 当代（6个）
16. Kilian Eng - `Kilian Eng style, geometric futurism, precise technical lines, retro sci-fi`
17. Dan McCarthy - `Dan McCarthy style, ultra-flat geometric abstraction, bold graphic shapes`
18. Jock - `Jock style, gritty expressive brushwork, dynamic action, raw energy`
19. Shepard Fairey - `Shepard Fairey style, propaganda poster aesthetic, halftone dots, high contrast`
20. Jay Ryan - `Jay Ryan style, folksy handmade aesthetic, warm textured, organic simple forms`
21. Paula Scher - `Paula Scher style, typographic maximalism, layered text as image, bold sans-serif`

## 设计风格要求（重要！用 impeccable-design 原则）
- 暗色主题（深灰背景 #1a1a1a，卡片 #242424）
- 品牌色：橙色 #FF6B35
- 字体：Noto Sans SC（中文），JetBrains Mono（代码块）
- 卡片圆角 10px，hover 轻微上浮
- 搜索框和筛选 Tab 要好看
- 整体有设计感，不像普通工具页

## 文件结构
```
design-style-library/
├── index.html
├── data.js
└── README.md
```

## 部署
- GitHub repo: ahmedkhalid54543-blip/design-style-library
- GitHub Pages 自动部署

## 完成标准
1. 本地打开 index.html 正常显示所有 20 个风格卡片
2. 搜索和分类筛选正常工作
3. 复制按钮功能正常
4. Modal 展开显示完整信息
5. 响应式布局（手机/平板/电脑）
6. 推送到 GitHub，Pages 可访问

