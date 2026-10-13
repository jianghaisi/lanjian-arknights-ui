# 岚笺 · 明日方舟风味 UI Skill

从岚笺已发布界面、设计文档和历史设计决定中提炼的可复用 Codex 技能。

基线是 [jianghaisi/lanjian 的公开提交 0873296](https://github.com/jianghaisi/lanjian/tree/08732963211976c13f206d01732126d72afd5417)。只收录这套已上传版本的档案终端语言，另一套空间 UI 预研不在范围内。

## 设计语言

暖纸和墨色承载中文阅读，深绿识别区承载作品身份，暖橙突出当前动作。通过细线网格、微编号、定位标记和少量切角建立档案秩序。正文保持稳定纸面；助笔、群聊保留发布版本的局部圆角与消息身份。

覆盖作品库、资料与表单、经典目录/正文/助笔工作台、主题、日常反馈、作品载入及独立开场。规则按组件职责使用，不要求更换技术栈或安装前端依赖。

## 安装

首次安装，将仓库克隆到个人 Codex 技能目录。

Windows PowerShell：

```powershell
git clone https://github.com/jianghaisi/lanjian-arknights-ui.git "$env:USERPROFILE/.codex/skills/lanjian-arknights-ui"
```

macOS / Linux：

```bash
git clone https://github.com/jianghaisi/lanjian-arknights-ui.git ~/.codex/skills/lanjian-arknights-ui
```

如果使用自定义 CODEX_HOME，将目标放到该目录的 skills/lanjian-arknights-ui 下。

## 使用

```text
使用 $lanjian-arknights-ui，按岚笺已发布版本的档案终端风格设计这个页面，保留现有功能与组件职责。
```

## 文件

| 文件 | 内容 |
| --- | --- |
| [SKILL.md](SKILL.md) | 触发范围、设计判断与工作方法 |
| [design-system.md](references/design-system.md) | 配色、中文排版、尺寸、主题与几何 |
| [patterns-and-motion.md](references/patterns-and-motion.md) | 页面组合、经典工作台与动效 |
| [provenance.md](references/provenance.md) | 固定版本、公开源码及实机截图出处 |
| [openai.yaml](agents/openai.yaml) | 技能显示名称与调用示例 |

仓库只提供技能说明和元信息，不附带私人对话、研究记录、应用源码、插画、字体或声音资产。公开来源链接固定到上述提交，后续主分支变化不会自动改变这份技能的依据。
