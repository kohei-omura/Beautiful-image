# ⚡ AI Image Enhancer

ESRGAN（TensorFlow.js + UpscalerJS）によるブラウザ完結型の超解像・高画質化アプリ。

## ✨ 機能

- 🔬 AIによるぼかし除去 & 超解像（×2 / ×3 / ×4）
- 🖥️ ブラウザ完結（画像はサーバーに送信されません）
- 📊 Before / After スライダー比較
- ⬇️ PNG形式でダウンロード
- 📱 スマホ・PCどちらも対応

## 🚀 GitHub Pagesでの公開手順

1. このリポジトリをGitHubにpush
2. Settings → Pages → Source: **GitHub Actions** を選択
3. `main`ブランチにpushするたびに自動デプロイ
4. `https://<あなたのユーザー名>.github.io/<リポジトリ名>/` でアクセス可能

## 📁 ファイル構成

```
/
├── index.html              # メインアプリ
├── .github/
│   └── workflows/
│       └── deploy.yml      # GitHub Pages 自動デプロイ
└── README.md
```

## 🛠️ 使用技術

| ライブラリ | バージョン | 用途 |
|---|---|---|
| TensorFlow.js | 4.17.0 | AI推論エンジン |
| UpscalerJS | 1.0.0-beta.18 | ESRGAN超解像 |
| ESRGAN Medium | CDN | 超解像モデル |

## ⚠️ 注意事項

- 初回実行時はモデルのダウンロードに数十秒かかります
- 大きな画像は処理に時間がかかります（推奨: 500px以下）
- スマホではメモリ不足になる場合があります

## 📄 License

MIT
