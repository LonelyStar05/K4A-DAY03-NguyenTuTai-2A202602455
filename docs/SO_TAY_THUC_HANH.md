# 📋 SỔ TAY THỰC HÀNH CÁ NHÂN & CHECKLIST TIẾN ĐỘ

---

## 🎯 HÌNH THỨC THỰC HIỆN: CÁ NHÂN

Bài thực hành thiết kế dành cho cá nhân học viên làm chủ quy trình phát triển Tác tử AI (AI Agent):
- Mỗi học viên tự Fork Repo về GitHub cá nhân.
- Tự hoàn thiện mã nguồn, tự đẩy bài nộp lên LMS VLearn.

---

## ⏱️ LỘ TRÌNH THỰC HÀNH (180 PHÚT LÀM BÀI)

```mermaid
gantt
    title TIẾN TRÌNH THỰC HÀNH 180 PHÚT
    dateFormat  m
    axisFormat %M m
    
    Phần 1: Agentic Fit & Tool Schemas       :m1, 0, 45m
    Phần 2: ReAct Loop & MCP Server          :m2, after m1, 60m
    Phần 3: Test Execution & Trace Log       :m3, after m2, 45m
    Phần 4: Self-Audit & Push GitHub Nộp bài :m4, after m3, 30m
```

---

## 📝 CHECKLIST CÁ NHÂN THEO TỪNG MỐC THỜI GIAN

### 🔷 PHẦN 1 (45 phút): Đánh giá Agentic Fit & Tool Schemas
* [ ] Chọn 1 chủ đề thực tế từ tệp `docs/DANH_SACH_DE_TAI.md`.
* [ ] Điền bảng Scoring Matrix 4 tiêu chí Agentic Fit vào file `docs/trace_eval.md`.
* [ ] Khai báo Tool Schema đúng chuẩn JSON Schema cho `schedule_appointment` vào file `src/tools.py`.
* [ ] Thêm 5 câu test case thực tế vào file `config/test_cases.json`.

---

### 🔷 PHẦN 2 (60 phút): ReAct Agent & MCP Server
* [ ] Hoàn thiện hàm thực thi gọi Tool theo chuẩn giao thức MCP trong `src/mcp_server.py`.
* [ ] Chạy lệnh `python src/mcp_server.py` xác nhận khởi tạo thành công MCP Server.
* [ ] Lắp ráp vòng lặp ReAct Native Tool Calling trong `src/app.py`.

---

### 🔷 PHẦN 3 (45 phút): Chạy Kiểm thử & Xuất Trace Waterfall Log
* [ ] Điền API Key thật vào file `.env`.
* [ ] Chạy lệnh `python src/app.py --all` cho 5 test cases.
* [ ] Kiểm tra file vết `docs/trace_waterfall.json` xuất ra đầy đủ độ trễ (latency_ms) và chi tiết các bước.
* [ ] Dán đoạn Trace log tóm tắt vào file `docs/trace_eval.md`.

---

### 🔷 PHẦN 4 (30 phút): Tự kiểm tra & Nộp bài Git/GitHub
* [ ] Kiểm tra tên Repo cá nhân đúng chuẩn: **`K4-DAY03-<HoVaTen>_<MSSV>`**.
* [ ] Chạy lệnh Git để push toàn bộ mã nguồn lên GitHub cá nhân:
  ```bash
  git add .
  git commit -m "feat: complete Day 03 Lab Chatbot vs ReAct Agent"
  git push origin main
  ```
* [ ] Nộp link Repo GitHub cá nhân lên hệ thống VLearn.

---

> [!NOTE]
> **HOÀN THÀNH QUY TRÌNH:** Học viên đã xem xong Sổ tay thực hành. Để quay lại Trang chủ xem lại tổng quan bài học:  
> 👉 **[Quay lại Bước 1: Trang chủ README.md](../README.md)**
