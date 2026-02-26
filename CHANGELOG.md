# Changelog

All notable changes to this project will be documented in this file.

---

## [1.6.4] - 2025-02-26

### Added
- **Claude Code Now Terminal.app** - Dedicated version that always launches in macOS Terminal.app
- **Claude Code Now iTerm2.app** - Dedicated version that always launches in iTerm2

### Changed
- **Permission Mode Fix**: Changed `--permission-mode` from `bypass` to `acceptEdits`
  - This allows Claude Code to access all user-installed skills
  - The original `bypass` mode restricted access to external skills for safety, but was too restrictive

### Fixed
- Terminal auto-detection now uses dedicated versions instead of unreliable config-based detection
- Users can now choose their preferred terminal without worrying about config file issues

---

## [1.6.3] - Original (Reference)

### Original Features
- 3-second launch time
- Smart folder launch
- Remembers last location
- Dock integration
- Right-click "Open With" support

---

## Installation Notes

### For Terminal Users
Download: [Claude.Code.Now.Terminal.v1.6.4.macOS.zip](./Claude.Code.Now.Terminal.v1.6.4.macOS.zip)

### For iTerm2 Users  
Download: [Claude.Code.Now.iTerm2.v1.6.4.macOS.zip](./Claude.Code.Now.iTerm2.v1.6.4.macOS.zip)
