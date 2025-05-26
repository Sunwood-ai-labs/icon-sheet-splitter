<div align="center">

![](assets/icon-sheet-splitter-banner.svg)

  <h1>🎯 Icon Sheet Splitter</h1>

  <p>
    <img alt="GitHub" src="https://img.shields.io/github/license/Sunwood-ai-labs/icon-sheet-splitter">
    <img alt="HTML5" src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white">
    <img alt="CSS3" src="https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white">
    <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black">
    <img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white">
    <img alt="GitHub issues" src="https://img.shields.io/github/issues/Sunwood-ai-labs/icon-sheet-splitter">
    <img alt="GitHub pull requests" src="https://img.shields.io/github/issues-pr/Sunwood-ai-labs/icon-sheet-splitter">
  </p>

  <p>
    大きなアイコンシートを個別ファイルに分割するWebアプリケーション<br>
    <b>ドラッグ&ドロップ</b>で簡単操作、<b>複数フォーマット対応</b>でデザイナーの作業効率を向上✨
  </p>

  <p>
    <a href="README_EN.md">🇺🇸 English</a> | 
    <a href="README.md">🇯🇵 日本語</a>
  </p>

</div>

## 📖 概要

Icon Sheet Splitterは、大きなアイコンシートファイルを指定したグリッドに従って個別のアイコンファイルに分割する、ブラウザベースのWebアプリケーションです。ゲーム開発、Webデザイン、モバイルアプリ開発において、スプライトシートやアイコンセットを効率的に管理できます。

### 🎯 主な特徴
- **シンプルなWeb UI**: ブラウザ上で動作、インストール不要
- **ドラッグ&ドロップ対応**: 直感的なファイルアップロード
- **リアルタイムプレビュー**: 分割結果をその場で確認
- **複数フォーマット対応**: PNG、JPG、WebP形式での出力
- **カスタマイズ可能**: グリッドサイズとファイル名を自由に設定

## ✨ 機能

- **📁 ファイルアップロード**: ドラッグ&ドロップまたはクリックで画像を選択
- **⚙️ 分割設定**: 列数・行数を指定してグリッドをカスタマイズ
- **👀 リアルタイムプレビュー**: 分割線を可視化して結果を事前確認
- **🖼️ 複数フォーマット出力**: PNG/JPG/WebP形式に対応
- **📝 ファイル名設定**: プレフィックスを指定して一括命名
- **⬇️ 個別/一括ダウンロード**: 単体ダウンロードまたは全ファイル一括取得
- **📱 レスポンシブデザイン**: PC・タブレット・スマートフォンに対応

## 🛠️ 技術スタック

- **HTML5**: セマンティックなマークアップとCanvas API
- **CSS3**: モダンなレイアウトとアニメーション
- **JavaScript ES6+**: 非同期処理とDOM操作
- **Canvas API**: 画像処理と分割機能
- **Docker**: コンテナ化による簡単デプロイ
- **Nginx**: 静的ファイル配信

## 🚀 使用方法

### 🌐 ブラウザで直接使用

1. **ファイルをダウンロード**
```bash
git clone https://github.com/Sunwood-ai-labs/icon-sheet-splitter.git
cd icon-sheet-splitter
```

2. **ブラウザで開く**
```bash
open index.html  # macOS
start index.html # Windows
```

### 🐳 Dockerで実行

1. **イメージをビルド**
```bash
docker build -t icon-sheet-splitter .
```

2. **コンテナを起動**
```bash
docker run -p 8080:80 icon-sheet-splitter
```

3. **ブラウザでアクセス**
```
http://localhost:8080
```

### 🔧 Docker Composeで実行

```bash
docker-compose up -d
```

## 💡 使用例

### 基本的な使い方

1. **画像をアップロード** - アイコンシートをドラッグ&ドロップ
2. **分割設定** - 列数・行数を指定（例：4×4グリッド）
3. **プレビュー確認** - 分割線が正しく表示されているか確認
4. **出力設定** - フォーマット（PNG/JPG/WebP）とファイル名プレフィックスを設定
5. **分割実行** - 「アイコンを分割」ボタンをクリック
6. **ダウンロード** - 個別またはまとめてダウンロード

### 実用的なケース

- **ゲーム開発**: スプライトシートを個別キャラクターファイルに分割
- **Webデザイン**: アイコンセットを個別アイコンに分割
- **モバイルアプリ**: UI要素を解像度別にバッチ処理
- **素材管理**: 大型アセットの効率的な管理と配布

## 📁 プロジェクト構成

```
icon-sheet-splitter/
├── README.md                 # プロジェクト説明書
├── index.html               # メインアプリケーション
├── assets/                  # 静的リソース
│   └── icon-sheet-splitter-banner.svg
├── Dockerfile              # Docker設定
├── docker-compose.yml      # Docker Compose設定
└── CLAUDE.md              # 開発ガイドライン
```

## 🎨 カスタマイズ

### CSS変数による見た目の調整

`index.html`の`:root`セクションでカラーテーマを変更可能：

```css
:root {
    --primary-color: #2c3e50;
    --accent-color: #e74c3c;
    --gold-color: #f39c12;
    /* 他のカラー変数... */
}
```

### 機能の拡張

JavaScriptセクションを編集して以下の機能を追加可能：
- 新しい出力フォーマットの対応
- カスタム分割パターン
- 画像フィルターの適用
- バッチ処理機能

## 🧪 対応ブラウザ

- **Chrome** 80+
- **Firefox** 75+
- **Safari** 13+
- **Edge** 80+

※ Canvas APIとES6機能を使用するため、モダンブラウザが必要です

## 🤝 コントリビューション

プロジェクトへの貢献を歓迎します！

### 貢献方法

1. **Issues報告** - バグ報告や機能要望をGitHub Issuesで投稿
2. **プルリクエスト** - 新機能や改善の実装
3. **ドキュメント改善** - READMEや説明の充実
4. **テスト** - 異なる環境での動作確認

### 開発環境のセットアップ

```bash
# リポジトリをフォーク
git fork https://github.com/Sunwood-ai-labs/icon-sheet-splitter.git

# ブランチを作成
git checkout -b feature/your-feature-name

# 変更を実装
# テストを実行
# プルリクエストを作成
```

## 📋 今後の予定

- [ ] SVG形式の対応
- [ ] アニメーションGIF分割機能
- [ ] AI-powered自動分割
- [ ] クラウドストレージ連携
- [ ] PWA対応
- [ ] 多言語国際化

## 📄 ライセンス

このプロジェクトはMITライセンスの下で公開されています。

## 👥 作者情報

- **開発**: [Sunwood AI Labs](https://github.com/Sunwood-ai-labs)
- **メンテナー**: Sunwood AI Labs チーム

## 🙏 謝辞

- Canvas APIを活用した画像処理機能
- モダンWebテクノロジーの活用
- オープンソースコミュニティへの感謝

---

<div align="center">

**Made with ❤️ using Modern Web Technologies**

[🏠 ホーム](https://github.com/Sunwood-ai-labs/icon-sheet-splitter) | 
[📊 Issues](https://github.com/Sunwood-ai-labs/icon-sheet-splitter/issues) | 
[🔄 Pull Requests](https://github.com/Sunwood-ai-labs/icon-sheet-splitter/pulls)

</div>