# Giai đoạn 5 — Infrastructure as Code (IaC)

🎯 Thay vì click chuột tạo server, ta viết code mô tả hạ tầng → tái lập, version, review được.

## Thứ tự học
1. `terraform` — Tạo & quản lý hạ tầng cloud bằng code (chuẩn ngành)
2. `ansible` — Cấu hình & cài đặt phần mềm trên server (configuration management)

## ✅ Checklist
- [ ] Dùng Terraform tạo một EC2 + security group trên AWS
- [ ] Hiểu: state, plan, apply, module, variable
- [ ] Dùng Ansible cài nginx lên nhiều server cùng lúc
- [ ] Không bao giờ commit file state/secret lên Git

## 🛠️ Dự án nhỏ
Terraform tạo toàn bộ hạ tầng (VPC + EC2 + S3), Ansible cấu hình server → tất cả bằng code.

## 📚 Tài nguyên
- HashiCorp Learn (developer.hashicorp.com/terraform/tutorials)
