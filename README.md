<div align="center">

# 🌸 すみれ — My Little AI Companion

**最新版：0.6.9 Closed Beta**

Easy Setup & Community Feedback · Windows x64

[日本語](docs/v0.6.9/README-JA.md) · [English](docs/v0.6.9/README-EN.md) · [Русский](docs/v0.6.9/README-RU.md)

**開発中のテスト版です。正式リリースではありません。**

[リリース一覧](https://github.com/AzazeliusZ/Sumire-Closed-Beta/releases) · [初回起動ガイド](docs/v0.6.9/START-HERE-JA.md) · [リリースノート](docs/v0.6.9/RELEASE-NOTES-JA.md)

</div>

---

## 最新版をダウンロード

- **[Windows x64 版（Portable ZIP）](https://github.com/AzazeliusZ/Sumire-Closed-Beta/releases/download/v0.6.9-beta.1/Sumire_0.6.9_Closed_Beta_Portable.zip)** · [SHA-256](https://github.com/AzazeliusZ/Sumire-Closed-Beta/releases/download/v0.6.9-beta.1/SHA256SUMS.txt)
- [日本語の導入手順](docs/v0.6.9/INSTALL-JA.md) · [動作環境](docs/v0.6.9/SYSTEM-REQUIREMENTS-JA.md) · [テスター向けのご案内](docs/v0.6.9/TESTERS-JA.md) · [日・英・露のドキュメント（ZIP）](https://github.com/AzazeliusZ/Sumire-Closed-Beta/releases/download/v0.6.9-beta.1/Sumire_0.6.9_Documentation_JA_EN_RU.zip)
- [0.6.9 のリリースページ](https://github.com/AzazeliusZ/Sumire-Closed-Beta/releases/tag/v0.6.9-beta.1)

## 今回のアップデート

日本の初期テスターの皆さまから寄せられたご意見をもとに、初回設定と使いやすさを改善しました。

1. **Automatic Setup：** 既存の Ollama・LM Studio を検出。必要な場合は、確認のうえで公式の Ollama インストーラーを起動できます。LM Studio の導入は手動です。
2. **Hardware Advisor：** RAM、専用 VRAM、ディスクの空き容量からモデル候補を提案。
3. **Easy Setup：** クラウド AI、ローカル AI、手動設定から選択。
4. **Voice Studio Lite：** Qwen3-TTS の声と日・英・露のサンプルを試聴。標準の声は Ono_Anna。
5. **GitHub Update Checker：** 新しいリリースを確認。EXE の自動更新は行いません。
6. **診断センター：** コンポーネントを確認し、必要に応じて音声環境を修復。
7. **API 接続テスト：** 接続、認証、モデル設定を確認。クラウドのテストは課金される場合があります。
8. **リソース管理：** メモリ使用状況の確認と、対応するモデルやコンポーネントの手動解放。
9. **フィードバック：** 選択した技術情報をプレビューし、診断レポートを端末に保存。自動送信はありません。

## すみれについて

すみれ（Sumire / すみれ）は、会話・音声・表情・記憶を備えた、Windows用のAIコンパニオンです。クラウドAIにもローカルAIにも対応しています。明るく親しみやすい基本のキャラクターを大切にしながら、話し方や回答の長さなどを好みに合わせて設定できます。

この版は、日本語での使いやすさと、初期設定・PC互換性の確認を目的としたクローズドベータ版です。開発者が案内したテスター向けの配布ページであり、動作を保証する正式版ではありません。

## 主な機能

| 機能 | 説明 | 追加で必要なもの |
|---|---|---|
| 💬 文字チャット | 雑談、質問、文章作成。クラウドまたはローカルLLMを利用 | クラウド：ネット接続・対応APIキー／ローカル：別途LLM環境 |
| 🌸 個性と会話スタイル | すみれの基本的な個性を保ちながら、言葉遣いや回答の長さを調整 | 追加ハードウェア不要 |
| 🧠 長期記憶 | 保存した情報の参照・編集・削除 | 利用者自身による設定・管理 |
| 😊 表情・口の動き | アニメーション、感情表現、読み上げ時のリップシンク | 音声に合わせた口の動きにはTTS設定が必要 |
| 🎤 音声入力 | Faster-Whisperを使ったマイク入力 | マイク・Python環境・音声認識モデル |
| 🔊 音声読み上げ | Qwen3-TTSによる音声生成（Ono_Annaなど） | 対応GPU、Python環境・音声モデル |
| 👁️ 画面認識 | 許可された画面を画像対応AIで解析 | 利用者の許可・ローカルVLM |
| 🌐 その他 | 翻訳機能、Discord音声連携 | 機能によって追加設定が必要 |

**文字チャットだけなら高性能なNVIDIA GPUは必要ありません。** 最初は「クラウドAI＋文字チャット」でお試しください。

## 動作環境の目安

下記は 0.6.9 ベータ版の推奨目安です。セットアップから Ollama を導入する場合は x64 版 Windows 10 22H2 以降が必要です。Windows 実機での初回起動、Ollama の導入、CUDA、音声入出力、既存プロファイルの移行は引き続き検証が必要です。

| 項目 | 目安 | 理由 |
|---|---|---|
| OS | Windows 10 64bit（ビルド19041以降）／Windows 11 64bit | Windows用WPFアプリのため |
| CPU | x64プロセッサー | アプリ本体に必要。音声認識のCPUモードにはAVX対応も必要 |
| RAM | 8GB以上を推奨 | 基本動作・クラウド文字チャット。ローカルモデル利用時は増える |
| GPU | クラウド文字チャットには専用GPU不要 | 文章生成はクラウド側で実行されるため |
| 空き容量 | アプリ展開用に約 500 MiB／Ollama、モデル、音声環境は別途必要 | Python、追加パッケージ、AIモデルを別途ダウンロードするため |
| インターネット | クラウド利用時・初回ダウンロード時に必要 | API接続とモデル取得のため |

### GPUがない場合でも使える？

**はい。** 文字チャットとアプリの基本画面は、高性能なNVIDIA GPUがなくても利用を試せます。

- **クラウドAIでの文字会話：** 専用GPU不要。APIキーとネット接続を用意します。
- **ローカルLLM：** CPUで動かせる小型モデルもありますが、RAMと応答速度はモデルによって異なります。
- **音声入力（Faster-Whisper）：** CPUモードならNVIDIA GPUなしでも試せます。Baseモデルなら8GB RAM、Smallモデルなら12～16GB RAMを目安にしてください。
- **音声読み上げ（Qwen3-TTS）：** 現行の自動セットアップはCUDA/BF16対応NVIDIA GPU中心です。参考目安は0.6BモデルでVRAM 6～8GB、1.7Bモデルで8GB以上。AMD Radeon・Intel GPUでの自動導入は保証していません。
- **画面認識：** 別途設定するVLMの要件によります。画面取得には利用者の許可が必要です。

**音声モデル、Python環境、ローカルLLMのモデルデータは配布ZIPに含まれていません。** 利用する機能だけを追加してください。

## ダウンロードと初回起動

上のリンクから Windows 用 ZIP を取得し、必要に応じて日本語の導入手順を参照してください。GitHubが自動生成するSource codeはアプリ本体ではありません。

1. ZIPをすべて展開してください。EXEだけを取り出さないでください。
2. 展開先の `Sumire-0.6.9-Closed-Beta/Windows/MyLittleAICompanion.exe` を起動します。.NETランタイムは同梱されています。
3. 表示言語を設定し、クラウド AI、ローカル AI、手動設定から選びます。最初はクラウドのテキスト会話がおすすめです。API キーは各自で用意し、開発者に送らないでください。ローカルの場合は、既存の Ollama または LM Studio を検出するか、セットアップから Ollama を導入できます。
4. 最後の画面で会話の好みを保存するか、スキップできます。あとから設定で変更できます。
5. 必要に応じて音声・画面認識を追加設定します。モデル、Ollama、LM Studio、Python 環境は同梱されていません。更新する場合は旧アプリを終了し、新しい ZIP を別のフォルダーへ展開してください。詳しくは[導入・復旧手順](docs/v0.6.9/INSTALL-JA.md)をご覧ください。

Windowsのセキュリティ機能を無効にしないでください。未署名アプリは警告が表示される可能性があります。入手元を確認できない場合は実行せず、開発者にお問い合わせください。

## 安全性とプライバシー

- 配布用ZIPは開発者個人のAPIキー、会話履歴、長期記憶、C#ソースコードを含めない構成です。
- クラウドAI利用時には会話テキストが選択したサービスへ送られます。機密情報は入力しないでください。
- 画面認識は許可が必要です。診断レポートにチャット履歴、記憶、API キー、音声、画面画像は含まれません。メールへのログ・画像の自動添付や送信は行いません。
- ベータ版のため未発見の不具合があります。初期設定、音声、GPU互換性などはPCごとに動作が異なります。
- SHA-256は [0.6.9 の SHA256SUMS.txt](https://github.com/AzazeliusZ/Sumire-Closed-Beta/releases/download/v0.6.9-beta.1/SHA256SUMS.txt) で確認できます。

## 感想・不具合報告

日本語の自然さ、キャラクターの一貫性、初期設定の分かりやすさ、GPU・音声まわりの不具合など、率直な感想をお寄せください。

📩 **Sumire Developer — [sumirehelp@gmail.com](mailto:sumirehelp@gmail.com)** · [GitHub Issues](https://github.com/AzazeliusZ/Sumire-Closed-Beta/issues)  
件名の例：`[Sumire] Bug Report` / `[Sumire] Feature Suggestion`

不具合報告では、Windowsのバージョン、CPU・GPU・RAM、再現手順、表示されたエラーメッセージを教えてください。**APIキー、パスワード、プライベートな会話、個人情報入りのスクリーンショットは送らないでください。**

---

## 以前のバージョン

- [0.6.8.1 Closed Beta（v0.6.8.1-beta.1）](https://github.com/AzazeliusZ/Sumire-Closed-Beta/releases/tag/v0.6.8.1-beta.1)：Windows ZIP、日本語 PDF、SHA-256。
- 0.6.8.1 の資料：[初回起動ガイド](START-HERE-JA.md) · [リリースノート](RELEASE_NOTES_JA.md) · [SHA-256](SHA256SUMS.txt)

---

**開発状況：** 0.6.9 / Closed Beta / Windows x64  
**コードについて：** この配布用リポジトリではC#ソースコードを公開していません。各外部ライブラリのライセンス情報はアプリのZIP内をご覧ください。
