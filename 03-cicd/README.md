# Giai đoạn 3 — CI/CD

🎯 Tự động build → test → deploy mỗi khi push code. Đây là kỹ năng nhà tuyển dụng hỏi nhiều nhất.

## Thứ tự học
1. `github-actions` — Học cái này TRƯỚC (miễn phí, dễ, phổ biến nhất)
2. `gitlab-ci` — Tương tự, dùng nhiều ở công ty dùng GitLab
3. `jenkins` — "Cổ điển" nhưng nhiều doanh nghiệp lớn vẫn dùng

## ✅ Checklist
- [ ] Tạo pipeline tự động test mỗi khi push lên GitHub
- [ ] Pipeline tự build Docker image & đẩy lên registry
- [ ] Hiểu: stage, job, runner, artifact, secret
- [ ] Pipeline tự deploy khi merge vào nhánh main

## 🛠️ Dự án nhỏ
Pipeline GitHub Actions: push code → chạy test → build Docker image → đẩy lên Docker Hub tự động.

## 📚 Tài nguyên
- GitHub Actions docs (docs.github.com/actions)
