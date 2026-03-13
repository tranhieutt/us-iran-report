---
layout: post
title: "Báo cáo Thủ công → AI Tự động"
date: 2026-03-13 10:00:00 +0700
categories: [AI, Automation, Productivity]
tags: [AI Agent, Pandoc, Tự động hóa]
author: "tranhieutt"
---

# Báo cáo Thủ công → AI Tự động

Ghi chú cá nhân - quy trình tự động hóa viết báo cáo học thuật (Case Study: Mỹ - Iran)

## Thu thập dữ liệu Thủ công → Multi-Agent

Bình thường: Mình phải đọc từng trang báo, tự lọc thông tin, copy và lưu link thủ công.
Bây giờ: Dùng 5 AI Agents quét và tổng hợp dữ liệu song song:

- Chính sách Mỹ (Trump) → us-policy-agent ✓
- Động thái Iran → iran-intel-agent ✓
- Biến động giá dầu → oil-market-analyst ✓

Tất cả dữ kiện được gom lại thành 1 file Markdown thô, đầy đủ số liệu mới nhất.

## Hành văn Tin tức thô ráp → Chuẩn Học thuật

Bình thường: Tự cấu trúc lại bài viết, chuyển đổi văn phong, viết kết nối ý.
Bây giờ: Kích hoạt `Academic Writer` agent để tự động rập khuôn lại bài báo thô thành bài nghiên cứu khách quan:

- Tóm tắt (Abstract) ✓
- Bối cảnh (Introduction) ✓
- Phân tích diễn biến (Pattern Analysis) ✓
- Đánh giá tác động KT-CT (Geoeconomic Impact) ✓
- Kết luận (Conclusion) ✓

## Xuất bản file Copy/Paste → Pandoc Workflow

Bình thường: Copy đoạn chat từ AI dán sang Word, sửa lại từng thẻ heading, chỉnh font, in đậm... (rất mất thời gian).
Bây giờ: Dùng Pandoc CLI - tự động bung file Markdown sang Word (.docx) mượt mà giữ nguyên cấu trúc:

```
pandoc report.md -o report.docx
```

## Kết luận

Hệ thống tự động hóa hoàn toàn luồng viết lách:

- Thời gian tìm kiếm & viết bài: Giảm 90% ✓
- Cấu trúc & định dạng: Chuẩn xác 100% ✓
- Việc duy nhất cần làm: Đọc duyệt lại tính logic của tư duy phân tích mà AI trả về.
