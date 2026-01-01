# fastapi-docker-template

## Overview
Minimal FastAPI template with Docker.
JWT authentication + Swagger Authorize supported.

## Features
- FastAPI
- JWT auth (/token, /me)
- Swagger UI with Authorize
- Docker (python:3.11-slim)

## Run
docker build -t fastapi-app .
docker run -p 8000:8000 fastapi-app

## Auth (Swagger)
1. POST /token
2. Copy access_token
3. Click Authorize

## Notes (for developers)
- FROM：土台
- WORKDIR：作業場所
- COPY：PC → コンテナ
- RUN：build中に実行
- CMD：起動コマンド
- -p：PC ↔ コンテナの橋
