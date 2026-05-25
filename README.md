# entropy-writer
**熵减笔记本小红书长图文写作引擎 · v1.5**

## 这个 Skill 是什么
为小红书账号「熵减笔记本」量身设计的内容写作引擎。

输入：英文翻译稿、文章链接、外部素材、散乱想法
输出：接近终稿的小红书长图文，作者只需微调 10%-20%

## 核心口诀
**领航员定方向，卡兹克给骨头，熵减给皮肤和呼吸。**

## 执行流程
Stage 1 · 领航员定位 → Stage 2 · 卡兹克强化 → Stage 3 · 熵减成文 → Stage 4 · 终稿自检

## 文件结构
```
entropy-writer/
├── README.md
├── SKILL.md
├── CLAUDE.md
├── references/
│   ├── navigator-5-stations.md
│   ├── entropy-style-v1.md
│   ├── khazix-extracted.md
│   └── khazix-boundary.md
└── cases/
    └── case-001-front-1-percent/
        ├── translation.md
        ├── final.md
        └── notes.md
```

## 触发条件
以下任意一种都应触发本 Skill：
- 「帮我把这篇翻译稿写成熵减风格的文章」
- 「用熵减笔记本的风格写一篇」
- 「这篇英文内容帮我做成小红书长图文」
- 「跑一下写作引擎」

**不适用于：** 300 字以内短内容、单图文、朋友圈级别内容、纯标题生成

## 输出格式（三段式）
1. **领航员骨架确认**（Stage 1+2 产出，正文主控骨架，供作者确认方向）
2. **正文终稿**（Stage 3+4 产出，可直接发布）
3. **作者微调提示**（AI 不能替你补的细节清单）
