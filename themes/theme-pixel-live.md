# 像素现场 · 阶梯页签

浅纸底上的直角色块和阶梯标记，一块暖金就够。建议语法：卡片流、章节流。

## Token

```
主色 primary     #5937B4
辅色 accent      #C4923A
正文 text        #3F3A48
次要 muted       #7A7388
线   line        #D9D0EA
浅底 wash        #EFEAF8
作品底 canvas    #F6F4FA
```

主色是像素紫（标题、阶梯、描边），辅色暖金只做阶梯里的一格或一处页签。正文用暖灰紫，不用纯黑。作品底是浅紫纸 `#F6F4FA`，不要 `#FFFFFF`。不要 `font-family`，不要 `transform`。圆角一律 0。

## 形态（一篇一套）

- **标题**：左对齐、字距 1px。主标题 24–28px、字重 700；二级 18px。标题上方一排高低不等的直角色块，其中只有一格用辅色。
- **分割**：8px 高的主色短条，左齐，不要通栏细线。
- **卡片**：圆角 0，背景 `#EFEAF8`，描边 `2px solid #5937B4`，无阴影。
- **图注**：左齐，次要色小字。
- **下划线**：`border-bottom:2px solid #C4923A;font-weight:700;`。每段 1–3 个短短语。

## 写法参考

版首（阶梯色块）：

```html
<section style="padding:24px 14px 18px;background:#F6F4FA;">
  <span style="display:inline-block;width:10px;height:6px;background:#5937B4;"></span>
  <span style="display:inline-block;width:10px;height:10px;margin-left:3px;background:#5937B4;"></span>
  <span style="display:inline-block;width:10px;height:14px;margin-left:3px;background:#5937B4;"></span>
  <span style="display:inline-block;width:10px;height:8px;margin-left:3px;background:#C4923A;"></span>
  <p style="margin:14px 0 0;font-size:26px;font-weight:700;color:#3F3A48;letter-spacing:1px;line-height:1.3;">主标题四到八字</p>
</section>
```

二级标题（短页签）：

```html
<section style="margin:24px 10px 12px;">
  <span style="display:inline-block;padding:3px 8px;background:#5937B4;color:#F6F4FA;font-size:11px;font-weight:700;letter-spacing:1px;">02</span>
  <p style="margin:8px 0 0;font-size:18px;font-weight:700;color:#3F3A48;line-height:1.4;">小标题</p>
  <span style="display:inline-block;width:36px;height:8px;margin-top:8px;background:#5937B4;"></span>
</section>
```

卡片小结：

```html
<section style="margin:12px 10px 0;padding:16px;background:#EFEAF8;border:2px solid #5937B4;border-radius:0;">
  <p style="margin:0;font-size:16px;line-height:1.75;color:#3F3A48;">一句话带走。</p>
</section>
```

## 适配场景

像素界面、点阵教程、独立开发笔记、复古主机制作、8-bit 视觉说明。电竞和深底荧光长文用 `cyber-dark`。不要把本主题写成霓虹暗底。

## 挑图气质

- styleAnchor：浅紫纸上的直角像素块，一格暖金，阶梯页签，界面清晰
- lightingHint：平光，无投影，色块边缘利落
