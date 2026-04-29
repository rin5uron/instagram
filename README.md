---
project: SNS運用プロジェクト
last_updated: "2026-04-29"
---

# SNS運用プロジェクト マスターダッシュボード

## プラットフォーム一覧

| プラットフォーム | アカウント | コード | 状態 |
|---|---|---|---|
| Instagram | ringo__note（栄養士） | `[RN]` | 運用中 |
| Instagram | ringonote_ai（AIスキル） | `[AI]` | 運用中 |
| YouTube | ringonote22@gmail.com | `[YT]` | 準備中 |
| YouTube Shorts | 同上 | `[YT]` | Instaストック後に開始 |
| TikTok | 未設定 | `[TK]` | YouTube本編後に開始 |

## 投稿フロー

```
短尺: ringo-note / ringonote-ai Instagram
        ↓ ストック溜まり次第
      YouTube Shorts へ流用

長尺: YouTube本編
        ↓ 公開後
      TikTok へ流用
```

---

## 投稿ワークフロー

1. **台本生成** → [templates/video-script-format.md](templates/video-script-format.md) を使用
2. **撮影・編集・投稿**
3. **issueで振り返り** → 再生数が出たらissueに記録

---

## 投稿一覧

### ringo-note（栄養士）→ [詳細](ringo-note/README.md)

| # | タイトル | 状態 | 投稿日 | 再生数 |
|---|---|---|---|---|
| [001](ringo-note/posts/001/README.md) | キャベツしかない時の美肌焼きそば | published | 2026-04-21 | 128 |
| [002](ringo-note/posts/002/README.md) | 蒸した芋たちの3日後 | published | 2026-04-22 | 61 |
| [003](ringo-note/posts/003/README.md) | ChatGPTとクッキング・フレンチトースト | published | 2026-04-25 | 計測中 |
| [004](ringo-note/posts/004/README.md) | 家にあるスパイス、眠ってない？ | in-progress | 未定 | - |

### ringonote-ai（AIスキル）→ [詳細](ringonote-ai/README.md)

| # | タイトル | 状態 | 投稿日 | 再生数 |
|---|---|---|---|---|
| [001](ringonote-ai/posts/001/README.md) | 動くプロフィール画像 | published | 2026-04-29 | 122(v1) |
| [002](ringonote-ai/posts/002/script.md) | 動くプロフの作り方 | in-progress | 未定 | - |

### YouTube → [詳細](youtube/README.md)

| # | タイトル | 状態 | 公開日 |
|---|---|---|---|
| - | 未投稿 | - | - |

---

## issueルール

| アカウント | コード | 例 |
|---|---|---|
| ringo-note | `[RN]` | `[RN] 004 振り返り` |
| ringonote-ai | `[AI]` | `[AI] 001 振り返り` |
| YouTube | `[YT]` | `[YT] ep001 まとめ` |
| TikTok | `[TK]` | `[TK] ep001 流用` |
| 設計・共通 | `[設計]` | `[設計] サムネルール` |

- 日付は**本文1行目**に `**日付:** YYYY-MM-DD` で記載

---

## リポジトリ構成

```
/
├── README.md                    # このファイル（マスターダッシュボード）
├── design/                      # 共通デザインルール
│   ├── thumbnail-rules.md
│   └── screenshots/
├── templates/                   # 台本テンプレート
├── ringo-note/                  # Instagram（栄養士）
│   ├── README.md
│   └── posts/NNN/
│       ├── README.md
│       ├── script.md
│       └── assets/
├── ringonote-ai/                # Instagram（AIスキル）+ YouTube Shorts
│   ├── README.md
│   └── posts/NNN/
│       ├── README.md
│       ├── script-vN.md
│       └── assets/
└── youtube/                     # YouTube本編 → TikTok流用
    ├── README.md
    └── episodes/NNN/
        ├── README.md
        ├── script.md
        └── assets/
```

---

## 関連issue

| issue | 内容 |
|---|---|
| #13 | [RN] コンセプト再設計 |
| #14 | [設計] サムネ・フックルール |
| #15 | [設計] リポジトリ構成・issueルール確定 |
