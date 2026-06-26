# Giai đoạn 8 — Bảo mật & DevSecOps

🎯 "Shift left" — đưa bảo mật vào sớm trong pipeline thay vì kiểm tra sau cùng.

## Học gì
- Quản lý secret (Vault, sealed-secrets) — KHÔNG bao giờ để password trong code
- Scan lỗ hổng image Docker (Trivy)
- Scan code & dependency (SAST, dependency scanning)
- Nguyên tắc least privilege (IAM, RBAC)

## ✅ Checklist
- [ ] Thêm bước scan image (Trivy) vào pipeline CI/CD
- [ ] Quản lý secret an toàn (không hardcode)
- [ ] Hiểu OWASP Top 10 ở mức cơ bản
- [ ] Áp dụng least privilege cho IAM/RBAC

## 🛠️ Dự án nhỏ
Bổ sung security scanning vào pipeline GĐ3: chặn deploy nếu image có lỗ hổng nghiêm trọng.

## 📚 Tài nguyên
- OWASP DevSecOps Guideline
- Trivy docs (aquasecurity.github.io/trivy)
