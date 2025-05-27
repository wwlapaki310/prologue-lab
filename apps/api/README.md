# API Backend (FastAPI)

PrologueLabのバックエンドAPI

## 技術スタック
- FastAPI
- Python 3.11+
- SQLAlchemy
- Alembic (マイグレーション)
- Pydantic
- PostgreSQL

## セットアップ
```bash
cd apps/api
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --reload
```

## API エンドポイント
- `/api/v1/opportunities` - 公募情報CRUD
- `/api/v1/auth` - 認証・認可
- `/api/v1/users` - ユーザー管理
- `/api/v1/search` - 検索機能
