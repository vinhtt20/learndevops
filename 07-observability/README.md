# Giai đoạn 7 — Observability (Giám sát & Logging)

🎯 "Không đo được thì không quản được." Biết hệ thống đang khỏe hay sắp sập.

## Thứ tự học
1. `prometheus-grafana` — Metrics & dashboard (đo CPU, RAM, request...)
2. `logging-elk` — Thu thập & tìm kiếm log tập trung (Elasticsearch/Loki + Kibana/Grafana)

## ✅ Checklist
- [ ] Cài Prometheus thu metrics, Grafana vẽ dashboard
- [ ] Đặt cảnh báo (alert) khi CPU/RAM vượt ngưỡng
- [ ] Gom log nhiều service về một nơi và tìm kiếm được
- [ ] Hiểu 3 trụ cột: metrics, logs, traces

## 🛠️ Dự án nhỏ
Thêm monitoring vào app K8s ở GĐ6: dashboard Grafana + alert khi service chết.

## 📚 Tài nguyên
- Grafana Play (play.grafana.org)
- Prometheus docs
