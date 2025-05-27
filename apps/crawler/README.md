# Data Crawler

公募情報を自動収集するクローラーシステム

## 技術スタック
- Scrapy
- Playwright
- Python 3.11+
- Celery (非同期タスク)
- Redis (キュー)

## 主要機能
- 政府・大学サイトのクローリング
- RSS/Atom フィード解析
- 重複除去・データクリーニング
- スケジューリング実行

## 対象サイト
- 文部科学省 科学技術振興機構
- JSPS 日本学術振興会
- Kaggle Competitions
- GitHub sponsors
- 各大学の公募情報
