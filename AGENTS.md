# Repository Guidelines

## プロジェクト概要
このリポジトリは CalcNote のオンラインヘルプと関連ドキュメントを管理します。主に Markdown を編集し、GitHub Pages で公開される静的コンテンツを更新します。

## Project Structure & Module Organization
- `documents/ja/` と `documents/en/`: 言語別のヘルプ本文。例: `documents/ja/how2use.md`。
- `documents/all/subscription/`: 共通のサブスク説明ページ。
- `docs/`: 公開用の静的サイト資産（`index.html`, `stylesheets/`, `javascripts/`, `privacy_policy/`, `terms/`, `subscription/` など）。
- `images/`: ヘルプで参照する画像。
- `README.md`: 入口と主要リンク。

## Build, Test, and Development Commands
このリポジトリには専用のビルドやテストコマンドはありません。編集後は以下の方法で内容を確認してください。
- Markdown のプレビュー: GitHub かエディタのプレビュー機能を使用。
- 公開サイトのローカル確認: `python -m http.server` を `docs/` で実行してブラウザ確認。

## Coding Style & Naming Conventions
- Markdown は ATX 見出し（`#`）を使用し、見出し階層は飛ばさない。
- 箇条書きは `-` を使用、インデントは 2 スペース。
- ファイル名は小文字スネークケース（例: `custom_extension.md`）。
- 相対リンクを優先し、画像は `images/` 配下を参照。
- 追加・変更は対象言語のフォルダに揃えて反映する。

## Testing Guidelines
自動テストはありません。以下を手動で確認してください。
- 主要ページのリンク切れ（`documents/ja/index.md` など）。
- 画像や埋め込みリンクの表示。
- 同内容の言語間で差分が過剰になっていないか。

## Commit & Pull Request Guidelines
- コミットメッセージは日本語の短い要約で、変更目的が分かる内容にします（例: 「FAQ を更新」「サブスク文言を修正」）。
- PR には変更概要、影響する言語、確認方法を記載。
- ページ構成や見た目に影響する変更はスクリーンショットを添付。

## Localization Notes
新規ページや機能説明の追加時は、対応する言語ページの追加・更新方針を明記してください。対応できない場合は PR 内で理由と今後の対応案を共有してください。
