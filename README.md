# 贾樟柯导演风格 Skill

把公开导演访谈、电影节与片方资料中的影像方法，整理成可研究、可写作、可拍摄、可剪辑的工作方式。支持风格记录、作品比较、原创剧本、导演阐述、分镜、剪辑诊断与视频提示词。

资料覆盖《小武》《站台》《任逍遥》《世界》《三峡好人》《二十四城记》《天注定》《山河故人》《江湖儿女》《风流一代》10 部代表作，比较持续主题与形式差异。技能不是导演本人或官方出品。

## 能做什么

- 记录叙事、人物、地方经验、时代变化、空间、摄影距离、镜头时间、声音与媒介等 18 个维度。
- 解释长镜头、固定镜头与远景的区别，设计镜头内部变化、切点及 12 种可选切换方案。
- 按演员、场地、设备和片长，把原创故事落实成动作、声音与可执行镜头表。
- 分析已有剧本或素材；保留用户指定的意图，按请求选择诊断或改写。

## 安装

下载本仓库后，把完整的 `jia-zhangke-skill` 目录复制到 `~/.codex/skills/jia-zhangke-skill`。例如，在仓库根目录执行：

```sh
mkdir -p ~/.codex/skills
cp -R ./jia-zhangke-skill ~/.codex/skills/
```

若目标目录已有同名技能，先比较并备份，再替换；避免新旧文件混合。

## 调用示例

```text
用 $jia-zhangke-skill，比较《小武》和《站台》的摄影距离与镜头切换，附来源。

用 $jia-zhangke-skill，写一个 60 秒原创短片：两名演员、一个便利店、手机拍摄，给剧本、分镜、切点和声音。

用 $jia-zhangke-skill，只诊断这段剧本的生活真实感和镜头切换，不重写。

用 $jia-zhangke-skill，把我提供的旧影像整理成素材索引，再提出剪辑主线。
```

## 技能文件

技能目录包含以下 10 个文件；本 README 为仓库说明。

```text
jia-zhangke-skill/
├── SKILL.md                         # 入口、任务路由与检查要求
├── agents/openai.yaml               # 显示名称与默认调用提示
├── assets/
│   ├── creative-brief.md             # 创作简报模板
│   └── shot-list.csv                 # 分镜表模板
└── references/
    ├── style-atlas.md                # 18 个风格维度
    ├── film-map.md                   # 10 部作品的方法差异
    ├── shot-editing.md               # 机位、内部变化、切点与声音
    ├── creation-workflow.md          # 研究、创作、诊断和素材流程
    ├── original-example.md           # 60 秒原创示例《留一盏灯》
    └── sources.md                    # 来源链接与证据归属
```

## 资料与制作边界

[来源说明](jia-zhangke-skill/references/sources.md)区分导演表述、作品事实、分析归纳与原创创作迁移，并记录版本差异。资料核对日期为 2026-10-13；历史访谈不自动代表导演当前全部观点。

本技能覆盖主要维度和代表作，未逐帧审阅全部影片。具体时码、焦距、单镜时长、剪切频率或调色参数，需要另核可观看的影片版本；示例秒数和机位是原创项目设计值。文本方案与结构检查不能代替试拍、实际生成或成片验收。

技能支持原创表达，不自称复刻原片；长镜头、方言、废墟、舞蹈、灰色调均不是每次必用的公式。媒体生成按当前工具能力另行执行。

进一步阅读：[风格库](jia-zhangke-skill/references/style-atlas.md) · [作品差异](jia-zhangke-skill/references/film-map.md) · [镜头与剪辑](jia-zhangke-skill/references/shot-editing.md) · [创作流程](jia-zhangke-skill/references/creation-workflow.md) · [完整示例](jia-zhangke-skill/references/original-example.md)。
