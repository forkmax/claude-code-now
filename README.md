# 🖥 Claude Code Now

**Launch Claude Code in 3 seconds, save 5 minutes daily** ⚡

**English** | [中文](README.zh.md)

> "Finally, no more typing commands in terminal every time!"

---

## 🎯 What Does It Do?

**Your current workflow:**
```
Open Terminal → Type commands → Wait → Select folder → Confirm → 😰
```

**With Claude Code Now:**
```
Click icon → Start working instantly → ✨
```

**💡 Side-by-side comparison:**
| What | Traditional Way | Claude Code Now |
|------|---------------|-----------------|
| Time needed | ~35s | ~3s |
| Steps required | 5-6 steps | 1 step |

---

## 📦 Available Versions

This fork provides two dedicated versions in addition to the auto-detect version:

| Version | Description | Download |
|---------|-------------|----------|
| **Claude Code Now Terminal** | Always launches in macOS Terminal.app | [Download](./Claude.Code.Now.Terminal.v1.6.4.macOS.zip) |
| **Claude Code Now iTerm2** | Always launches in iTerm2 | [Download](./Claude.Code.Now.iTerm2.v1.6.4.macOS.zip) |

### Why Dedicated Versions?

The original auto-detect version cannot truly detect your system's default terminal. It only:
1. Checks which terminal apps are installed
2. Uses a hardcoded priority (iTerm > Warp > Alacritty > Terminal)
3. Saves the first detected terminal to a config file — never re-checks

**Solution:** Use the dedicated version that matches your preferred terminal.

---

## 🚀 Features

- **🚀 3-Second Launch** - Click and go, no waiting
- **📁 Smart Folder Launch** - Works where you are
- **💾 Remembers Last Location** - Starts where you left off
- **🔧 Permission Mode Fix** - Uses `acceptEdits` instead of `bypass` for full skill access

### 🔧 Key Fix in This Fork

The original version used `--permission-mode bypass` which restricts access to user-installed Claude skills. This fork changes it to `--permission-mode acceptEdits`, allowing full access to all your installed skills.

---

## 📥 Installation

### Option 1: Download Pre-built Apps

1. Download the desired version:
   - [Claude Code Now Terminal](./Claude.Code.Now.Terminal.v1.6.4.macOS.zip)
   - [Claude Code Now iTerm2](./Claude.Code.Now.iTerm2.v1.6.4.macOS.zip)

2. Unzip the file

3. Move the `.app` to `/Applications`:
   ```bash
   mv "Claude Code Now Terminal.app" /Applications/
   ```

4. (Optional) Drag to Dock for quick access

### Option 2: Build from Source

```bash
# Clone this repository
git clone https://github.com/forkmax/claude-code-now.git
cd claude-code-now

# Create the app bundle (manual steps required)
# See source/ directory for the launcher script
```

---

## ❓ Usage

1. **Click the app icon** in Dock or Applications
2. **Or right-click a folder** → "Open With" → Choose the app
3. Claude Code launches instantly in your chosen terminal

---

## 🔧 Configuration

### Terminal Preference

The dedicated versions force their respective terminals:
- **Terminal version** → Always uses Terminal.app
- **iTerm2 version** → Always uses iTerm2

No configuration needed!

---

## 📝 Changelog

See [CHANGELOG.md](./CHANGELOG.md) for full version history.

### v1.6.4 (This Fork)
- ✅ Changed `--permission-mode` from `bypass` to `acceptEdits` for full skill access
- ✅ Added dedicated Terminal version app
- ✅ Added dedicated iTerm2 version app
- ✅ Fixed terminal selection logic issues

---

## 🤝 Contributing

Contributions welcome! Please open an issue or PR.

---

## 📄 License

MIT License

---

## ⭐ Acknowledgments

- Original project: [orange2ai/claude-code-now](https://github.com/orange2ai/claude-code-now)
- Thanks to all contributors!
