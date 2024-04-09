# How to use Grafana K6 for load testing

## Introduction

This document will guide you through the process of setting up Grafana and K6 for load testing.

## Prerequisites

- Docker
- Docker Compose

## Setup

1. Install K6 https://grafana.com/docs/k6/latest/set-up/install-k6/

2. Create folder for your test scripts and cd into it

3. Create and initialize a new script file

```bash
docker run --rm -i -v $PWD:/app -w /app grafana/k6 new
```

4. Run K6

```bash
docker run --rm -i grafana/k6 run - <script.js
```

## References

1. https://grafana.com/docs/k6/latest/set-up/install-k6
2. https://grafana.com/docs/k6/latest/get-started/running-k6/
