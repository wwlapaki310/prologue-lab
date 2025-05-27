# Contributing to PrologueLab

🎉 まず始めに、PrologueLabプロジェクトに貢献していただき、ありがとうございます！

冒険者として、あなたの貢献がより多くの人々の「はじまりの一歩」をサポートすることになります。

## 🗺️ 貢献の方法

### 1. Issues
- **バグ報告**: 見つけた問題を詳しく報告してください
- **機能提案**: 新しいアイデアや改善案を提案してください
- **質問**: 分からないことがあれば気軽に質問してください

### 2. Pull Requests
- **新機能**: 新しい機能の実装
- **バグ修正**: 既存の問題の解決
- **ドキュメント改善**: README、技術仕様書などの改善
- **UI/UX改善**: より良いユーザー体験の提供

### 3. その他の貢献
- **情報提供**: 新しい公募情報の提供
- **デザイン**: アイコン、イラストの作成
- **翻訳**: 多言語対応のサポート
- **テスト**: QA、ユーザビリティテスト

## 🛠️ 開発環境のセットアップ

### 前提条件
- Node.js 18+
- Python 3.11+
- Docker & Docker Compose
- Git

### セットアップ手順

1. **リポジトリをフォーク**
```bash
# GitHubでフォークしてからクローン
git clone https://github.com/your-username/prologue-lab.git
cd prologue-lab
```

2. **環境変数の設定**
```bash
cp .env.example .env
# .envファイルを編集して必要な設定を追加
```

3. **依存関係のインストール**
```bash
npm install
```

4. **開発環境の起動**
```bash
# Dockerで全サービスを起動
npm run docker:up

# または個別に起動
npm run dev
```

5. **データベースの初期化**
```bash
npm run db:migrate
npm run db:seed
```

## 📋 コーディング規約

### TypeScript/JavaScript
- ESLintとPrettierの設定に従ってください
- 関数とクラスにはTSDocコメントを記述
- テストを必ず書いてください

### Python
- Black、flake8の設定に従ってください
- 型ヒントを使用してください
- doctestまたはpytestでテストを書いてください

### コミットメッセージ
Conventional Commitsを使用してください：
```
type(scope): subject

body

footer
```

例：
```
feat(api): add opportunity search endpoint
fix(ui): resolve card hover animation issue
docs(readme): update installation instructions
```

## 🧪 テスト

### フロントエンド
```bash
cd apps/web
npm run test        # ユニットテスト
npm run test:e2e    # E2Eテスト
```

### バックエンド
```bash
cd apps/api
python -m pytest    # ユニットテスト
python -m pytest tests/integration/  # 統合テスト
```

## 🚀 Pull Request のプロセス

1. **ブランチの作成**
```bash
git checkout -b feature/your-feature-name
# または
git checkout -b fix/issue-description
```

2. **コードの変更**
- 小さな、焦点を絞った変更を心がけてください
- テストを追加/更新してください
- ドキュメントを更新してください

3. **コミット**
```bash
git add .
git commit -m "feat: add new adventure card component"
```

4. **プッシュとPR作成**
```bash
git push origin feature/your-feature-name
```
その後、GitHubでPull Requestを作成してください。

### PRの説明に含めるべき内容
- 変更の概要と理由
- 関連するIssue番号（`Closes #123`）
- テスト方法
- スクリーンショット（UI変更の場合）

## 📝 Issue の作成

### バグ報告
```markdown
## バグの概要
簡潔にバグを説明してください。

## 再現手順
1. ページ「...」に移動
2. ボタン「...」をクリック
3. エラーが発生

## 期待される動作
何が起こるべきかを説明してください。

## 実際の動作
実際に何が起こったかを説明してください。

## 環境
- OS: 
- ブラウザ: 
- バージョン: 
```

### 機能要求
```markdown
## 機能の概要
追加したい機能を説明してください。

## 動機
なぜこの機能が必要なのかを説明してください。

## 提案する解決策
機能の実装方法を説明してください。

## 代替案
他に考えられる解決策があれば記述してください。
```

## 🌟 コミュニティガイドライン

### 行動規範
- 敬意を持って接してください
- 建設的なフィードバックを提供してください
- 包括的な環境を維持してください
- 学習意欲を大切にしてください

### コミュニケーション
- **GitHub Issues**: バグ報告、機能要求
- **GitHub Discussions**: 一般的な質問、アイデア共有
- **Pull Requests**: コードレビュー、技術的議論

## 🏆 貢献者の認識

貢献者の皆様は以下の方法で認識されます：
- README.mdの貢献者セクションに記載
- リリースノートでの言及
- 特別な「冒険者バッジ」の付与（将来予定）

## 📚 参考資料

- [技術アーキテクチャ](docs/architecture/system-design.md)
- [API仕様](docs/api/openapi-spec.md)
- [UIコンポーネント](docs/design/ui-components.md)
- [デプロイメント](docs/deployment/infrastructure.md)

## 💡 始めやすい貢献

初回貢献者におすすめのタスク：
- ドキュメントの typo 修正
- テストケースの追加
- 小さなUI改善
- サンプルデータの追加

「good first issue」ラベルの付いたIssueから始めることをお勧めします。

---

🌟 **あなたの冒険がここから始まります！** 質問があれば遠慮なくお聞かせください。

一緒にPrologueLabを世界中の冒険者にとって最高のプラットフォームにしましょう！