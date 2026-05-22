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
Stage 4 必须执行 L1-L6 检查（含成稿前自检）。

## v1.2 关键变更
- 开头规范：条件 A「四步开头」（生活冲动→情绪误读→核心反转→原作者原话定锚）优先；条件 B「生活切片型三行开头」作为备选；禁止为满足生活切片型而编造第一手经历
- 正文结构：核心反转(20-25%) → 实操建议(50-60%) → 行动收束(15-20%)
- 方法段合格标准：每条建议必须含动作+解释+案例，素材来自原文，不许编造
- 小标题规则：优先判断型/反常识型/压缩型强观点，8-18字，避免功能说明型
- 机制筛选规则：不能服务主线的机制优先压缩或删除
- 字数控制：默认2200-3000字，上限3200，超3000字执行5项压缩动作
- 禁止三段式议论文（提出观点→展开论证→总结升华）
- Stage 4 新增 L6 成稿前自检（8 项结构性检查）

## 确认加载
加载完成后，回复用户：

```
entropy-writer v1.2 已就绪。
请把翻译稿或素材发给我。
我会先跑 Stage 1 领航员定位，确认方向后再进入成文阶段。
```
