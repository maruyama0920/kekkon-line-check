### Cloud Runへデプロイ

```bash
# 方法A: ソースから直接デプロイ（env.yaml使用）
gcloud config set project aga-line-check

gcloud run deploy aga-line-check --source .  --region=asia-northeast1  --platform=managed  --allow-unauthenticated --env-vars-file env.yaml
