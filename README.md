# Git/GitHub 練習用リポジトリ

このリポジトリは、Git および GitHub の操作を練習するために設計されています。基本的な Git コマンド、ブランチ管理、コンフリクト解消、コラボレーションワークフローに慣れることを目的としています。

## 概要

このリポジトリは、以下の Git および GitHub の様々な側面をカバーするために構成されています：

- 基本的な Git コマンド（`clone`、`pull`、`push`など）
- ブランチ管理とマージ
- コンフリクトの解消
- プルリクエストの作成とレビュー
- `.gitignore`やリポジトリ設定の取り扱い

## リポジトリ構成

- **`README.md`**: このファイルです。リポジトリの概要と練習用の手順書が記載されています。
- **`LICENSE`**: リポジトリのライセンス。
- **`index.html`**:このファイルを更新していく。
- **`.gitignore`**: Git で追跡しないファイルやディレクトリを指定するためのファイル。
- **`src/`**: メインのコードを含むディレクトリ。スクリプトやプロジェクトが増えるに従って拡張します。

## ブランチ戦略

- **`main` ブランチ**: 完成した機能やバグ修正がマージされる安定したブランチ。
- **`develop` ブランチ**: `main`にマージする前に新しい機能を統合するためのブランチ。
- **`feature/*` ブランチ**: 新しい機能を開発するため、または変更を加えるためのブランチ。

## 練習手順

### 1. リポジトリをクローンする

```bash
git clone https://github.com/yourusername/git-practice.git
```

### 2. 新しいブランチを作成する

```bash
git checkout -b feature/your-feature-name
```

### 3. 変更を加えコミットする

- `src/index.html`に新しい行を追加します。
- ul タグ内の li タグ最終行に`<li>your name</li>`を追加します。
- 変更をステージングし、コミットします。

```bash
git add .
git commit -m "add your sname"
```

### 4. 変更をプッシュする

```bash
git push origin feature/your-feature-name
```

### 5. プルリクエストを作成する

- GitHub 上でリポジトリにアクセスします。
- `feature/*`ブランチから`develop`または`main`ブランチへの新しいプルリクエストを作成します。
- レビューを依頼するか、ソロプロジェクトの場合は自分でマージします。

### 6. マージとコンフリクトの解消

- マージコンフリクトが発生した場合、ローカルまたは GitHub のコンフリクト解消ツールを使用して解決の練習を行います。
- コンフリクトが解消されたら、プルリクエストをマージします。

### 7. 最新の変更を取得する

```bash
git checkout main
git pull origin main
```

## 参考文献

- [Pro Git Book](https://git-scm.com/book/ja/v2) - Git の包括的なガイド。
- [GitHub Docs](https://docs.github.com/ja) - GitHub の公式ドキュメント。
