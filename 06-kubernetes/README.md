# Giai đoạn 6 — Kubernetes (K8s)

🎯 Điều phối container ở quy mô lớn. Khó nhất nhưng giá trị nhất. Cần vững GĐ2 (Docker) trước.

## Thứ tự học
1. `basics` — Pod, Deployment, Service, ConfigMap, Secret, Ingress
2. `helm` — "Trình quản lý gói" cho K8s, đóng gói app phức tạp
3. `gitops-argocd` — Deploy tự động từ Git (GitOps)

## ✅ Checklist
- [ ] Cài cluster local (minikube / kind / k3s)
- [ ] Deploy app + scale lên nhiều pod
- [ ] Hiểu: Pod vs Deployment vs Service; cách K8s tự healing
- [ ] Expose app ra ngoài bằng Ingress
- [ ] Đóng gói app bằng Helm chart

## 🛠️ Dự án nhỏ
Deploy app web + database lên K8s, scale 3 replica, có Ingress, cập nhật không downtime.

## 📚 Tài nguyên
- kubernetes.io/docs/tutorials
- killercoda.com — sandbox K8s miễn phí
- Chứng chỉ: CKA (Certified Kubernetes Administrator)
