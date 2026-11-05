# AirPulse 🌬️

**End-to-End MLOps Platform for Real-Time Air Quality Forecasting**

> 🚧 Work in progress — building in public.

AirPulse ingests live air quality and weather data, forecasts hourly AQI
with ML/DL models, and automatically detects drift and retrains —
deployed entirely on free infrastructure.

## Planned Features
- [ ] Automated hourly data ingestion (Open-Meteo)
- [ ] Data validation & versioning (Pandera, DVC)
- [ ] Experiment tracking & model registry (MLflow on DagsHub)
- [ ] Forecasting models: XGBoost baseline → LSTM
- [ ] FastAPI serving in Docker, deployed on Hugging Face Spaces
- [ ] CI/CD with GitHub Actions
- [ ] Drift monitoring (Evidently) & automated retraining
- [ ] Live dashboard (Streamlit)

## Tech Stack
Python · Pandas · XGBoost · PyTorch · DVC · MLflow · FastAPI · Docker ·
uv GitHub Actions · Evidently · Prometheus · Grafana · Streamlit

## Architecture
See [ARCHITECTURE.md](ARCHITECTURE.md).

## Local Setup
Requires [uv](https://docs.astral.sh/uv/).
```bash
git clone https://github.com/<you>/air-pulse.git
cd air-pulse
uv sync          # creates .venv with Python 3.12 and installs locked deps
```
Roadmap

Phase 1 Foundations → 2 Data pipeline → 3 Modelling → 4 Serving →
5 CI/CD → 6 Monitoring & retraining → 7 Dashboard
