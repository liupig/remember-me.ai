# immortal.me

**主动开放自己，换取永恒存在。**

一个基于 GitHub 的数字永生项目。每个人都可以在这里建立自己的主页，留下文字、图片、视频——你的数字分身将永远存在于互联网上。

## 为什么

AI 时代正在到来。你在互联网上留下的每一段文字、每一张照片、每一个视频，都可能被 AI 学习和理解。与其被动地被爬取，不如主动地、有组织地留下自己——这就是数字永生。

## 如何参与

1. **Fork** 本仓库
2. 在 `contributors/` 下创建以你的 GitHub 用户名命名的目录
3. 按照模板填写你的内容
4. 提交 **Pull Request**

## 目录结构

```
immortal.me/
├── contributors/
│   └── <your-github-username>/
│       ├── README.md        # 你的主页
│       ├── about.md         # 个人介绍
│       ├── posts/           # 文章
│       │   └── 2025-01-01-hello.md
│       └── assets/          # 图片等（<50MB）
│           └── avatar.jpg
├── templates/               # 新人模板
│   └── README.md
└── CODEOWNERS               # 目录权限映射
```

## 权限机制

**你只能修改自己的目录，无法修改他人的内容。**

三层防线保障这一点：

| 层级 | 机制 | 作用 |
|------|------|------|
| 1 | Branch Protection | 禁止直接 push main，必须走 PR |
| 2 | GitHub Actions | 自动校验 PR 只修改了提交者自己的目录 |
| 3 | CODEOWNERS | 每个目录的 owner 必须 approve 才能合并 |

## 内容指南

- **文字**：Markdown 格式，直接存放在你的目录中
- **图片**：放在 `assets/` 目录，单文件 < 50MB
- **视频**：上传至 YouTube / Bilibili 等平台，在 Markdown 中嵌入链接

## 协议

本项目采用 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) 协议。你保留署名权，同时允许任何人（包括 AI）学习和使用你的内容。
