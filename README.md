# 💬 Chatbot Anh Lập Trình

Chương trình chatbot được tạo ra từ Anh Lập Trình (https://pyan.vn/)

## 📋 Mô tả

Đây là một ứng dụng chatbot tương tác được xây dựng bằng Streamlit và tích hợp với OpenAI API. Chatbot sử dụng các file training để tùy chỉnh hành vi và phản hồi.

## 🚀 Cài đặt

### Yêu cầu hệ thống
- Python 3.7 trở lên
- Tài khoản OpenAI API (có API key)

### Các bước cài đặt

1. **Clone hoặc tải dự án về máy**

2. **Cài đặt các thư viện cần thiết:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Cấu hình API Key:**
   - Mở file `streamlit_app.py`
   - Thay thế API key OpenAI của bạn vào dòng 28:
   ```python
   openai_api_key = "your-api-key-here"
   ```
   ⚠️ **Lưu ý bảo mật:** Không nên commit API key vào git. Nên sử dụng biến môi trường hoặc file cấu hình riêng.

4. **Chuẩn bị các file cần thiết:**
   - `00.xinchao.txt` - Nội dung chào mừng
   - `01.system_trainning.txt` - Hệ thống training cho chatbot
   - `02.assistant.txt` - Tin nhắn khởi tạo từ assistant
   - `module_chatgpt.txt` - Tên model ChatGPT sử dụng (ví dụ: "gpt-3.5-turbo" hoặc "gpt-4")
   - `phong.jpg` - Logo/hình ảnh hiển thị (tùy chọn)

## 🎯 Sử dụng

Chạy ứng dụng bằng lệnh:
```bash
streamlit run streamlit_app.py
```

Ứng dụng sẽ tự động mở trong trình duyệt mặc định tại địa chỉ `http://localhost:8501`

## 📁 Cấu trúc dự án

```
Repository_Chatbot/
├── streamlit_app.py          # File chính của ứng dụng
├── requirements.txt          # Danh sách các thư viện cần thiết
├── README.md                 # File hướng dẫn này
├── 00.xinchao.txt           # Nội dung chào mừng
├── 01.system_trainning.txt  # Hệ thống training
├── 02.assistant.txt         # Tin nhắn khởi tạo
├── module_chatgpt.txt       # Tên model ChatGPT
├── phong.jpg                # Logo/hình ảnh (tùy chọn)
└── setup.sh                 # Script setup (nếu có)
```

## ✨ Tính năng

- 💬 Giao diện chat trực quan và dễ sử dụng
- 🤖 Tích hợp OpenAI API với streaming response
- 📝 Lưu trữ lịch sử hội thoại trong session
- 🎨 Giao diện được tùy chỉnh với CSS
- 📚 Hỗ trợ training tùy chỉnh thông qua file text

## 🔧 Cấu hình

### Thay đổi model ChatGPT
Chỉnh sửa nội dung trong file `module_chatgpt.txt` (ví dụ: `gpt-3.5-turbo`, `gpt-4`, `gpt-4-turbo-preview`)

### Tùy chỉnh hành vi chatbot
- Chỉnh sửa `01.system_trainning.txt` để thay đổi cách chatbot phản hồi
- Chỉnh sửa `02.assistant.txt` để thay đổi tin nhắn chào mừng ban đầu

## 📝 Ghi chú

- Đảm bảo bạn có đủ credit trong tài khoản OpenAI để sử dụng API
- API key được lưu trực tiếp trong code (không an toàn cho production)
- Đề xuất sử dụng biến môi trường hoặc Streamlit secrets cho API key trong môi trường production

## 👨‍💻 Tác giả

Anh Lập Trình - https://pyan.vn/

## 📄 License

Dự án này được tạo ra bởi Anh Lập Trình.
