# MyVoice Studio — 配布と更新情報

Apple Silicon Mac向けのローカル音声合成アプリです。ここには公開配布物とリリース情報だけを置きます。開発用ソースコードは非公開で管理しています。

## v0.2.0 開発プレビュー

この版には声の登録、Qwen3-TTS Base用の推論アダプター、原稿の読み上げ画面、生成履歴、アプリアイコン、手動の更新確認が含まれます。**Qwen3-TTSの実モデルによる日本語音声生成は未検証です。完成版ではありません。** Apple Developer IDでの署名・公証も行っていません。

アプリZIPにPython、MLX Audio、FFmpeg、音声モデルは含まれません。Apple Silicon MacとmacOS 14以降が必要です。初回に `brew install python@3.12 ffmpeg` を実行し、アプリ内の `Contents/Resources/scripts/setup_runtime.sh` でMLX Audioをインストールしてください。その後、アプリの設定画面からQwen3-TTS Baseモデルを取得します。これらの準備にはネットワーク接続が必要です。推論時はローカル処理です。

音声ファイル、モデル、生成履歴はMac内に保存され、この公開リポジトリには含まれません。アプリ内の「更新を確認」はこのリポジトリのリリース情報だけを読みます。
