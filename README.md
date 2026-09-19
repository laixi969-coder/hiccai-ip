# hiccai-ip

IP 形象设计与诊断 skill：先判断用途与载体，再把轮廓、比例、五官转成设计动作和验证方法。

适用于品牌吉祥物、潮玩、文创、系列角色的从零策划、升级、AI 改稿与方案评审。支持快速诊断和完整方案，也支持只改表情等局部任务。

## 使用

将整个仓库目录安装到所用工具的 skills 目录。例如 Codex：

```bash
git clone https://github.com/laixi969-coder/hiccai-ip.git ~/.codex/skills/hiccai-ip
```

已有同名目录时先更新已有安装。使用示例：

- “用 hiccai-ip 帮我诊断这个品牌吉祥物，先看识别问题。”
- “这个角色要做成 12 厘米毛绒挂件，哪些结构应调整？”
- “轮廓已经注册，只改五官，让表情更委屈。”
- “给博物馆文创做文化保留项、产品载体和购买理由推导。”

## 结构

[SKILL.md](SKILL.md) 是入口，按任务读取参考资料：

| 文件 | 用途 |
|---|---|
| [01 设计观](references/01-design-principle.md)、[02 第一用途](references/02-first-use.md) | 作用与定位 |
| [03 三变量](references/03-three-variables.md)、[04 设计路径](references/04-design-paths.md) | 改稿变量与项目路径 |
| [05 流程](references/05-workflow.md)、[06 检查表](references/06-checklist.md) | 执行与证据验收 |
| [07 案例库](references/07-case-library.md) | 案例对照 |
| [08 来源边界](references/08-source-and-boundary.md) | 转写疑点、引用方式 |
| [09 索引](references/09-corpus-index.md)、[10 转写](references/10-spoken-corpus.md) | 按视频 ID 查来源 |
| [11 应用卡](references/11-application-cards.md) | 从口播到动作、载体与验证 |
| [test-prompts.json](test-prompts.json) | 行为验收场景及判据，不是自动化测试结果 |

## 1.1.0 的调整

- 从“固定顺序改稿”改为按问题选变量，保留用户锁定资产。
- 补充有来源的视频 ID 应用卡、社交与内容路径。
- 区分统一素体换装系列与独立角色家族，不强制所有系列重做结构。
- 验收按真实证据记为已验证、待验证或不适用；16 项全适用时满分 32。
- 原始语料保持不变，新增 54 个视频 ID 索引，标出 1 条无有效口播的记录。

## 来源与许可范围

材料源于用户提供的转写及仓库既有“徐阿乐 IP判断”资料。54 条记录中 53 条含实质文本，1 条只有字幕署名；尚未逐条回查音视频。整理后的引文不是经过核实的逐字原话，历史账号统计也不代表当前状态。

本 skill 的整理部分沿用 MIT 标记，不涵盖第三方原始表达与品牌资产。新项目建议属于方法论应用，不代表原作者观点。详细疑点见来源说明。
