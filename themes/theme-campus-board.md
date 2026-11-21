# 青春校园 · 活页公告

虚线活页配黑板青编号，粉笔黄只在版首出现一次。建议语法：卡片流、章节流。

## Token

```
主色 primary     #1E5C56
辅色 accent      #D4B15A
正文 text        #3F3F3F
次要 muted       #7A7568
线   line        #C9C2B2
浅底 wash        #E7F0EE
作品底 canvas    #F7F4EA
```

主色是黑板青（编号、标题），辅色粉笔黄只用于版首的一枚编号块。正文 `#3F3F3F`。作品底是活页纸 `#F7F4EA`，不要 `#FFFFFF`。不要 `font-family`，不要 `transform`。不要硬阴影，以免和摸鱼票据撞形。

## 形态（一篇一套）

- **标题**：左对齐。主标题 24–28px、字重 700；二级 18px，左侧一块主色编号。版首另有一枚粉笔黄编号，全文不再重复。
- **分割**：`1px dashed #C9C2B2` 通栏虚线，像活页横线。不要实线，不要色条。
- **卡片**：圆角 4px，背景 `#E7F0EE`，描边 `1px dashed #1E5C56`，无阴影。
- **图注**：左齐，次要色小字。
- **下划线**：`border-bottom:2px solid #1E5C56;font-weight:600;`。每段 1–3 个短短语。下划线用主色。

## 写法参考

版首（公告条 + 一枚粉笔黄）：

```html
<section style="padding:22px 14px 18px;background:#F7F4EA;border-bottom:1px dashed #C9C2B2;">
  <span style="display:inline-block;padding:4px 8px;background:#1E5C56;color:#F7F4EA;font-size:11px;font-weight:700;letter-spacing:1px;">NOTICE</span>
  <span style="display:inline-block;margin-left:8px;padding:4px 8px;background:#D4B15A;color:#3F3F3F;font-size:11px;font-weight:700;">01</span>
  <p style="margin:14px 0 0;font-size:26px;font-weight:700;color:#1E5C56;line-height:1.35;">主标题五到九字</p>
</section>
```

二级标题（活页虚线 + 青编号）：

```html
<section style="margin:24px 10px 12px;padding-bottom:10px;border-bottom:1px dashed #C9C2B2;">
  <span style="display:inline-block;padding:3px 8px;background:#1E5C56;color:#F7F4EA;font-size:12px;font-weight:700;">02</span>
  <p style="margin:8px 0 0;font-size:18px;font-weight:700;color:#1E5C56;line-height:1.4;">小标题</p>
</section>
```

卡片小结：

```html
<section style="margin:14px 10px 0;padding:16px;background:#E7F0EE;border:1px dashed #1E5C56;border-radius:4px;">
  <p style="margin:0;font-size:16px;line-height:1.8;color:#3F3F3F;">一句话带走。</p>
</section>
```

## 适配场景

校园活动、社团公告、升学经验、学生成长记录。通用教育杂志用 `moyu-green`。门票硬卡和测评用 `moyu-ticket`。

## 挑图气质

- styleAnchor：活页纸虚线，黑板青编号，版首一枚粉笔黄，公告栏清楚
- lightingHint：教室顶光，纸面平整，颜色不发灰
