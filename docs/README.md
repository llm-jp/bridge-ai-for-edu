# BRIDGE教育AI — プロジェクトサイト

このディレクトリ（`docs/`）は、GitHub Pages で公開されるプロジェクトサイトのソースです。
[Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) テーマ（remote theme）を使用しています。

公開URL: https://llm-jp.github.io/bridge-ai-for-edu/

## ディレクトリ構成

```
docs/
├── _config.yml            # サイト全体の設定
├── _data/
│   └── navigation.yml     # ヘッダー／サイドバーのメニュー
├── _pages/                # 各固定ページ
│   ├── research.md         # 研究概要
│   ├── roadmap.md          # 実施計画・KPI
│   ├── outcomes.md         # 出口戦略・社会実装
│   ├── organizations.md    # 実施体制（一覧）
│   ├── org-nii.md          # 国立情報学研究所（NII）
│   ├── org-kyoto.md        # 京都大学
│   ├── org-osaka.md        # 大阪教育大学
│   ├── news.md             # ニュース一覧
│   ├── members.md          # メンバー
│   └── publications.md     # 研究業績
├── _posts/                # ニュース記事（YYYY-MM-DD-タイトル.md）
├── assets/
│   ├── css/main.scss       # カスタムスタイル
│   └── images/logo.png     # ロゴ
├── index.md               # トップページ
└── Gemfile
```

## 進捗（ニュース）の追加方法

`_posts/` に `YYYY-MM-DD-任意の名前.md` というファイル名で記事を追加します。
トップページとニュース一覧に自動的に反映されます。

```markdown
---
title: "記事のタイトル"
date: 2026-08-01
categories:
  - お知らせ      # 例: お知らせ / 研究成果 / イベント
tags:
  - タグ
---

本文をここに書きます。
```

## メンバーの追加方法

- 各機関ページ（`_pages/org-*.md`）と `_pages/members.md` の表に行を追加します。

## ローカルでの確認（任意）

```bash
cd docs
bundle install
bundle exec jekyll serve
# http://localhost:4000/bridge-ai-for-edu/ で確認
```

## GitHub Pages の公開設定

リポジトリの Settings → Pages で、Source を「Deploy from a branch」、
Branch を `main`（または該当ブランチ）の `/docs` フォルダに設定してください。
