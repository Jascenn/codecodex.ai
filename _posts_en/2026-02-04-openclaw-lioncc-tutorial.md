---
layout: post
title: "🚀 Get Started with OpenClaw + LionCC in 3 Minutes"
date: 2026-02-04
summary: "OpenClaw is an AI assistant that actually does things — clears your inbox, manages calendars, auto check-in for flights. This guide shows you how to configure OpenClaw with LionCC in 3 minutes, connecting to Claude's most powerful models with direct China network access!"
categories: [Tutorial, AI Tools]
tags: ["AI Tools", "Claude", "OpenClaw", "LionCC", "Tutorial"]
cover: "/images/openclaw_hero_banner.png"
lang: en
lang_ref: openclaw-lioncc-tutorial
---

![Banner](/images/openclaw_hero_banner.png)

> ✨ **OpenClaw** — The AI that actually does things. Clears your inbox, sends emails, manages calendars, auto check-in... Control it through WhatsApp, Telegram, or any chat app!

---

## 🎯 What Can It Do?

- 📧 **Email Management** — Clear inbox, auto-reply
- 📅 **Calendar Coordination** — Smart scheduling
- ✈️ **Travel Assistant** — Auto check-in, flight lookup
- 🌐 **Browser Control** — Fill forms, scrape data
- 💬 **Multi-platform Chat** — WhatsApp / Telegram / Discord / Slack
- 🔒 **Privacy First** — Runs locally, your data stays yours

---

## 📋 Prerequisites

Install one software first: **Node.js**

1. 👉 Go to [nodejs.org](https://nodejs.org)
2. 📥 Download the **LTS version**
3. ✅ Double-click to install, next all the way

---

## 🛠️ Installation (Just Copy & Paste)

Open Terminal (Mac) or Command Prompt (Windows), run:

```bash
# 💻 Step 1: Install OpenClaw
npm install -g openclaw

# 💻 Step 2: Install LionCC
curl -fsSL https://raw.githubusercontent.com/Jascenn/lioncc/main/install.sh | bash
```

---

## 🔑 Get Your API Key

1. 👉 Go to [vibecodingapi.ai](https://vibecodingapi.ai/login)
2. 📝 Register and login
3. ➕ Click "Token Management" → "Add New Token"
4. 🏷️ Select group `Claude Code(CC)`
5. 📋 Copy the Key

---

## ⚙️ Configure OpenClaw with LionCC

```bash
lioncc
```

👇 Follow the prompts to complete 3 steps:

1. 🔑 **Enter API Key** → Paste the key you just copied
2. 🏢 **Select Provider** → Use ↑↓ arrow keys to select VibeCoding, press Enter
3. 🤖 **Select Model** → Recommended: `claude-opus-4-5-20251101` (strongest)

✅ You'll see "Configuration saved!" when done

---

## ▶️ Start Using

Open two terminal windows:

![Two Windows](/images/startup_two_windows.png)

```bash
# 🖥️ Window 1
openclaw gateway

# 💬 Window 2
openclaw tui
```

🎉 Done! Start chatting!

---

## 📚 More Resources

👉 **[Full Documentation on Feishu](https://my.feishu.cn/wiki/Dp8ywZfZKiVTWNkS9lucS5sDnkg)**

---

## 🆘 Troubleshooting

| Issue | Solution |
|-------|----------|
| ❌ command not found | Reinstall Node.js, restart terminal |
| 😐 No response | Check if Window 1 is running |
| 🔄 Change Key | Re-run `lioncc` |

---

## 🔗 Quick Links

- 🦞 [openclaw.ai](https://openclaw.ai)
- 🔑 [vibecodingapi.ai](https://vibecodingapi.ai)
- 📖 [Feishu Docs](https://my.feishu.cn/wiki/Dp8ywZfZKiVTWNkS9lucS5sDnkg)
