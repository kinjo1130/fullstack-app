# フルスタックを目指したTodoアプリケーション

## 技術構成
- バックエンド
  - Nest.js
  - Prisma
  - Swagger
  - Supabase
- フロントエンド
  - Next.js
  - Orval
  - 
- インフラ
  - Cloud Run
  - Docker
  - GCR
  - Terraform

### 環境構築
それぞれのディレクトリのREADME.mdを見てください


### Deploy方法
- `cd infra`
- `terraform init` // 初回のみ
  - `terraform refresh` // 依存関係を更新したときなど
- `terraform plan` // Deployの内容の確認
- `terraform apply`



### 残っていて、やりたいこと
- 認証周りの追加
- GCRのtagとイメージのpushを自動化(TerraformかMakefileで作るか)
- Secret Mangerを使って、環境変数をセキュアにする
- Testの追加
  - フロントエンド
  - バックエンド(e2eは入っている)
- cron jobsでコールドスタートの回避



### 気になっているところ
- Docker上にSupabaseがあるので、個人でSupabaseのDBを触るなんてことはないはずかを確かめる