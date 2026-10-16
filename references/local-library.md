# 连接用户自己的资料库

本地库是可选增强，技能不绑定某位用户的磁盘或项目目录。优先使用用户给定的位置；未指定时可只读检查当前项目是否已有 `design_library`。确认库内确有 `WORKFLOW.md`、`index.md` 与需要的目录/脚本后再使用，不把文档示例路径当成现存资料。

原始资料的位置以该库 `sources.json` 或用户指定为准，保持只读。派生记录写入该库允许的输出位置；不移动或打包原始来源。目标项目自己的开发规范仅在修改那个项目时适用，不扩展为所有设计工作的门禁。

找不到库时使用 [内置文字配方](portable-style-recipes.md)，明确原始参考不可展示；也可按 [原始参考索引](style-preview-gallery.md) 定位用户已有来源或允许访问的原始地址，不用AI生成图补位。检索原库、增量建库或精确找回原图的请求需要先解决来源缺失，不能臆造STYLE或声称完成检索。

## 按任务读取

- 总入口：`WORKFLOW.md`、`index.md`。
- 检索/提示词：`catalog/styles.json`、所选 `styles/STYLE-xxx.md`、`prompts/reusable_prompt_recipes.md`。
- 选择时的图片：先核对卡片对应的原始图/忠实预览关系，再查看实际图；AI概念稿不作选风格的示例。[原始参考索引](style-preview-gallery.md) 保留28卡/47来源的元信息快照，不包含原始图片或安装者的本地路径；实时数量以用户实际库为准。
- 实际生图：`GENERATION_EVAL_WORKFLOW.md`。在库内 `experiments/` 建版本记录，不覆盖旧图。
- 增量分析：`reports/coverage.md`、`catalog/assets.json` 和 `sources.json`。不要把缩略图、生成图或未看过的资料算成已审阅原作。
- 用户明确要组件：`components/index.md`、所选风格组合章节、`catalog/compositions.json`。

## 复用现有脚本

仅当用户项目确有以下目录与脚本时，从其项目根运行；库放在其他位置就使用已经核对的真实路径。脚本并不随本技能分发，不自动安装或重建用户的库：

```powershell
python -X utf8 design_library/scripts/library.py list
python -X utf8 design_library/scripts/library.py recommend "科技展览 黄黑 海报"
python -X utf8 design_library/scripts/library.py prompt STYLE-001 "原创研究展览" --title "ROBOT LAB" --aspect 16:9
python -X utf8 design_library/scripts/library.py changes
```

`prompt --title`只控制准确主标题，不会自动创建丰富的副标题、图标、说明。完整参考海报需要按任务补充准确文案层级与位置，不添加冲突的无字指令。

只有明确需要组件时才运行 `library.py recipe ...`。脚本输出配方不是实际生成结果，也不代表可以自动开始制作全部组件。

## 分发与维护边界

历史实验和私人研究日志不随技能提供。公开README中的生成图是一次试用产出，不是原始风格来源，也不能证明其他主题或模型会得到相同结果。

用户自己的库若由脚本生成卡片/索引，应修改相应生成器或来源记录，避免下次重建覆盖人工修订；没有对应脚本时不要自行臆造命令。普通设计请求不自动续做其他实验或组件包。
