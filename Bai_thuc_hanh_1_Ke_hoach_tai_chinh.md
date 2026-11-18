###  Lập kế hoạch tài chính cá nhân

**[C] Context (Bối cảnh & Vai trò):**
Hãy đóng vai một chuyên gia hoạch định tài chính cá nhân thông minh và tỉ mỉ. Bạn đang tư vấn cho một khách hàng có thu nhập biến động mỗi tháng và đang có một số khoản nợ cần thanh toán. Khách hàng này cần một kế hoạch tài chính chi tiết, tối ưu hóa dòng tiền và đề xuất phân bổ ngân sách chi tiêu hợp lý. 

**[R] Request:**
Hãy lập một kế hoạch tài chính hàng tháng từ dữ liệu đầu vào được cung cấp, đảm bảo tính toán chính xác để tối ưu dòng tiền, trả nợ đúng hạn và lập quỹ dự phòng.

**[E] Explanation (Hướng dẫn chi tiết, Ràng buộc & Kỹ thuật CoT):**
**Hãy suy nghĩ từng bước một và tính toán chi tiết trước khi đưa ra quyết định.**
Bạn phải vạch ra quy trình lập luận theo đúng 4 bước sau:
- Bước 1: Tính toán tổng thu nhập khả dụng sau khi trừ thuế và chi phí cố định bắt buộc.
- Bước 2: Phân bổ khoản tiền trả nợ tối thiểu.
- Bước 3: Trích lập quỹ tiết kiệm theo tỷ lệ cam kết (đảm bảo mức tối thiểu 20%).
- Bước 4: Chia phần còn lại cho chi tiêu linh hoạt theo quy tắc 50/30/20 cải tiến.

*Ràng buộc*
- Bắt buộc hiển thị đầy đủ các phép tính cộng, trừ, nhân, chia trung gian. Tuyệt đối không nhảy cóc ra kết quả.
- Đảm bảo tổng tỷ lệ phần trăm phân bổ ngân sách cuối cùng phải bằng chính xác 100%.
- Không dùng Pydantic hay code Python, thực hiện hoàn toàn bằng tư duy logic (Prompting logic).

**[A] Action / Arguments (Dữ liệu đầu vào):**
Thực hiện tính toán dựa trên các số liệu của tháng này như sau:
- Tổng thu nhập: [Điền số tiền, VD: 30.000.000 VNĐ]
- Chi phí cố định bắt buộc: [Điền số tiền, VD: 7.000.000 VNĐ]
- Các khoản nợ cần trả (tối thiểu): [Điền số tiền, VD: 4.000.000 VNĐ]
- Mục tiêu tiết kiệm: [Điền tỷ lệ, VD: 20%]

**[T] Tone / Type (Giọng điệu & Định dạng đầu ra):**
Giọng điệu chuyên nghiệp, rõ ràng. Trình bày kết quả thành hai phần rõ rệt:
- **Phần 1: Nhật ký suy luận logic (Reasoning Steps)** chỉ ra công thức tính toán và số liệu trung gian của từng bước.
- **Phần 2: Bảng phân bổ ngân sách** (hiển thị bằng Markdown Table) gồm các cột: Hạng mục | Số tiền | Tỷ lệ % | Ghi chú.
