# GrafanaTempo
Grafana Tempo設定範例

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