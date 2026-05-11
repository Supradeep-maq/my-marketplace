# Work IQ Email Helper

**Configuration-only MCP plugin** for Work IQ email summarization and action item extraction.

No custom code required - pure configuration!

---

## 🚀 Installation

This plugin is designed to be installed via GitHub Copilot CLI marketplace commands.

### From GitHub

```powershell
# Add the marketplace
copilot plugin marketplace add yourusername/my-marketplace

# Browse available plugins
copilot plugin marketplace browse workiq-helper

# Install the plugin
copilot plugin install workiq-helper
```

---

## ✨ Available Tools

### 1. `summarize_email`
Summarize Work IQ emails or email threads

**Parameters:**
- `email_id` (required): Email ID or thread ID from Work IQ
- `summary_type`: "brief", "detailed", or "action-items"

**Example:**
```
Summarize email ID abc123 from Work IQ
```

### 2. `extract_action_items`
Extract action items and tasks from emails

**Parameters:**
- `email_id` (required): Email ID or thread ID from Work IQ

**Example:**
```
Extract action items from email ID abc123
```

### 3. `get_email_sentiment`
Analyze sentiment and tone of emails

**Parameters:**
- `email_id` (required): Email ID from Work IQ

**Example:**
```
What's the sentiment of email ID abc123?
```

---

## 📋 Configuration

This plugin uses `.mcp.json` for configuration - no code files needed!

All tools are defined declaratively in:
- `.mcp.json` - MCP server configuration
- `plugin.json` - Tool definitions and schemas

---

## 🎯 Usage with Copilot CLI

After installation, use the tools naturally in conversation:

```powershell
copilot "Summarize my Work IQ email ID abc123"
copilot "Extract action items from email thread def456"
copilot "Analyze the sentiment of email ghi789"
```

Or in interactive mode:
```powershell
copilot
> Summarize email abc123 with detailed summary
> Extract action items from email def456
```

---

## 🔧 No Code Required

This plugin demonstrates configuration-only MCP:
- ✅ No Python/Node.js code
- ✅ No dependencies to install
- ✅ Easy to understand and modify
- ✅ Works across platforms
- ✅ Pure JSON/Markdown configuration

---

**License:** MIT
