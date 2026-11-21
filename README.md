# Kazumi Source Hub · 扩展规则仓库

适用于 [Kazumi](https://github.com/Predidit/Kazumi) 的第三方动画搜索与播放规则。仓库于 2026-11-21 整理，**不是官方规则库**。

## 使用方式

1. 建议先使用 Kazumi 2.4.3 或更高版本。
2. 打开 **设置 → 规则管理 → 规则仓库**（具体菜单随版本变化）。
3. 添加这个仓库地址：

   `https://raw.githubusercontent.com/huangjun7hb/kazumi-source-hub/main/index.json`

4. 返回规则列表，先测试以下 5 条候选：`guangsu`、`mdzy`、`ruyi`、`maoyan`、`DM6900`。剩余 7 条为实验/旧站点候选。

本仓库首批收录 **12 条额外规则**，与 [Kazumi 官方 18 条规则](https://github.com/Predidit/KazumiRules) 分开。**规则能够导入不等于资源可播放**。建议按「搜索到作品 → 取得集数 → 实际播放」三步逐条验证；其中 4 条是通用视频资源站 API，不保证搜索结果都是动画。

## 规则及来源

| 原仓库 | 规则 | 状态 |
|---|---|---|
| [JHeyzo/KazumiRules](https://github.com/JHeyzo/KazumiRules) | guangsu、mdzy、ruyi、maoyan | 优先试用；未独立实测播放 |
| [abulice/kazumisource](https://github.com/abulice/kazumisource) | DM6900 | 作者报告近期测试；此处未独立实测，目标站点为 HTTP |
| [violetACER/kazumirules](https://github.com/violetACER/kazumirules) | anime1、animoe、FQDM、omofuns、xifan、yhdmat、yinghuadm | 实验候选；部分可能失效 |

**注意**：原始规则归原作者所有。文件按源仓库格式整理并注明出处；此处不托管或分发任何动画视频，也不保证外部站点持续可用。若使用后出现登录、黑屏、无集数、转圈等现象，先换规则或检查 Kazumi 的网络设置。


## 注意：不要把 index.json 链接粘贴到「导入规则」文本框

「导入规则」弹窗接受完整的规则 JSON（或 JSON 数组）、kazumi:// 分享链接，而不是规则仓库的 index.json URL。若要直接安装规则，请打开下列 JSON 的 Raw 内容，复制**文件内容**粘贴进导入框，或使用客户端支持的本地 JSON 文件导入方式：

- [优先试用：5 条规则（JSON 数组）](./import-priority.json)
- [实验候选：7 条规则（JSON 数组）](./import-experimental.json)

如果要添加规则仓库，请在「规则仓库」的自定义仓库设置里使用 [index.json](./index.json)，不要在「导入规则」弹窗输入它的 URL。

## 目录

- `index.json`：供 Kazumi 自定义规则仓库订阅的入口
- `<规则名>.json`：单条规则定义
- `sources.json`：上游来源记录

最后更新：2026-11-21。
