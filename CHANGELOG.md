# Changelog

本项目遵循 [Keep a Changelog](https://keepachangelog.com/zh-CN/1.1.0/) 规范，版本号遵循 [语义化版本](https://semver.org/lang/zh-CN/)。

## [Unreleased]

## [1.2.0] - 2026-11-23

### 新增

- 新增主题红标简编（`red-marker`）：正红章节编号、砖橙小标题与引用线，近白底，无卡片无分割，靠字号、字色、加粗和留白分层
- 主题总数 19 套（经典系 6，趋势系 13）。选主题脚本与主题清单已同步

### 变更

- `metadata.openclaw` 改为一条 JSON 字符串，键和值都是字符串，便于豆包校验技能元数据

## [1.1.0] - 2026-11-21

### 新增

- 新增 6 套主题：像素现场、浅蓝水彩、靛蓝布标、复古报刊、手绘绘本、青春校园。气质参考公开排版方向，版式为本仓库原创
- 主题总数 18 套（经典系 6，趋势系 12）。选主题脚本与主题清单已同步

## [1.0.4] - 2026-11-17

随包附上完整许可证，详情页补改编说明。流程与 1.0.3 相同。

### 变更

- 许可证文件改为 `LICENSE.txt`，仓库与 SkillHub 安装包共用这一份全文
- `README.md` 的许可证链接改为 `LICENSE.txt`
- `overview.md` 与 `SKILL.md` 写明基于甲木 × 摸鱼小李的 gzh-design-skill 改编，并附原仓库链接
- 版本号改为 `1.0.4`

## [1.0.3] - 2026-11-15

更换 SkillHub 技能图标。流程与 1.0.2 相同。

### 变更

- 技能图标改为微排版标识

## [1.0.2] - 2026-11-15

重新发布当前技能包。流程与 1.0.1 相同。

### 变更

- 说明里不再写出服务端转换函数名
- 注意事项不再指向画布导入技能
- `scripts/publish.py` 注释与当前 API 源站校验一致

## [1.0.1] - 2026-11-15

本次只调整 SkillHub 上架信息，便于按「公众号排版」「公众号文章」「微信图文」被找到。技能流程与 1.0.0 相同。

### 变更

- `SKILL.md` 展示名改为「微排版公众号文章排版」，短简介、长描述和标签改为公众号排版、文章排版、微信图文、轮播
- frontmatter 增加 `license: AGPL-3.0`，版本号改为 `1.0.1`
- `overview.md` 改成给详情页读者看的公众号文章排版说明
- `README.md` 首段改为公众号文章排版

## [1.0.0] - 2026-11-14

首次按 SkillHub 上架形态整理。文章工作流与已安装的 `weipaiban-article` 相同。

### 新增

- `SKILL.md` 增加 `slug`、`displayName`、`summary`、`version`、`tags`、`homepage`，展示名为「微排版公众号流式文章」
- 新增 `overview.md`，作为 SkillHub 详情页概述
- `README.md` 改为人类说明，并补充开源仓库与微信交流群二维码（`assets/contact-me-qr.png`）
- 新增 `scripts/api_base.py`。发布、取素材、上传共用源站校验，只接受 `https://weipaiban.cn`（含子域）或本机回环，并校验 TLS 证书
- 说明 `WEIPAIBAN_API_KEY` 在 <https://weipaiban.cn/settings/api-keys> 创建或复制

### 变更

- `python3` 改为必需二进制；`rembg` 仍为可选，技能不会自动安装
- 发布与取素材脚本不再提供跳过证书校验的开关
