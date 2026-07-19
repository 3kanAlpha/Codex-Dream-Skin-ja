# Codex Dream Skin 日本語化

<a href="./README.zh.md">本家README</a>（中国語）

## 変更点

- タスクトレイのメニュー日本語化
- フォントの変更を無効化

## 動作に必要な環境

- Windows PowerShell 5.1以降
- Node.js 22以降

ChatGPTアプリは一度起動して初期設定を作成しておく必要があります。

## インストール手順

ChatGPTアプリを終了してから実行してください。管理者としてPowerShellを起動する必要はありません。

```powershell
powershell.exe -NoProfile -ExecutionPolicy Bypass `
  -File .\windows\scripts\install-dream-skin.ps1
```

インストーラーは次の処理を行います。

- ChatGPTアプリがインストールされているか確認する
- Node.jsのバージョンを確認する
- 実行ファイルを`%LOCALAPPDATA%\CodexDreamSkin\engine`へコピーする
- Codexの外観設定をバックアップする
- デスクトップとスタートメニューにショートカットを作成する
- システムトレイを起動する
