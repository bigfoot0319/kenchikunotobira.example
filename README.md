# 建築のトビラ - 公式Webサイト

建築の世界への新しい扉を開くラジオ番組「建築のトビラ」の公式Webサイトです。

## 番組概要

- **放送開始**: 2026年1月4日（日）
- **放送時間**: 毎週日曜 11:00〜11:55
- **配信**: ミュージックバード、Spotify、YouTube
- **パーソナリティ**: 田中知子
- **制作協力**: 大阪府建築士事務所協会

## サイト構成

このサイトは以下のセクションで構成されています：

- Hero（メインビジュアル）
- Episodes（エピソード紹介）
- About（番組について）
- Cast（出演者紹介）
- Broadcast（放送情報）
- Pillars（番組の柱）
- Contents（コンテンツ紹介）
- Schedule（スケジュール）
- Stations（放送局一覧）
- Association（協会について）
- Sponsors（スポンサー）
- Contact（お問い合わせ）

## 技術スタック

- **HTML5** - セマンティックなマークアップ
- **Tailwind CSS v4.1** - CDN版を使用したユーティリティファーストCSS
- **Animate.css v4.1.1** - アニメーション効果
- **AOS v2.3** - スクロールアニメーション
- **Lucide Icons** - アイコン
- **Google Fonts** - Noto Sans JP

## ファイル構成

```
kenchikunotobira.example.jp/
├── public/              # 公開用ディレクトリ
│   ├── index.html       # メインページ
│   └── assets/          # 静的ファイル
│       ├── css/         # スタイルシート
│       ├── js/          # JavaScript
│       └── images/      # 画像
├── project-docs/        # プロジェクト関連ドキュメント
├── dev-tools/           # 開発ツール
│   ├── unsplash-search.js
│   └── README.md
├── CLAUDE.md            # Claude Code用指示書
└── README.md            # このファイル
```

## ローカル開発

1. **リポジトリをクローン**
   ```bash
   git clone <repository-url>
   cd kenchikunotobira.example.jp
   ```

2. **依存パッケージをインストール**
   ```bash
   npm install
   ```

3. **ローカルサーバーを起動**
   - VS Code の Live Server 拡張機能を使用
   - または任意のローカルサーバーで `public/` ディレクトリを公開

## デプロイ

Cloudflare Pages でのデプロイを推奨します：

1. Cloudflare にログイン
2. Workers & Pages を選択
3. 「アプリケーションを作成」→「Pages」タブ
4. Git リポジトリをインポート
5. 公開フォルダに `public` を設定
6. デプロイ実行

## 画像取得（開発用）

Unsplash API を使用して高品質な画像を検索できます：

```bash
node dev-tools/unsplash-search.js "建築"
```

※ 使用には Unsplash API キーが必要です。環境変数 `UNSPLASH_ACCESS_KEY` または `.env.local` ファイルで設定してください。

## ライセンス

All Rights Reserved - 建築のトビラ制作委員会
