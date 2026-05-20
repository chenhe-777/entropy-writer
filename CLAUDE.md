# entropy-writer · Agent 加载说明

## 这个 Skill 做什么
将外部素材（英文翻译稿、文章链接、任何外部内容）转化为
「熵减笔记本」风格的小红书长图文。

## 加载时必须做的事
1. 加载 SKILL.md 作为主执行规范
2. 加载 references/navigator-5-stations.md 作为 Stage 1 执行标准
3. 加载 references/entropy-style-v1.md 作为 Stage 3 和 Stage 4 的风格锚
4. 加载 references/khazix-extracted.md 作为 Stage 2 的素材池参考
5. 加载 references/khazix-boundary.md 确认卡兹克模块使用边界

## 优先级
```
用户本次明确要求
  > references/entropy-style-v1.md
  > references/navigator-5-stations.md
  > references/khazix-boundary.md
  > references/khazix-extracted.md
```
当资料有冲突时，以 entropy-style-v1.md 为准。

## 触发条件
用户说以下任何一种，都应该触发这个 Skill：
- 帮我把这篇翻译稿写成熵减风格的文章
- 用熵减笔记本的风格写一篇
- 这篇英文内容帮我做成小红书长图文
- 跑一下写作引擎
- 按熵减笔记本的方式处理这篇文章

## 不适用于
- 300 字以内的短内容
- 单图文或朋友圈级别的内容
- 纯标题生成
- 纯翻译任务

## 执行顺序
```
Stage 1 · 领航员定位
  → Stage 2 · 卡兹克强化
  → Stage 3 · 熵减成文
  → Stage 4 · 终稿自检
```
Stage 1 不可跳过。
Stage 2 只生成素材池，不得直接写最终正文。
Stage 3 必须以熵减风格为最终口吻。
Stage 4 必须执行 L1-L5 检查。

## 确认加载
加载完成后，回复用户：

```
entropy-writer v1.1 已就绪。
请把翻译稿或素材发给我。
我会先跑 Stage 1 领航员定位，确认方向后再进入成文阶段。
```
