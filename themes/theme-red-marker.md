# 红标简编 · 零装饰流式

正红章节标号、砖橙小标题与引用线，近白底、无卡片无分割。建议语法：章节流、叙事流。

全篇靠字号、字色、加粗和留白分层，不靠容器、色块或装饰线。

## Token

```
主色 primary     #E1251B
辅色 accent      #D85A30
正文 text        #444444
次要 muted       #888888
图注 caption     #999999
线   line        #D85A30
浅底 wash        #FBF6F4
作品底 canvas    #FDFDFC
```

主色只用于章节编号与章节标题；辅色只用于三级小标题与引用左边线。不要第三种彩色。正红用 `#E1251B`，不用纯红。作品底用 `#FDFDFC`，不用纯白。章节标题 18px。

段距 18px 高于通用表的 8–12px。本主题的分割语言就是留白，段距保持 18px，章节前保持 32px。

## 形态（一篇一套）

- **版首**：不写大标题。文章标题由微信原生头部承担，正文直接从导语段开场。确需版首时只用一行 22px 深色字，不加色条、不加英文小标、不加底边线。
- **章节标题**：两行式，不用 flex、不用编号胶囊、不用左竖条、不用底边线。第一行「`01` + 上半句」，第二行「下半句」，两行连排 margin 0，均 `18px / 700 / #E1251B / line-height 1.1 / 左齐`。章节前留 32px 空白。
- **三级小标题**：居中、`16px / 700 / #D85A30`，上 22px 下 8px。全篇统一，不要改成左齐或加前缀符号。
- **分割**：**留白**。全篇不画细线、不角色条、不放装饰分隔符，章节只靠 28–32px 间距断开。
- **卡片**：不用卡片、不用背景块、不用阴影。要点直接用正文段落 + `<b>` 加粗短句表达。
- **引用**：`border-left:3px solid #D85A30`，无底色、无圆角、无阴影；文字 `15px / #888888`，左内边距 14px。
- **图片**：宽 70%、居中、`border-radius:5px`、无描边无阴影。图注 12px `#999999` 左齐，图下 20px。
- **下划线**：不用下划线。强调只用 `<b>` 加粗，不换色。
- **结尾信息**：需要补充说明时，用 12px 灰色小字逐行平铺，无框无底，行距 1.9。
- **正文**：14px / line-height 1.9 / `#444444` / justify / 段距 18px / 左右页边距 10px。
- **圆角**：全篇只有图片 5px 这一处，卡片圆角不适用。图文 SVG 主图圆角跟图片，用 5px。

## 写法参考

导语开场（不加版首）：

```html
<section style="padding:16px 10px 0;">
  <p style="margin:0 0 18px;font-size:14px;line-height:1.9;color:#444444;text-align:justify;">开篇先给读者一个具体场景，再进入这一节要讲的事情。</p>
</section>
```

章节标题（两行式）：

```html
<section style="margin:32px 10px 18px;">
  <p style="margin:0;font-size:18px;font-weight:700;color:#E1251B;line-height:1.1;">01  先把问题说清楚</p>
  <p style="margin:0;font-size:18px;font-weight:700;color:#E1251B;line-height:1.1;">再给出这一节的答案</p>
</section>
```

三级小标题 + 要点：

```html
<section style="padding:0 10px;">
  <p style="margin:22px 0 8px;font-size:16px;font-weight:700;color:#D85A30;text-align:center;">这一层在讲什么</p>
  <p style="margin:0 0 18px;font-size:14px;line-height:1.9;color:#444444;text-align:justify;">用普通段落把步骤写完。<b>需要记住的短句</b>只加粗，不换色。</p>
</section>
```

图片 + 图注（70% 居中、5px 圆角）：

```html
<section style="padding:10px;">
  <section style="text-align:center;line-height:0;">
    <img src="{manifest.src}" style="display:block;width:70%;margin:0 auto;border-radius:5px;" />
  </section>
  <p style="margin:10px 0 20px;font-size:12px;line-height:1.6;color:#999999;text-align:left;">图注写在图下，说明这张图对应哪一步</p>
</section>
```

引用（3px 橙线）：

```html
<section style="padding:0 10px;">
  <blockquote style="margin:18px 0;padding:4px 0 4px 14px;border-left:3px solid #D85A30;font-size:15px;line-height:1.9;color:#888888;">把一句判断单独提出来，让读者在长文里能停一下。</blockquote>
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

案例拆解、营销复盘、产品功能说明、操作教程、企业内刊、服务商获客长文。适合「以界面截图为主、文字讲逻辑」的内容。不适合品牌大片、节庆海报、需要氛围感的叙事长文——那些请用 `editorial-serif` 或 `glassmorphism`。党政与节庆庄重请用 `red-white`。

## 挑图气质

- styleAnchor：产品界面截图原色，白底或浅底，无滤镜，信息密度偏高，70% 居中留白，红橙 UI 点缀
- lightingHint：界面原色直出，不加布光、不加渐变
