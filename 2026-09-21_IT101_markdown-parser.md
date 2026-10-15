# ⚙️ Tìm Hiểu Về Cơ Chế Hoạt Động Của Markdown Parser

> *“Đơn giản, gọn nhẹ và tối ưu hóa thời gian biên dịch tài liệu kỹ thuật.”*

## 🚀 Tổng quan
**Markdown Parser** là công cụ nhận diện các ký tự thô (như `#`, `-`, `**`) và chuyển đổi chúng thành các thẻ định dạng HTML tương ứng trên trình duyệt.

## 🛠️ Ví dụ minh họa khối mã nguồn (Code Block)
Đoạn mã Python mô phỏng cách bộ phân tích kiểm tra cú pháp tiêu đề đơn giản:

```python
def kiem_tra_heading(dong):
    if dong.startswith("#"):
        return "Day la the Heading"
    return "Van ban thuong"
```
---
---

#### **3. Nội dung file tích hợp AI `2026-10-15_IT108_ai-token-explained.md`**

```markdown
#  Khái Niệm Token Trong AI (Được giải thích bởi AI)

##  Prompt đã gửi cho AI (Chiến lược 3 phần)
```markdown
## Bối cảnh
Tôi là sinh viên năm nhất Khoa CNTT, chưa có nền tảng lập trình sâu.

## Khái niệm cần giải thích
Thuật ngữ "Token" trong ngữ cảnh xử lý ngôn ngữ của AI và LLM.

```
"Token là đơn vị cơ bản mà AI dùng để đọc và viết. Bạn có thể tưởng tượng một câu dài giống như một bức tranh ghép hình Lego, mỗi mảnh Lego nhỏ (có thể là một từ, một phần của từ hoặc một dấu câu) chính là một Token. Ví dụ, từ 'Lập trình' có thể được AI cắt thành 2 token riêng biệt để xử lý."

---

### **Phần 3: Giải quyết Trường hợp Kiểm thử (Edge Case)**

* **Tình huống:** Sau 1 tháng, Knowledge Base có 50 file và bạn không nhớ tên file giải thích về 'Token AI'.
* **Đề xuất 2 cơ chế tìm kiếm nhanh:**
  1. **Cơ chế 1: Sử dụng tính năng tìm kiếm nội dung toàn cục (Global Text Search / `Ctrl + Shift + F` trong VS Code)**
     * *Cách hoạt động:* Gõ từ khóa `Token` vào khung tìm kiếm hệ thống để quét toàn bộ nội dung text bên trong 50 file `.md`.
     * *Ưu điểm:* Tìm thấy chính xác đoạn văn bản chứa từ khóa dù tên file hoàn toàn không khớp.
     * *Nhược điểm:* Nếu từ khóa xuất hiện quá nhiều lần ở các file khác nhau, danh sách kết quả trả về sẽ bị loãng, mất thời gian lọc.
  2. **Cơ chế 2: Áp dụng hệ thống Frontmatter Metadata & Tagging (Gắn thẻ phân loại)**
     * *Cách hoạt động:* Thêm phần đầu mỗi file `.md` các thẻ siêu dữ liệu (ví dụ: `tags: [AI, LLM, token, IT108]`) kết hợp với việc duy trì bảng `INDEX.md` làm mục lục trung tâm.
     * *Ưu điểm:* Quản lý cực kỳ chuyên nghiệp, thu hẹp phạm vi tìm kiếm theo đúng chủ đề ngay lập tức mà không cần mở từng file.
     * *Nhược điểm:* Đòi hỏi thói quen kỷ luật cao của người dùng phải cập nhật tag đầy đủ cho mọi file mới tạo ra.



## Yêu cầu
- Dùng ngôn ngữ đơn giản, so sánh với mảnh ghép Lego hoặc ký tự.
- Giải thích ngắn gọn dưới 150 từ.
