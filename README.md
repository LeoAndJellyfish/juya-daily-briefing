# Juya Daily Briefing

一个可复用的 Agent Skill：读取橘鸦 Juya AI 早报文字版、按期号去重、核对原始来源，并生成中文新闻精选。与 Juya 官方无隶属关系。

## 安装

将 `skills/juya-daily-briefing` 目录复制到你的全局技能目录：

- Windows：`%USERPROFILE%\.agents\skills\juya-daily-briefing`
- macOS / Linux：`~/.agents/skills/juya-daily-briefing`

目录中必须直接包含 `SKILL.md`。重启或重新加载支持 Agent Skills 的宿主后调用 `$juya-daily-briefing`，例如：“检查 Juya 最新一期，有更新时生成中文精选”。

## 功能

- latest、首页、归档交叉检查，RSS 仅为补充。
- 所有要闻纳入，另外精选模型、开发工具和研究洞察。
- 规范 URL 与期号去重，访问失败不误报无更新。
- 原始来源核查与明确的发布、内测、计划状态。
- 支持已有定时订阅，但不会自行创建调度、登录或发送到未授权目标。

需要宿主提供公开网页读取能力；自动推送还需要其调度与消息工具。私有去重状态应保存在技能目录以外，不要提交 GitHub。
