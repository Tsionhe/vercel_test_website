# Vercel Test Website

这是一个用于演示 GitHub 与 Vercel 自动化部署流程的静态网页项目。页面内容集中在 `index.html` 中，适合用于测试零配置部署、预览发布效果，以及验证 GitHub 仓库与 Vercel 项目的连接流程。

## 项目结构

```text
.
├── AGENTS.md    # AI 编码代理协作说明
├── README.md    # 项目说明文档
└── index.html   # 静态页面入口
```

## 本地预览

可以直接用浏览器打开 `index.html` 查看页面。

如需通过本地服务预览，可在项目根目录运行：

```powershell
python -m http.server 3000
```

然后访问：

```text
http://localhost:3000
```

## 部署说明

该项目是纯静态页面，不需要安装依赖或运行构建命令。部署到 Vercel 时通常可以保持默认配置：

- Framework Preset: `Other`
- Build Command: 留空
- Output Directory: 留空或使用默认值
- Install Command: 留空

将仓库推送到 GitHub 后，在 Vercel 中导入该仓库即可自动生成部署。后续提交到关联分支时，Vercel 会自动触发新的部署。

## 修改建议

- 页面内容和样式主要在 `index.html` 中维护。
- 保存中文内容时使用 UTF-8 编码。
- 修改后建议同时检查桌面和移动端显示效果，避免文本溢出或布局重叠。
