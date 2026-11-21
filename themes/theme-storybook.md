# 手绘绘本 · 挂旗

一排短色条当挂旗，木色只占其中一旗。建议语法：叙事流、卡片流。

## Token

```
主色 primary     #73343E
辅色 accent      #8A632C
正文 text        #3F3438
次要 muted       #8A7A74
线   line        #E4D2CC
浅底 wash        #F8EEEA
作品底 canvas    #FBF6F1
```

主色是酒红（标题、挂旗），辅色是木色，只在版首挂旗里出现一格。正文用暖褐灰，不用纯黑。作品底是绘本纸 `#FBF6F1`，不要 `#FFFFFF`。不要 `font-family`，不要 `transform`。挂旗是 `inline-block` 色条，不要旋转。

## 形态（一篇一套）

- **标题**：左对齐。主标题 26–30px、字重 700、字距 1px；二级 18px。版首挂旗三格，中间一格用辅色，两侧用主色。
- **分割**：左齐 28px 宽、8px 高的主色短条。不要虚线。
- **卡片**：圆角 8px，背景 `#F8EEEA`，无描边，无阴影。
- **图注**：左齐，次要色小字。
- **下划线**：`border-bottom:2px solid #73343E;font-weight:600;`。每段 1–3 个短短语。下划线用主色，不再引入木色。

## 写法参考

版首（挂旗）：

```html
<section style="padding:28px 14px 22px;background:#FBF6F1;">
  <span style="display:inline-block;width:18px;height:10px;background:#73343E;"></span>
  <span style="display:inline-block;width:18px;height:10px;margin-left:6px;background:#8A632C;"></span>
  <span style="display:inline-block;width:18px;height:10px;margin-left:6px;background:#73343E;"></span>
  <p style="margin:16px 0 0;font-size:28px;font-weight:700;color:#73343E;letter-spacing:1px;line-height:1.35;">主标题四到八字</p>
</section>
```

二级标题（短条，不再用木色）：

```html
<section style="margin:28px 10px 14px;">
  <span style="display:inline-block;width:28px;height:8px;background:#73343E;"></span>
  <p style="margin:10px 0 0;font-size:18px;font-weight:700;color:#73343E;line-height:1.4;">小标题</p>
</section>
```

卡片小结：

```html
<section style="margin:16px 10px 0;padding:18px 16px;background:#F8EEEA;border-radius:8px;">
  <p style="margin:0;font-size:16px;line-height:1.9;color:#3F3438;">一句话带走。</p>
</section>
```

## 适配场景

亲子阅读、绘本导读、睡前故事、社区故事、儿童活动记录。门票测评和硬阴影卡片用 `moyu-ticket`。胶带手账用 `collage-journal`。

## 挑图气质

- styleAnchor：绘本暖纸，酒红挂旗与一格木色，圆角短文，手绘但平整
- lightingHint：室内暖光，纸面干净，阴影很轻
