# PROJECT: wit-teishutsu-kun

## 概要
- 目的：プリント提出（撮影/トリミング/補正/OCR/提出ログ）
- 形態：Google Apps Script（Webアプリ）＋ Drive（画像）＋ Sheet（ログ）＋ OCR（連携）

## 重要リンク（あとで埋める）
- GitHub（正本）：https://github.com/wit-ai-apps/wit-teishutsu-kun
- GAS編集URL：
- 配布URL（必ず ?b=BUILD_ID）：
- ログ用スプレッドシート：
- Driveフォルダ（提出画像）：
- OCR/APIキー（保存場所メモ）：※キー自体は書かない

## UI凍結ルール（最重要）
- UI（見た目）は完全固定（変更禁止）
  - HTML構造 / 文言 / 配置 / サイズ / 色 / 余白 / クラス名
- 変更してよいのは「内部処理（ロジック）」のみ
- UI差分が出たら **差し戻し優先**
- 例外を作る場合：なべさんの明示許可がある時だけ

## 依頼文の固定フレーズ（Rex/Gemini/ユイ共通）
依頼の先頭に必ず書く：
> UI凍結で、中身だけ。UI差分が出たら差し戻し。

## 版管理ルール（固定）
- VERSION：vX.Y.Z
- BUILD_ID：YYYY-MM-DD_HHMM_<tag>
- 配布URL：必ず `?b=BUILD_ID`（検証のみ `&debug=1`）
