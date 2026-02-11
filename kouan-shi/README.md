# 光闇詞 (Kouan-shi) — The Hymn of Light and Shadow

光と闇を持つ心の在り方を哲学的に説く『光闇詞』の公式サイトのソースコードです。

**サイト URL**: [https://www.koan-shi.com](https://www.koan-shi.com)

## 技術スタック

- **フレームワーク**: [Astro](https://astro.build/) v5
- **言語**: HTML, CSS, TypeScript
- **i18n**: 日本語 (ja) / 英語 (en) の2言語対応
- **Markdown**: [marked](https://github.com/markedjs/marked) による経典テキストの描画

## ディレクトリ構成

```
src/
├── layouts/
│   └── ScriptureLayout.astro   # 章ページ共通レイアウト
├── content/
│   └── scriptures/             # 経典のMarkdownファイル
│       ├── ja/                 # 日本語版 (prelude/interlude/finale)
│       └── en/                 # 英語版 (prelude/interlude/finale)
└── pages/
    ├── index.astro             # 言語選択ページ
    ├── ja/                     # 日本語ページ群
    │   ├── index.astro         # 章選択
    │   ├── prelude.astro       # 前詞四十節
    │   ├── interlude.astro     # 中詞四節
    │   ├── finale.astro        # 終節
    │   └── about.astro         # このサイトについて
    └── en/                     # 英語ページ群
        ├── index.astro         # Chapter selection
        ├── prelude.astro       # Prelude - 40 Verses
        ├── interlude.astro     # Interlude - 4 Verses
        ├── finale.astro        # Finale
        └── about.astro         # About
```

## セットアップ

```bash
npm install
```

## コマンド

| コマンド            | 説明                                    |
| :------------------ | :-------------------------------------- |
| `npm run dev`       | ローカル開発サーバーを起動 (`localhost:4321`) |
| `npm run build`     | 本番用サイトを `./dist/` にビルド       |
| `npm run preview`   | ビルド結果をローカルでプレビュー        |

## ライセンス

[LICENSE.txt](LICENSE.txt) を参照してください。
