# 来源与版本边界

## 冻结依据

本技能来自 [岚笺 GitHub 发布源码](https://github.com/jianghaisi/lanjian/tree/08732963211976c13f206d01732126d72afd5417)，固定提交 `08732963211976c13f206d01732126d72afd5417`，对应本次提炼时已上传 GitHub 的0.1版本。后续 main 变化不自动重写本技能；更新技能时重新对照指定版本及用户决定。

作者要求先从既有 Codex 对话和设计文档溯源，并明确两套方案中只提炼已上传版本。研究先定位迁移前后153份日志，筛出169条去重UI线索，核对34条必要用户短引文，再将适用规则映射到固定提交源码/截图；技能编写时补齐来源，最终核对29个发布文件。关键词命中、历史开发批准、成品视觉接受是不同事实。私人原话及日志路径保留在原任务研究记录，不放入可分发技能。

## 可公开核对的视觉资料

- [README 桌面模块说明](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/README.md)：书库、编辑、定义、资料、世界、大纲、纪事等模块。
- [截图来源](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/docs/assets/README.md)：2026-10-12安装后Windows0.1.0实机，独立示例数据；不含作者小说或模拟模型回复。
- [作品库](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/docs/assets/desktop-library.png)：整体身份、几何、书名层级、主档案与快捷入口。
- [编辑与助笔](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/docs/assets/desktop-editor.png)：经典目录/纸面/助笔分工及局部圆角。
- [定义表单](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/docs/assets/desktop-definition.png)：档案标题、核心设想与表单层级。

截图是该版本当时的实际呈现，不能独立证明全部主题、硬件、生成或动态行为已验收。素材被截入README不改变其授权；本技能不复制图片、角色、字体或音频。

## 规则与源码对应

| 规则 | 固定提交源码 |
| --- | --- |
| 颜色、语义尺度与主题 | [narrative-tokens.css](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/desktop/src/renderer/assets/narrative-tokens.css) |
| 本地字体别名与底层变量 | [desktop.css](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/desktop/src/renderer/assets/desktop.css) |
| 实际令牌映射 | [narrative-terminal.css](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/desktop/src/renderer/assets/narrative-terminal.css) |
| 样式入口与次序 | [main.js](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/desktop/src/renderer/app/main.js) |
| 工具页、表单、方角与容器堆叠 | [archive-workspace.css](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/desktop/src/renderer/assets/archive-workspace.css) |
| 经典工作台布局与编辑周边 | [approved-archive.css](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/desktop/src/renderer/assets/approved-archive.css)、[AppShell.vue](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/desktop/src/renderer/app/AppShell.vue) |
| 档案主卡、切角、空态及入口 | [LibraryArchiveHero.vue](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/desktop/src/renderer/features/library/components/LibraryArchiveHero.vue) |
| 作品集合与库内布局 | [ProjectLibrary.vue](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/desktop/src/renderer/features/library/components/ProjectLibrary.vue) |
| 标题层级与渐进显现 | [ArchivePageHeader.vue](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/desktop/src/renderer/ui/ArchivePageHeader.vue) |
| 字段标注/错误与动作壳 | [ArchiveFormField.vue](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/desktop/src/renderer/ui/ArchiveFormField.vue)、[ArchiveAction.vue](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/desktop/src/renderer/ui/ArchiveAction.vue) |
| 助笔密度、身份、局部圆角 | [assistant-workspace.css](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/desktop/src/renderer/features/assistant/assets/assistant-workspace.css)、[AssistantDocument.vue](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/desktop/src/renderer/features/assistant/components/AssistantDocument.vue) |
| 群聊独立展示语义 | [GroupChatWorkspace.vue](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/desktop/src/renderer/features/group-chat/components/GroupChatWorkspace.vue) |
| 日常面板/导航反馈 | [interaction-motion.css](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/desktop/src/renderer/assets/interaction-motion.css) |
| 作品载入 | [WorkspaceLoadingScreen.vue](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/desktop/src/renderer/features/library/components/WorkspaceLoadingScreen.vue) |
| 独立应用开场 | [AppBootScreen.vue](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/desktop/src/renderer/app/components/AppBootScreen.vue)、[CinematicBoot.vue](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/desktop/src/renderer/app/components/boot/CinematicBoot.vue)、[ImpactBoot.vue](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/desktop/src/renderer/app/components/boot/ImpactBoot.vue) |
| 原开场音效生命周期 | [useBootSounds.ts](https://github.com/jianghaisi/lanjian/blob/08732963211976c13f206d01732126d72afd5417/desktop/src/renderer/app/composables/useBootSounds.ts) |

在其他项目使用时，以上链接用于理解构图与组件职责；不强制搬入源代码、第三方依赖或岚笺业务。规则正文已经自包含。需要源码精确复现或更新版本时才读取对应源文件。

## 历史筛选结果

保留：人的完整任务链、书库档案精细度、字体/组件一致性、真实状态、长文信息密度、助笔身份与宽度、主题完整状态、作品热进入、日常转场以及已发布的档案开场。

排除：另一套空间工作区的三维章节阵列、底部空间导航、抽取/浮面编辑；官网特定玻璃人物/液体生长/倒三角背景；本地未发布变化和旧版整套数值。旧“不要绿色”不能否定当前深绿档案；早期方角反馈也不能抹掉公开版本已有的聊天圆角。

开场阵列与空间工作台虽共享档案意象，但拥有不同作用域。前者在本发布版已存在，后者是被用户排除的另一套方案。
