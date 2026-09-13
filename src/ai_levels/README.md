# 📚 ARCHITECTURAL REFERENCE LEVELS [REFERENCE ONLY]

> ⚠️ **LƯU Ý QUAN TRỌNG DÀNH CHO HỌC VIÊN:**
> - Các file trong thư mục này (`ai_levels/`) **KHÔNG PHẢI LÀ BÀI TẬP** bạn cần chỉnh sửa hay debug.
> - Đây là **MÃ NGUỒN MẪU THAM KHẢO** thể hiện quá trình tiến hóa kiến trúc qua các cấp độ Agentic AI:
>   * `level3_native_mcp_agent.py`: Cấp 3 - ReAct Agent giao tiếp qua giao thức MCP (Model Context Protocol).
> - **PHẦN BÀI TẬP BẮT BUỘC CỦA BẠN NẰM Ở:**
>   1. **`src/tools.py`**: Khai báo Tool Schemas JSON (Task 1.2).
>   2. **`src/mcp_server.py`**: Hoàn thiện hàm thực thi gọi tool qua MCP Server (Task 2.1).
>   3. **`src/app.py`**: Lắp ráp ReAct Loop và trích xuất Trace Log (Task 2.2).
>   4. **`config/test_cases.json`**: Viết bộ 5 Test Cases theo đề tài bạn đã chọn (Task 1.1).
