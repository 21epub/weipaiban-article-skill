# 浅蓝水彩 · 水色停顿

一条水色色条托住标题，正文行距偏宽。建议语法：叙事流、章节流。

## Token

```
主色 primary     #315E71
辅色 accent      #8C4E46
正文 text        #3E4A4E
次要 muted       #7A868A
线   line        #C5D3D6
浅底 wash        #E5EEF0
作品底 canvas    #F3F6F6
```

主色是浅青蓝（标题、色条），辅色赭石只用于短下划线和一处小标签。正文用青灰，不用纯黑。作品底是冷纸色 `#F3F6F6`，不要 `#FFFFFF`。不要 `font-family`，不要 `transform`。

## 形态（一篇一套）

- **标题**：左对齐、字重 500–700、字距 1px。主标题 26–30px；二级 18px。标题块底边一条 8px 主色色条。
- **分割**：同样是这条 8px 主色色条，不要细线，不要虚线。
- **卡片**：圆角 14px，背景 `#E5EEF0`，无描边，无阴影。
- **图注**：左齐，次要色小字。
- **下划线**：`border-bottom:2px solid #8C4E46;font-weight:600;`。每段 1–3 个短短语。

## 写法参考

版首（水色色条）：

```html
<section style="padding:32px 16px 20px;background:#F3F6F6;border-bottom:8px solid #315E71;">
  <span style="display:inline-block;font-size:11px;letter-spacing:2px;color:#8C4E46;">手记</span>
  <p style="margin:12px 0 0;font-size:28px;font-weight:500;color:#315E71;letter-spacing:1px;line-height:1.45;">主标题五到九字</p>
</section>
```

二级标题：

```html
<section style="margin:28px 10px 14px;padding-bottom:12px;border-bottom:8px solid #315E71;">
  <p style="margin:0;font-size:18px;font-weight:700;color:#315E71;line-height:1.4;">小标题</p>
</section>
```

卡片小结：

```html
<section style="margin:16px 10px 0;padding:20px 18px;background:#E5EEF0;border-radius:14px;">
  <p style="margin:0;font-size:16px;line-height:2;color:#3E4A4E;">一句话带走。</p>
</section>
```

## 适配场景

活动手记、轻教程、旅行随笔、需要停顿的生活长文。墨线留白和散文呼吸用 `zen-whitespace`。内刊温度用 `olive-journal`。

## 挑图气质

- styleAnchor：冷纸底上的浅青水彩色条，赭石短点，宽行距，柔和停顿
- lightingHint：窗边散射光，色彩含水，阴影很淡
