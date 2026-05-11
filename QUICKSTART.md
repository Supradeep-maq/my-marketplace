# ⚡ Quick Start

Install and use Work IQ Email Helper plugin in 3 commands!

---

## 🚀 Installation

```powershell
# 1. Add marketplace
copilot plugin marketplace add yourusername/my-marketplace

# 2. Browse (optional)
copilot plugin marketplace browse workiq-helper

# 3. Install
copilot plugin install workiq-helper
```

---

## 💡 Usage

```powershell
# Start Copilot
copilot

# Then ask:
> Summarize email abc123 from Work IQ
> Extract action items from email def456
> What's the sentiment of email ghi789?
```

Or one-shot:
```powershell
copilot "Summarize my Work IQ email ID abc123"
```

---

## ✨ Available Tools

- **summarize_email** - Summarize emails/threads
- **extract_action_items** - Extract tasks
- **get_email_sentiment** - Analyze tone

---

## 📁 What's Inside?

```
my-marketplace/
├── marketplace.json          # Plugin registry
├── README.md                # Full docs
├── INSTALL.md              # Installation guide
└── plugins/
    └── workiq-helper/
        ├── .mcp.json       # MCP config (NO CODE!)
        ├── plugin.json     # Tool schemas (NO CODE!)
        └── README.md       # Plugin docs
```

**Configuration-only - absolutely no custom code!**

---

## 🌐 Deploy to GitHub

```powershell
cd "c:\Users\v-rsupradeep\Music\Test plugin"
git init
git add .
git commit -m "Initial commit"
gh repo create my-marketplace --public --source=. --push
```

Update `yourusername` in `marketplace.json` to your GitHub username, then:

```powershell
git add marketplace.json
git commit -m "Update repository URL"
git push
```

---

## 📚 Documentation

- **[README.md](README.md)** - Full documentation
- **[INSTALL.md](INSTALL.md)** - Detailed installation guide
- **[Plugin README](plugins/workiq-helper/README.md)** - Plugin details

---

**That's it!** Pure configuration, no code, works everywhere. 🎉
