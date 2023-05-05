# GrafanaTempo
Grafana Tempo 設定範例

以官方 Grafana Tempo v1.5 的範例為基準來修改  
[https://github.com/grafana/tempo/tree/v1.5.0/example/docker-compose](https://github.com/grafana/tempo/tree/v1.5.0/example/docker-compose)

## 各服務 image 版本
- Grafana Agent: v0.29.0
- Grafana Tempo: main-81aa300-arm64 (mac arm 架構的 cpu, v1.5.x)
- Grafana: 9.3.2
- Grafana Prometheus: v2.40.7

## 使用方式
```
docker-compose up -d
```

## 服務
docker compose 內包含以下服務：

### Grafana Agent
- 資料中轉站
- port: 4317 (grpc), 4318 (http)

### Grafana Prometheus
- 監控各服務的指標
- port: 9090

### Grafana Tempo
- 追蹤資料的資料庫
- port: 3200

### Grafana
- 視覺化
- port: 3000
