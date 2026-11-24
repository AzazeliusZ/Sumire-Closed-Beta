# 🌸 すみれ v0.6.8.1-beta.1 — 日本語テスト版

**Windows x64 / 開発中のクローズドベータ（正式版ではありません）**

すみれは、会話・声・表情・記憶を備えたWindows用AIコンパニオンです。このバージョンでは、キャラクターの一貫性、会話スタイルの設定、日本語表示、初回セットアップを中心に改善しました。

## このバージョンの主な内容

- **Sumire Identity：** すみれの基本的な個性を保つ仕組み
- **会話の好み：** 回答の長さ、言葉遣い、説明スタイルなどを設定
- **初回のごあいさつ：** 会話スタイルの設定は保存・スキップ可能
- **日本語 / English / Русский：** 表示言語と回答言語の設定
- **Lavender Night：** ラベンダーを基調にしたUI
- **既存の機能：** クラウド／ローカルAI、長期記憶、音声入力・音声合成、表情とリップシンク、画面認識、翻訳など
- **フィードバック：** sumirehelp@gmail.com

## 配布予定ファイル（Assets）

1. `Sumire_0.6.8.1_Closed_Beta_Portable.zip` — Windows向け本体（約92MiB）
2. `Sumire_0.6.8.1_Closed_Beta_Guide_JA.pdf` — 日本語の機能・動作環境ガイド（5ページ）
3. `SHA256SUMS.txt` — ダウンロードファイルの整合性確認用

配布先：[Releases](https://github.com/AzazeliusZ/Sumire-Closed-Beta/releases)

**注意：GitHubが自動生成する Source code (zip/tar.gz) はアプリ本体ではありません。配布開始後、Assets内のWindows用ZIPをご利用ください。**

## はじめに

ZIPをすべて展開し、`Sumire-0.6.8.1-Closed-Beta/Windows/MyLittleAICompanion.exe` を実行してください。最初は**クラウドAI＋文字チャット**がおすすめです。クラウドのAPIキーは各自でご用意ください。

GPUがなくても基本画面とクラウド文字チャットは試せます。Qwen3-TTSによる音声読み上げや一部ローカルモデルは、高性能なGPU・追加モデル・Python環境が必要です。

**.NETは同梱されていますが、音声モデル・Python環境・ローカルLLMは同梱されていません。** アプリのウィザードで必要な機能を選んでください。

## テストしていただきたい点

日本語の表現、すみれの個性、初期設定の分かりやすさ、各種AIモデルへの接続、音声とGPUの互換性、予期しないクラッシュなど。

📩 不具合・感想：**sumirehelp@gmail.com**（件名：`[Sumire] Bug Report`）

APIキー、パスワード、個人的な会話などは送らないでください。Windows DefenderやSmartScreenを無効にしないでください。未署名の実行ファイルはWindowsで警告される可能性があります。

**このバージョンはテスト用です。すべての構成での動作を保証するものではありません。**
