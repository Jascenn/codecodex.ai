---
layout: post
title: "🚀 3 分钟上手 OpenClaw + LionCC"
date: 2026-02-04 10:00:00
summary: "OpenClaw 是真正能帮你干活的 AI 助手，清理邮箱、管日历、自动值机……本文教你用 LionCC 3 分钟快速配置 OpenClaw，接入 Claude 最强模型，国内网络直连使用！"
categories: [教程, AI工具]
tags: ["AI工具", "Claude", "OpenClaw", "LionCC", "教程"]
cover: "/images/openclaw_hero_banner.png"
---

![封面](/images/openclaw_hero_banner.png)

> ✨ **OpenClaw** — 真正能帮你干活的 AI 助手。清理邮箱、发邮件、管日历、自动值机……通过 WhatsApp、Telegram 等聊天软件就能指挥它！

---

## 🎯 它能干嘛？

- 📧 **邮件管理** — 清理收件箱、自动写回复
- 📅 **日历协调** — 智能安排日程
- ✈️ **出行助手** — 自动值机、查航班
- 🌐 **浏览器控制** — 填表单、抓数据
- 💬 **多平台聊天** — WhatsApp / Telegram / Discord / Slack
- 🔒 **隐私优先** — 本地运行，数据不外泄

---

## 📋 准备工作

先装一个软件：**Node.js**

1. 👉 打开 [nodejs.org](https://nodejs.org)
2. 📥 下载 **LTS 版本**
3. ✅ 双击安装，一路下一步

---

## 🛠️ 安装（复制粘贴就行）

打开终端（Mac）或命令提示符（Windows），依次执行：

```bash
# 💻 第 1 步：安装 OpenClaw
npm install -g openclaw

# 💻 第 2 步：安装 LionCC
curl -fsSL https://raw.githubusercontent.com/Jascenn/lioncc/main/install.sh | bash
```

---

## 🔑 获取 API Key

1. 👉 打开 [vibecodingapi.ai](https://vibecodingapi.ai/login)
2. 📝 注册登录
3. ➕ 点「令牌管理」→「添加新令牌」
4. 🏷️ 分组选 `Claude Code(CC)`
5. 📋 复制 Key

---

## ⚙️ 用 LionCC 配置 OpenClaw

```bash
lioncc
```

👇 按提示完成 3 步：

1. 🔑 **输入 API Key** → 粘贴刚才复制的 Key
2. 🏢 **选择服务商** → 用 ↑↓ 方向键选择 VibeCoding，按回车确认
3. 🤖 **选择模型** → 推荐选 `claude-opus-4-5-20251101`（最强）

✅ 配置完成后会显示「Configuration saved!」

---

## ▶️ 启动使用

开两个终端窗口：

![双窗口](/images/startup_two_windows.png)

```bash
# 🖥️ 窗口 1
openclaw gateway

# 💬 窗口 2
openclaw tui
```

🎉 搞定！开始聊天吧！

---

## 📚 更多教程

👉 **[飞书知识库完整文档](https://my.feishu.cn/wiki/Dp8ywZfZKiVTWNkS9lucS5sDnkg)**

---

## 🆘 遇到问题？

| 问题 | 解决方法 |
|------|---------|
| ❌ command not found | 重装 Node.js，重启终端 |
| 😐 没反应 | 检查窗口 1 是否在运行 |
| 🔄 换 Key | 重新运行 `lioncc` |

---

## 🔗 链接汇总

- 🦞 [openclaw.ai](https://openclaw.ai)
- 🔑 [vibecodingapi.ai](https://vibecodingapi.ai)
- 📖 [飞书文档](https://my.feishu.cn/wiki/Dp8ywZfZKiVTWNkS9lucS5sDnkg)
