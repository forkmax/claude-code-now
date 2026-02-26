# 🖥 Claude Code Now

**3秒でClaude Code起動、毎日5分節約** ⚡

[English](README.md) | [中文](README.zh.md) | **日本語**

> "ついに毎回ターミナルでコマンドを入力する必要がなくなった！"

---

## 🎯 何ができるの？

**現在の作業フロー：**
```
ターミナル開く → コマンド入力 → 待機 → フォルダ選択 → 確認 → 😰
```

**Claude Code Nowを使えば：**
```
アイコンクリック → すぐに作業開始 → ✨
```

**💡 比較表：**
| 項目 | 従来の方法 | Claude Code Now |
|------|----------|-----------------|
| 所要時間 | ~35秒 | ~3秒 |
| 操作回数 | 5-6回 | 1回 |

---

## 📦 入手可能なバージョン

このフォークは以下の2つの専用バージョンを提供します：

| バージョン | 説明 | ダウンロード |
|---------|-------------|----------|
| **Claude Code Now Terminal** | 常にmacOS Terminal.appで起動 | [ダウンロード](https://github.com/forkmax/claude-code-now/releases/latest/download/Claude.Code.Now.Terminal.v1.6.4.macOS.zip) |
| **Claude Code Now iTerm2** | 常にiTerm2で起動 | [ダウンロード](https://github.com/forkmax/claude-code-now/releases/latest/download/Claude.Code.Now.iTerm2.v1.6.4.macOS.zip) |

### 専用バージョンが必要な理由

元の自動検出バージョンは、システムデフォルトのターミナルを本当に検出することはできません。以下のことしかできません：
1. どのターミナルアプリがインストールされているか確認
2. 固定の優先順位を使用（iTerm > Warp > Alacritty > Terminal）
3. 初めて検出したターミナルを設定ファイルに保存 - 再検出しない

**解決策：** お好みのターミナルに一致する専用バージョンを使用してください。

---

## 🚀 機能

- **🚀 3秒起動** - クリックだけで開始、待ち時間なし
- **📁 スマートフォルダ起動** - いる場所で起動
- **💾 前回の場所を記憶** - 前回いた場所から開始
- **🔧 許可モードを修正** - `bypass` の代わりに `acceptEdits` を使用してフルスキルアクセス

### 🔧 このフォークの重要な修正

元のバージョンは `--permission-mode bypass` を使用しており、これはユーザーインストールしたClaudeスキルへのアクセスを制限していました。このフォークでは `--permission-mode acceptEdits` に変更し、インストールしたすべてのスキルへのフルアクセスを可能にしています。

---

## 📥 インストール

1. お好みのバージョンをダウンロード：
   - [Terminalバージョン](https://github.com/forkmax/claude-code-now/releases/latest/download/Claude.Code.Now.Terminal.v1.6.4.macOS.zip)
   - [iTerm2バージョン](https://github.com/forkmax/claude-code-now/releases/latest/download/Claude.Code.Now.iTerm2.v1.6.4.macOS.zip)

2. ファイルをアーカイブ解除

3. `.app` を `/Applications` に移動：
   ```bash
   mv "Claude Code Now Terminal.app" /Applications/
   ```

4. （オプション）Dockにドラッグしてクイックアクセス

---

## ❓ 使い方

1. **Dockまたはアプリケーションのアイコンをクリック**
2. **またはフォルダを右クリック** → "開く" → アプリを選択
3. 選択したターミナルでClaude Codeが即座に起動

---

## 📝 変更履歴

完全なバージョ履歴は [CHANGELOG.md](./CHANGELOG.md) をご覧ください。

### v1.6.4（このフォーク）
- ✅ `--permission-mode` を `bypass` から `acceptEdits` に変更し、フルスキルアクセスを提供
- ✅ 専用Terminalバージョンアプリを追加
- ✅ 専用iTerm2バージョンアプリを追加

---

## 🤝 コントリビューション

コントリビューション大歓迎！IssueまたはPRを開いてください。

---

## 📄 ライセンス

MITライセンス

---

## ⭐ 謝辞

- 元プロジェクト：[orange2ai/claude-code-now](https://github.com/orange2ai/claude-code-now)
- すべてのコントリビューターに感謝！
