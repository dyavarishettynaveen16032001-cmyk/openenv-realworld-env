# OpenEnv Real World Environment

## Overview
This project implements a real-world AI training environment using the OpenEnv specification.

## Features
- step() / reset() / state() API
- Typed Pydantic models
- Easy / Medium / Hard grading
- Reward normalization (0.0–1.0)
- Docker container support
- Hugging Face Spaces ready

## Project Structure
```bash
app/
  env.py
  models.py
  graders.py
  baseline.py
```

## Actions
- 0 = Complete Task
- 1 = Optimize
- 2 = Waste

## Observations
- budget
- tasks_pending
- completed
- efficiency

## Installation
```bash
pip install -r requirements.txt
```

## Run Baseline
```bash
python app/baseline.py
```

## Docker
```bash
docker build -t openenv .
docker run openenv
```# openenv-realworld-env
Production-grade OpenEnv-compliant real-world simulation environment for AI agent training, benchmarking, Docker deployment, and Hugging Face Spaces hosting.
