# My MCP Marketplace - Work IQ Email Helper

**Configuration-only MCP marketplace** - No custom code required!

This marketplace contains plugins that work purely through configuration files. Perfect for teams that want simple, maintainable tools without managing codebases.

---

## 🚀 Quick Start (3 Commands)

```powershell
# 1. Add this marketplace
copilot plugin marketplace add yourusername/my-marketplace

# 2. Browse plugins
copilot plugin marketplace browse workiq-helper

# 3. Install
copilot plugin install workiq-helper
```

**That's it!** Start using it immediately with Copilot CLI.

---

## 📦 Available Plugins

### Work IQ Email Helper
Summarize emails and extract action items from Work IQ

**Tools:**
- `summarize_email` - Summarize emails or threads
- `extract_action_items` - Extract tasks and action items
- `get_email_sentiment` - Analyze email sentiment

**Usage:**
```powershell
copilot "Summarize my Work IQ email ID abc123"
copilot "Extract action items from email def456"
```

---

## 📁 Repository Structure

```
my-marketplace/
├── marketplace.json                    # Plugin registry
├── README.md                          # This file
└── plugins/
    └── workiq-helper/
        ├── .mcp.json                  # MCP configuration (config only!)
        ├── plugin.json                # Tool definitions (config only!)
        └── README.md                  # Plugin docs
```

**No code files!** Everything is JSON configuration.

---

## 🎯 Why Configuration-Only?

- ✅ **No Dependencies** - No npm install, no pip install
- ✅ **Easy to Understand** - Just JSON files
- ✅ **Easy to Modify** - Edit config, push to GitHub
- ✅ **Works Everywhere** - No runtime requirements
- ✅ **Team-Friendly** - Anyone can read and update configs

---

## 🌐 Deployment to GitHub

### Step 1: Create Repository

```powershell
cd "c:\Users\v-rsupradeep\Music\Test plugin"
git init
git add .
git commit -m "Initial commit: Work IQ Email Helper plugin"
gh repo create my-marketplace --public --source=. --push
```

### Step 2: Update URLs

Edit [marketplace.json](marketplace.json) and replace `yourusername` with your GitHub username:

```json
{
  "repository": "https://github.com/YOUR_GITHUB_USERNAME/my-marketplace"
}
```

Then commit and push:
```powershell
git add marketplace.json
git commit -m "Update repository URL"
git push
```

### Step 3: Share with Team

Your team can now install with:
```powershell
copilot plugin marketplace add YOUR_GITHUB_USERNAME/my-marketplace
copilot plugin install workiq-helper
```

---

## 💡 Usage Examples

After installation, use naturally in Copilot:

```powershell
# Interactive mode
copilot
> Summarize email abc123 from Work IQ
> Extract action items from that email
> What's the sentiment?

# One-shot commands
copilot "Give me a detailed summary of email abc123"
copilot "List all action items from email thread def456"
copilot "Analyze sentiment of email ghi789"
```

---

## 🔧 Customization

Want to add more tools or modify behavior? Just edit the config files:

1. Edit `.mcp.json` to add/modify tools
2. Edit `plugin.json` to update tool schemas
3. Commit and push to GitHub
4. Users run `copilot plugin update workiq-helper`

No code changes needed!

---

## 📚 Documentation

- **[Plugin README](plugins/workiq-helper/README.md)** - Detailed plugin documentation
- **[MCP Protocol](https://modelcontextprotocol.io)** - Official MCP docs

---

## 🤝 Contributing

Want to add more plugins? Just:

1. Create a new folder under `plugins/`
2. Add `.mcp.json` and `plugin.json` (configuration only!)
3. Update `marketplace.json`
4. Submit a pull request

Keep it configuration-only - no code!

---

**License:** MIT
