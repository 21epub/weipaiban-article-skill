# 复古报刊 · 双栏线

上下各一条细墨线，印泥红只在版首日期出现一次。建议语法：章节流、对照流。

## Token

```
主色 primary     #2A2622
辅色 accent      #9C3B32
正文 text        #3F3A36
次要 muted       #7A736C
线   line        #2A2622
浅底 wash        #E7E2D8
作品底 canvas    #F3F0E8
```

主色是报纸墨色（标题、双线）。辅色印泥红只用于版首日期，二级标题和卡片不再用它。正文 `#3F3A36`。作品底是旧报纸色 `#F3F0E8`，不要 `#FFFFFF`，也不要 `#000000`。不要 `font-family`。栏线用边框，不要分栏 float。

## 形态（一篇一套）

- **标题**：左对齐、字重 800。主标题 28–32px、行高 1.2；二级 18–20px。日期用 11px、字距 1.5px。
- **分割**：上下各 1px 实线的双线，中间留 4px。不要色条，不要虚线。
- **卡片**：圆角 0，背景 `#E7E2D8`，无描边，无阴影。顶部一条 1px 墨线。
- **图注**：左齐，次要色，可加「图 / 」前缀，前缀用主色。

## 写法参考

版首（日期只用一次印泥红）：

```html
<section style="padding:22px 14px 16px;background:#F3F0E8;border-top:1px solid #2A2622;border-bottom:1px solid #2A2622;">
  <span style="display:inline-block;font-size:11px;letter-spacing:1.5px;color:#9C3B32;font-weight:700;">2026.11.20</span>
  <p style="margin:10px 0 0;font-size:30px;font-weight:800;color:#2A2622;letter-spacing:0.5px;line-height:1.2;">主标题六到十字</p>
</section>
```

二级标题（双线，不再用红）：

```html
<section style="margin:28px 10px 14px;padding:8px 0;border-top:1px solid #2A2622;border-bottom:1px solid #2A2622;">
  <p style="margin:0;font-size:18px;font-weight:800;color:#2A2622;line-height:1.35;">小标题</p>
</section>
```

卡片小结：

```html
<section style="margin:14px 10px 0;padding:16px 0 0;background:#F3F0E8;border-top:1px solid #2A2622;border-radius:0;">
  <p style="margin:0;padding:14px;background:#E7E2D8;font-size:16px;line-height:1.8;color:#3F3A36;">一句话带走。</p>
</section>
```

## 适配场景

时评、本地新闻、事件复盘、剪报式资料、需要日期感的报道。杂志长文和金线大字用 `editorial-serif`。硬切割年报用 `swiss-minimal`。

## 挑图气质

- styleAnchor：旧报纸双线栏，墨色标题，版首一处印泥红日期，资料感
- lightingHint：均匀平光，纸色偏暖，几乎无阴影
