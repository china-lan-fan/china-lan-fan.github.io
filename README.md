# fan-doc

中文脚本语言 [fan](https://github.com/china-lan-fan/fan) 的官方文档，使用 [VitePress](https://vitepress.dev/)（Vue 3）构建，部署在 GitHub Pages。

在线阅读：<https://china-lan-fan.github.io/fan-doc/>

## 本地开发

需要 Node.js 20+ 与 pnpm 10+。

```bash
pnpm install
pnpm dev
```

## 构建

```bash
pnpm build
pnpm preview
```

推送到 `main` 分支后，GitHub Actions 会自动构建并部署到 GitHub Pages（见 `.github/workflows/deploy.yml`）。

## 目录

```text
docs/
├── index.md          # 首页
├── guide/            # 语言指南
├── examples/         # 示例
└── reference/        # 语法速查 / 关键字 / 内建函数
```
