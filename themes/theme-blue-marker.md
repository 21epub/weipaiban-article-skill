# 蓝标简编 · 科技感零装饰流式

电光蓝章节编号、冰蓝青小标题与引用线，近白底、渐变短线分层。由「红标简编」换色并微调骨架而来，适合科技感拆解长文。建议语法：章节流、叙事流。

全篇靠字号、字色、加粗、留白与一条渐变短线分层，不靠卡片与复杂装饰。

## Token

```
主色 primary     #0057E8
辅色 accent      #00B2D6
正文 text        #444444
次要 muted       #888888
图注 caption     #999999
线   line        #00B2D6
浅底 wash        #F3F8FC
作品底 canvas    #FDFDFC
渐变 gradient    linear-gradient(90deg,#0057E8,#00B2D6)
```

主色只用于章节编号与章节标题；辅色只用于栏目小标、三级小标题与引用左边线。不要第三种彩色。电光蓝用 `#0057E8`，不用纯蓝。作品底用 `#FDFDFC`，不用纯白。章节标题 18px。

段距 18px 高于通用表的 8–12px。本主题的分割语言是渐变短线 + 留白，段距保持 18px，章节前保持 36px。

## 形态（一篇一套）

- **版首**：不写大标题。文章标题由微信原生头部承担。版首开头顶部一条通栏渐变细线（2px，`linear-gradient(90deg,#0057E8,#00B2D6)`），下接一行栏目小标（12px / 700 / `#00B2D6` / 字距 3px，可带英文小字），再进导语段。
- **章节标题**：单行式「`01｜` + 标题」，`18px / 700 / #0057E8 / line-height 1.3 / 左齐 / 字距 0.5px`；标题正下方 8px 处跟一条 48×3px 渐变短线（圆角 2px）。章节前留 36px 空白。不用编号胶囊、不用左竖条、不用通栏底边线。
- **三级小标题**：左对齐，`16px / 700 / #00B2D6`，`border-left:4px solid #00B2D6` + 左内边距 10px，上 22px 下 8px。全篇统一，不要改成居中或加前缀符号。
- **分割**：渐变短线 + 留白。全篇唯一的装饰线就是章节标题下与版首的渐变短线，不再画其它细线、不放装饰分隔符。
- **卡片**：不用卡片、不用阴影。要点直接用正文段落 + `<b>` 加粗短句表达；引用块是唯一带底色的元素。
- **引用**：浅蓝底 `background-color:#F3F8FC` + `border-left:3px solid #00B2D6`，右侧圆角 `border-radius:0 8px 8px 0`，无阴影；文字 `15px / #888888`，内边距 `12px 14px`。
- **图片**：宽 88%、居中、`border-radius:10px`、无描边无阴影。图注 12px `#999999` 左齐，图下 20px。
- **下划线**：不用下划线。强调只用 `<b>` 加粗，不换色。
- **结尾信息**：需要补充说明时，用 12px 灰色小字逐行平铺，无框无底，行距 1.9。
- **正文**：14px / line-height 1.9 / `#444444` / justify / 段距 18px / 左右页边距 10px。
- **圆角**：图片 10px、引用块右侧 8px、渐变短线 2px，全篇就这三处。图文 SVG 主图圆角跟图片，用 10px。

## 写法参考

版首（渐变细线 + 栏目小标 + 导语）：

```html
<section style="padding:16px 10px 0;">
  <section style="width:100%;height:2px;border-radius:1px;background:linear-gradient(90deg,#0057E8,#00B2D6);margin-bottom:14px;"></section>
  <p style="margin:0 0 14px;font-size:12px;font-weight:700;color:#00B2D6;letter-spacing:3px;">栏目小标 · COLUMN</p>
  <p style="margin:0 0 18px;font-size:14px;line-height:1.9;color:#444444;text-align:justify;">开篇先给读者一个具体场景，再进入这一节要讲的事情。</p>
</section>
```

章节标题（单行 + 渐变短线）：

```html
<section style="margin:36px 10px 14px;">
  <p style="margin:0;font-size:18px;font-weight:700;color:#0057E8;line-height:1.3;letter-spacing:0.5px;">01｜先把问题说清楚</p>
  <section style="margin-top:8px;width:48px;height:3px;border-radius:2px;background:linear-gradient(90deg,#0057E8,#00B2D6);"></section>
</section>
```

三级小标题（青竖条左对齐）+ 要点：

```html
<section style="padding:0 10px;">
  <p style="margin:22px 0 8px;padding-left:10px;border-left:4px solid #00B2D6;font-size:16px;font-weight:700;color:#00B2D6;line-height:1.4;">这一层在讲什么</p>
  <p style="margin:0 0 18px;font-size:14px;line-height:1.9;color:#444444;text-align:justify;">用普通段落把步骤写完。<b>需要记住的短句</b>只加粗，不换色。</p>
</section>
```

图片 + 图注（88% 居中、10px 圆角）：

```html
<section style="padding:6px 10px 0;">
  <section style="text-align:center;line-height:0;">
    <img src="{manifest.src}" style="display:block;width:88%;margin:0 auto;border-radius:10px;" />
  </section>
  <p style="margin:10px 0 20px;font-size:12px;line-height:1.6;color:#999999;text-align:left;">图注写在图下，说明这张图对应哪一步</p>
</section>
```

引用（浅蓝底 + 3px 青线 + 右侧圆角）：

```html
<section style="padding:0 10px;">
  <blockquote style="margin:18px 0;padding:12px 14px;background-color:#F3F8FC;border-left:3px solid #00B2D6;border-radius:0 8px 8px 0;font-size:15px;line-height:1.9;color:#888888;">把一句判断单独提出来，让读者在长文里能停一下。</blockquote>
</section>
```

结尾信息行：

```html
<section style="padding:0 10px 24px;">
  <p style="margin:0;font-size:12px;line-height:1.9;color:#888888;">补充说明</p>
  <p style="margin:0;font-size:12px;line-height:1.9;color:#888888;">阅读对象</p>
  <p style="margin:0;font-size:12px;line-height:1.9;color:#888888;">发布日期</p>
</section>
```

## 适配场景

科技产品拆解、AI / 大模型工具教程、互联网产品复盘、数码评测、SaaS 功能说明、开发者向长文。适合「以界面截图或科技插画为主、文字讲逻辑」的内容。不适合党政节庆（用 `red-white`）、暖调营销复盘（用 `red-marker`）、深底电竞氛围（用 `cyber-dark`）。

## 挑图气质

- styleAnchor：科技感界面与光效插画，蓝青色系，深蓝紫渐变背景或浅底科技场景，信息密度偏高，界面感构图，88% 居中留白
- lightingHint：冷色光效直出，蓝青发光线条，干净高光，不加暖色滤镜
