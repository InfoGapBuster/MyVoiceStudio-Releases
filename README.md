# MyVoice Studio — 配布と更新情報

Apple Silicon Mac向けのローカル音声合成アプリです。ここには公開配布物とリリース情報だけを置きます。開発用ソースコードは非公開で管理しています。

## v0.3.0-preview.1 開発プレビュー

声の登録、Qwen3-TTS BaseとCosyVoice 3のモデル取得・読み上げ、生成履歴、アプリアイコン、「MyVoice Studioとは」メニュー、手動の更新確認を含みます。実モデルによる日本語音声生成はまだ検証できていません。Apple Developer ID署名と公証も未実施です。

ZIPにはPython、MLX Audio、FFmpeg、音声モデルを含めません。Apple Silicon MacとmacOS 14以降が必要です。初回に `brew install python@3.12 ffmpeg` を実行し、アプリ内の `Contents/Resources/scripts/setup_runtime.sh` で基本のMLX実行環境を導入してください。その後、アプリの設定画面からモデルを取得します。CosyVoice 3を取得すると、専用の実行環境と音声トークナイザーも導入されます。

音声ファイル、モデル、生成履歴はMac内に保存され、この公開リポジトリには含まれません。アプリ内の「更新を確認」はこのリポジトリのリリース情報だけを読みます。
