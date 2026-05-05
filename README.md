# 行业洞察资料库 (Industry Insights)

## 目录结构

```
industry-insights/
├── README.md           # 本文件
├── liquid-cooling/     # 液冷行业分析
│   ├── docs/           # 分析文档（.md）
│   ├── ppt/            # PPT文件（.pptx）
│   └── sources/        # 原始资料（PDF/网页/下载文件）
├── gpu-chips/          # GPU芯片行业分析
│   ├── docs/
│   ├── ppt/
│   └── sources/
├── OTT-cloud/          # OTT云厂商/IDC租赁分析
│   ├── docs/
│   ├── ppt/
│   └── sources/
└── articles/           # 微信公众号文章归档
    ├── liquid-cooling/
    ├── gpu-chips/
    └── OTT-cloud/
```

## 归档规则

### 文章归档流程
1. 收到微信公众号文章链接
2. 用 Chrome headless 转为 PDF（`google-chrome --headless --print-to-pdf=...`）
3. 按行业分类存到 `articles/<行业>/`
4. 对应的 source 目录也保存一份
5. Git push 同步到 GitHub

### 文件命名规范
- 文章PDF：`wechat-article-YYYY-MM-DD.pdf`
- PPT：`liquid-cooling-latest.pptx` 或 `liquid-cooling-YYYY-MM-DD.pptx`
- 文档：`YYYY-MM-DD-主题-name.md`

## 仓库信息
- GitHub: https://github.com/marshall9900/industry-insights
- 用途：保存所有行业分析资料，包括文档、PPT、原始来源、PDF归档