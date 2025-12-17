# 中北大学 AI+移动互联创新实验室官网

<p align="center">
  <img src="public/medias/logo.png" alt="Ailab Logo" width="120">
</p>

<p align="center">
  <strong>NUC AI+Mobile Internet Innovation Laboratory</strong>
</p>

<p align="center">
  <a href="https://hexo.io"><img src="https://img.shields.io/badge/Hexo-8.0.0-blue?logo=hexo" alt="Hexo"></a>
  <a href="https://github.com/blinkfox/hexo-theme-matery"><img src="https://img.shields.io/badge/Theme-Matery-green" alt="Theme"></a>
  <a href="https://nodejs.org"><img src="https://img.shields.io/badge/Node.js-18+-339933?logo=node.js" alt="Node.js"></a>
</p>

## 📖 简介

本项目是**中北大学 AI+移动互联创新实验室**的官方网站源码，采用 [Hexo](https://hexo.io/) 静态博客框架构建，使用 [hexo-theme-matery](https://github.com/blinkfox/hexo-theme-matery) 主题。

### 🌟 网站功能

| 模块 | 说明 |
|------|------|
| 🏠 首页 | 实验室介绍、公告动态 |
| 👨‍🏫 导师团队 | 实验室导师信息展示 |
| 🏆 竞赛成果 | 学生竞赛获奖记录 |
| 📝 招生信息 | 实验室招生相关通知 |
| 🎓 校友风采 | 优秀校友展示 |
| 📚 学习生活 | 实验室日常学习记录 |
| 🤝 团队建设 | 团建活动展示 |

## 🚀 快速开始

### 环境要求

- [Node.js](https://nodejs.org/) >= 18.x
- [Git](https://git-scm.com/)

### 安装步骤

1. **克隆仓库**

```bash
git clone https://github.com/WangDollar/nuc-ailab.git
cd nuc-ailab
```

2. **安装依赖**

```bash
npm install
```

3. **本地预览**

```bash
npm run server
```

访问 http://localhost:4000 查看网站

4. **生成静态文件**

```bash
npm run build
```

生成的静态文件位于 `public/` 目录

5. **清理缓存**

```bash
npm run clean
```

### 部署

```bash
npm run deploy
```

## 📁 项目结构

```
nuc-ailab/
├── _config.yml          # Hexo 主配置文件
├── package.json         # 项目依赖
├── scaffolds/           # 文章模板
├── source/              # 网站源文件
│   ├── _data/           # 数据文件 (导师、校友、竞赛等)
│   ├── _posts/          # 博客文章
│   ├── admissions/      # 招生页面
│   ├── alumni/          # 校友页面
│   ├── competition-results/  # 竞赛成果页面
│   ├── study-life/      # 学习生活页面
│   ├── supervisor-team/ # 导师团队页面
│   └── team-building/   # 团队建设页面
└── themes/
    └── hexo-theme-matery/  # 主题文件
```

## ✏️ 内容编辑

### 添加/修改导师信息

编辑 `source/_data/teachers.yml`：

```yaml
- name: 导师姓名
  profile_url: "https://导师主页链接"
  image_path: "/medias/teachers/导师照片.jpg"
```

### 添加/修改竞赛成果

编辑 `source/_data/competition_results.yml`

### 添加/修改校友信息

编辑 `source/_data/alumni.yml`

### 发布新文章

```bash
npx hexo new "文章标题"
```

然后编辑 `source/_posts/文章标题.md`

## ⚙️ 配置说明

### 主配置文件 (`_config.yml`)

- `title`: 网站标题
- `subtitle`: 网站副标题
- `author`: 作者
- `language`: 语言设置 (默认 `zh-CN`)

### 主题配置 (`themes/hexo-theme-matery/_config.yml`)

- `menu`: 导航菜单配置
- `socialLink`: 社交链接配置
- `music`: 音乐播放器配置
- 更多配置请参考主题文档

## 🔗 相关链接

- [Hexo 官方文档](https://hexo.io/zh-cn/docs/)
- [hexo-theme-matery 主题](https://github.com/blinkfox/hexo-theme-matery)
- [中北大学计算机科学与技术学院](https://cst.nuc.edu.cn/)

