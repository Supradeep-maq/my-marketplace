# Work IQ Email Helper

Simple plugin that uses the **Work IQ MCP server** for email operations.

Work IQ MCP automatically handles Outlook authentication and email fetching - no setup needed!

---

## 🚀 Installation

```powershell
copilot plugin marketplace add Supradeep-maq/my-marketplace
copilot plugin install workiq-email-helper@my-mcp-marketplace
```

---

## ✨ Usage

Work IQ MCP automatically connects to your Outlook. Just ask:

```
Summarize my latest email
Extract action items from my last 5 emails
What's the sentiment of my recent emails?
```

---

## 📋 Structure

```
workiq-helper/
├── .mcp.json           # References Work IQ MCP server
├── plugin.json         # Plugin metadata and skills
├── README.md
└── skills/            # AI guidance for using email tools
    ├── email-summary.md
    ├── action-items.md
    └── email-sentiment.md
```

---

## 🔧 How It Works

This plugin simply references the **Work IQ MCP server** (`@microsoft/work-iq-mcp`):
- ✅ Work IQ handles Outlook authentication automatically
- ✅ No Graph API setup needed
- ✅ No custom code - just skills configuration
- ✅ Works out of the box

---

## 🎯 Available Skills

- **email-summary** - Summarize emails
- **action-items** - Extract tasks from emails  
- **email-sentiment** - Analyze email tone

All powered by Work IQ MCP!

---

**License:** MIT
