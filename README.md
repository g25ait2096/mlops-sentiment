# MLOps Sentiment Pipeline

End-to-end MLOps pipeline fine-tuning DistilBERT on SST-2 sentiment classification.

## Team
| Name | Role | GitHub |
|------|------|--------|
| Sanjay Marathe | Admin / ML lead | @g25ait2096 |
| ABC | Infra / Docker | @ABC |
| XYZ | CI/CD | @XYZ |

## Stack
- Model: `distilbert-base-uncased` (Hugging Face)
- Dataset: SST-2 (GLUE)
- Tracking: Weights & Biases
- Container: Docker + FastAPI
- CI/CD: GitHub Actions

## Branches
- `main` — protected, requires PR review
- `develop` — integration branch

- 
git clone https://github.com/YOUR_ORG/mlops-sentiment.git
cd mlops-sentiment

# Create placeholder files in every folder
mkdir -p data train inference/.github/workflows configs kaggle
touch data/.gitkeep
touch train/.gitkeep
touch inference/app.py inference/Dockerfile inference/requirements.txt
touch configs/base.yaml configs/lr_high.yaml configs/lr_low.yaml
touch kaggle/experiment.ipynb
touch .github/workflows/pipeline.yml

git add .
git commit -m "chore: scaffold folder structure with placeholder files"
git push origin main
