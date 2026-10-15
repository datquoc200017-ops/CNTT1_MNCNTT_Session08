### Phần 1. Phân tích: Vì sao Markdown tối ưu hơn HTML cho AI?

1.  **Tiết kiệm 50–70% Token:**
    
    -   HTML tốn nhiều thẻ mở/đóng và thuộc tính dư thừa (`<h1>...</h1>`, `<p>...</p>`, `class="..."`).
        
    -   Markdown chỉ dùng ký hiệu tối giản (`#`, `-`, `**`). Ít ký tự hơn → ít token hơn → **giảm trực tiếp chi phí API**.
        
2.  **Xử lý nhanh và chính xác hơn:**
    
    -   Càng ít token rác, cơ chế Attention của AI càng tập trung vào **nội dung chính** thay vì phân tích thẻ cấu trúc.
        
    -   Giúp AI phản hồi nhanh hơn và giảm thiểu lỗi "ảo giác" .
        

### Phần 2. Đánh giá & Quyết định

-   **Lựa chọn cho hệ thống:** Chọn **Markdown** để gửi dữ liệu cho AI xử lý nhằm tối ưu chi phí và tốc độ.
    
-   **So sánh nhanh:**
    
    -   **Chi phí Token:** Markdown rất thấp, HTML rất cao do nhiều thẻ thừa.
        
    -   **Độ dễ đọc (Human-readable):** Markdown đọc trực tiếp dạng thô rất dễ; HTML nhiều mã lồng ghép nên rối mắt.
        
    -   **Tốc độ AI:** Markdown xử lý nhanh hơn; HTML chậm hơn vì phải tải thêm token cấu trúc.
        
    -   **Tương thích Git:** Markdown kiểm soát thay đổi theo từng dòng (`diff`) rất sạch; HTML dễ bị xung đột và diff rác.
        
-   **Lý do lập trình viên luôn chọn Markdown cho `README.md`:**
    
    1.  **Đọc trực tiếp:** Dễ đọc ngay trên Terminal (`cat`, `nano`) hoặc Text Editor đơn giản mà không cần trình duyệt web.
        
    2.  **Quản lý phiên bản sạch:** Dễ dàng theo dõi lịch sử chỉnh sửa code (`git diff`) theo từng dòng cụ thể.
        
    3.  **Hỗ trợ code tốt:** Viết code block và tô màu cú pháp bằng 3 dấu backtick (` ``` `) nhanh gọn, không lo bị lỗi mã hóa ký tự như trong HTML.
