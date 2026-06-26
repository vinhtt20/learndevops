# 🚀 Lộ trình học DevOps (cho người trái ngành)

Repo này là không gian học tập DevOps được tổ chức theo **lộ trình tuần tự**: học từ nền tảng
(Linux, mạng, dòng lệnh) rồi đi dần lên các kỹ năng cao hơn. Mỗi thư mục có số thứ tự — học theo
đúng thứ tự đó, đừng nhảy cóc.

> 💡 **Nguyên tắc cho người trái ngành:** Đừng cố hiểu hết mọi thứ cùng lúc. Mỗi giai đoạn học
> đủ để *làm được* một dự án nhỏ, rồi mới sang giai đoạn sau. Học bằng cách gõ tay, không chỉ đọc.

## 🗺️ Bản đồ lộ trình

| Giai đoạn | Thư mục | Học gì | Thời gian gợi ý |
|-----------|---------|--------|-----------------|
| 0 | `00-foundations` | Linux, mạng cơ bản, dòng lệnh, Git | 4–6 tuần |
| 1 | `01-scripting` | Bash & Python để tự động hóa | 3–4 tuần |
| 2 | `02-containers` | Docker & Docker Compose | 3–4 tuần |
| 3 | `03-cicd` | CI/CD: GitHub Actions / GitLab / Jenkins | 3–4 tuần |
| 4 | `04-cloud` | Cloud cơ bản (chọn 1: AWS / Azure / GCP) | 4–6 tuần |
| 5 | `05-iac` | Infrastructure as Code: Terraform, Ansible | 4 tuần |
| 6 | `06-kubernetes` | Kubernetes, Helm, GitOps | 6–8 tuần |
| 7 | `07-observability` | Monitoring & Logging (Prometheus/Grafana, ELK) | 3–4 tuần |
| 8 | `08-security-devsecops` | Bảo mật trong pipeline | 2–3 tuần |

## 📁 Thư mục hỗ trợ

- **`projects/`** — Dự án thực hành. Đây là phần quan trọng nhất để bỏ vào CV/portfolio.
- **`labs/`** — Nơi thử nghiệm linh tinh, code nháp, phá phách thoải mái.
- **`notes/`** — Ghi chú học tập, cheatsheet, chuẩn bị phỏng vấn.
- **`resources/`** — Link khóa học, sách, bài viết hay.

## ✅ Cách dùng repo này

1. Vào thư mục giai đoạn hiện tại, đọc `README.md` của nó.
2. Làm theo phần "Mục tiêu" và "Bài tập".
3. Ghi lại tiến độ mỗi ngày vào `notes/daily-log/`.
4. Sau mỗi 1–2 giai đoạn, làm 1 dự án trong `projects/`.
5. Đánh dấu ✅ vào checklist khi xong.

## 🎯 Mục tiêu cuối cùng

Hoàn thành **dự án capstone** (`projects/capstone/`): triển khai một ứng dụng thật từ source code →
container → CI/CD pipeline → cloud → Kubernetes → có monitoring. Đây sẽ là tấm vé đi xin việc.

---
*Bắt đầu ngay: mở `00-foundations/README.md`*
