# 🚀 Installation Guide

Complete guide for installing and using the Work IQ Email Helper plugin from GitHub marketplace.

---

## Prerequisites

- GitHub Copilot CLI installed
- Git and GitHub CLI (`gh`)
- Access to Work IQ

Verify:
```powershell
copilot --version
gh --version
```

---

## 📦 Installation (3 Simple Commands)

### Step 1: Add Marketplace

```powershell
copilot plugin marketplace add yourusername/my-marketplace
```

This registers the marketplace with your Copilot CLI.

---

### Step 2: Browse Plugins

```powershell
copilot plugin marketplace browse workiq-helper
```

This shows you the plugin details before installing.

---

### Step 3: Install Plugin

```powershell
copilot plugin install workiq-helper
```

Done! The plugin is now available in Copilot.

---

## ✅ Verify Installation

```powershell
# List installed plugins
copilot plugin list

# Should show: workiq-helper
```

---

## 🎯 Usage

### Interactive Mode

```powershell
copilot
```

Then use naturally:
```
> Summarize email abc123 from Work IQ
> Extract action items from email def456
> What's the sentiment of email ghi789?
```

### Direct Commands

```powershell
copilot "Summarize my Work IQ email ID abc123"
copilot "Extract action items from email thread def456"
copilot "Analyze sentiment of email ghi789"
```

---

## 🔄 Updating

When the plugin is updated on GitHub:

```powershell
copilot plugin update workiq-helper
```

---

## 🗑️ Uninstalling

```powershell
copilot plugin uninstall workiq-helper
```

---

## 📍 What Gets Installed

The plugin is pure configuration - no code!

**Files:**
- `.mcp.json` - MCP server configuration
- `plugin.json` - Tool definitions

**Location:** Managed by Copilot CLI (usually in `~/.copilot/plugins/`)

---

## 🆘 Troubleshooting

### Plugin not found

**Issue:** `copilot plugin install workiq-helper` fails

**Solution:**
1. Make sure you added the marketplace:
   ```powershell
   copilot plugin marketplace add yourusername/my-marketplace
   ```
2. Replace `yourusername` with the actual GitHub username

---

### Tools not available

**Issue:** Copilot doesn't recognize email summarization tools

**Solution:**
1. Verify installation:
   ```powershell
   copilot plugin list
   ```
2. Try restarting your terminal
3. Be explicit: "Use the summarize_email tool for email abc123"

---

### Marketplace URL invalid

**Issue:** Can't add marketplace

**Solution:**
Make sure the repository is public and exists:
```powershell
gh repo view yourusername/my-marketplace
```

---

## 🌐 For Deployers

If you're deploying this marketplace:

### 1. Push to GitHub

```powershell
cd "c:\Users\v-rsupradeep\Music\Test plugin"
git init
git add .
git commit -m "Initial commit"
gh repo create my-marketplace --public --source=. --push
```

### 2. Update URLs

Edit `marketplace.json`:
```json
{
  "repository": "https://github.com/YOUR_USERNAME/my-marketplace"
}
```

Then:
```powershell
git add marketplace.json
git commit -m "Update repository URL"
git push
```

### 3. Share

Tell your team:
```powershell
copilot plugin marketplace add YOUR_USERNAME/my-marketplace
copilot plugin install workiq-helper
```

---

## 💡 Available Tools

| Tool | Description | Example |
|------|-------------|---------|
| `summarize_email` | Summarize emails or threads | "Summarize email abc123" |
| `extract_action_items` | Extract tasks and action items | "Extract action items from email def456" |
| `get_email_sentiment` | Analyze email sentiment and tone | "What's the sentiment of email ghi789?" |

---

## ✨ Key Benefits

- ✅ **No Code** - Pure configuration
- ✅ **No Dependencies** - Nothing to install except the plugin
- ✅ **Easy Updates** - Edit config, push, users update
- ✅ **Portable** - Works on any machine with Copilot CLI

---

**You're all set!** Start summarizing Work IQ emails with Copilot. 🎉
