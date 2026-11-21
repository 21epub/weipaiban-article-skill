# 靛蓝布标 · 明线

窄靛蓝边和虚线针脚，褐线只作小标。建议语法：章节流、叙事流。

## Token

```
主色 primary     #283855
辅色 accent      #894F35
正文 text        #3A3E48
次要 muted       #7C756C
线   line        #C8C2B6
浅底 wash        #E6E8EF
作品底 canvas    #F4F2EC
```

主色是靛蓝（标题、布边、针脚），辅色是染褐，只用于小标签和针脚下划线。正文用暖灰蓝，不用纯黑。作品底是未漂白布色 `#F4F2EC`，不要 `#FFFFFF`。不要 `font-family`，不要 `transform`。针脚用虚线，不要斜贴。

## 形态（一篇一套）

- **标题**：左对齐。主标题 26–30px、字重 700；二级 18px。标题区底边是 `1px dashed #283855`。
- **分割**：同一条靛蓝虚线，全篇重复，不要实线色条。
- **卡片**：圆角 2px，背景 `#E6E8EF`，描边 `1px dashed #283855`。左侧 4px 实线靛蓝边，无阴影。
- **图注**：左齐，次要色小字。
- **下划线**：`border-bottom:1px dashed #894F35;font-weight:600;`。每段 1–3 个短短语。

## 写法参考

版首（布边 + 小标）：

```html
<section style="padding:28px 14px 20px;background:#F4F2EC;border-bottom:1px dashed #283855;">
  <span style="display:inline-block;padding:2px 8px;color:#894F35;font-size:11px;letter-spacing:2px;border-bottom:1px dashed #894F35;">蓝染</span>
  <p style="margin:14px 0 0;font-size:28px;font-weight:700;color:#283855;letter-spacing:1px;line-height:1.35;">主标题四到八字</p>
</section>
```

二级标题（明线）：

```html
<section style="margin:28px 10px 14px;padding-bottom:10px;border-bottom:1px dashed #283855;">
  <p style="margin:0;font-size:18px;font-weight:700;color:#283855;line-height:1.4;">小标题</p>
</section>
```

卡片小结（布边）：

```html
<section style="margin:16px 10px 0;padding:18px 16px;background:#E6E8EF;border:1px dashed #283855;border-left:4px solid #283855;border-radius:2px;">
  <p style="margin:0;font-size:16px;line-height:1.9;color:#3A3E48;">一句话带走。</p>
</section>
```

## 适配场景

蓝染、草木染、布艺记录、工艺品牌、手作工坊。宣纸印章和器物国风用 `neo-chinese`。胶带拼贴用 `collage-journal`。

## 挑图气质

- styleAnchor：未漂白布面上的靛蓝明线，褐线小标，针脚虚线，边角方正
- lightingHint：平铺顶光，布纹可见，无强投影
