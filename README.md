# 📐 Trợ lý Soạn Giáo án STEM Toán học (CV 3089)

Ứng dụng web hỗ trợ giáo viên Toán học THCS soạn giáo án STEM theo Công văn 3089/BGDĐT-GDTrH một cách nhanh chóng và chuyên nghiệp.

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://streamlit.io)

## ✨ Tính năng

- ✅ **Soạn giáo án tự động** theo chuẩn CV 3089/BGDĐT-GDTrH
- ✅ **5 hoạt động STEM đầy đủ**: Xác định vấn đề → Nghiên cứu → Thiết kế → Chế tạo → Chia sẻ
- ✅ **Tích hợp AI Gemini** để tạo nội dung chất lượng
- ✅ **Xuất file Word** với định dạng chuẩn Times New Roman, cỡ 13
- ✅ **Tự động tạo** phiếu học tập và rubric đánh giá
- ✅ **Giao diện thân thiện** dễ sử dụng cho giáo viên

## 🚀 Demo nhanh

**Link ứng dụng:** [Sẽ có sau khi deploy]

## 📋 Hướng dẫn sử dụng cho Giáo viên

### Bước 1: Truy cập website
Mở trình duyệt và truy cập link ứng dụng

### Bước 2: Nhập thông tin
- Chọn khối lớp (6, 7, 8, 9)
- Nhập tên bài dạy (VD: Thiết kế cầu tre, Đo chiều cao cây...)
- Chọn chu trình STEM (Kỹ thuật hoặc Khoa học)
- Chọn thời lượng (1-3 tiết)
- Nhập kiến thức Toán học trọng tâm
- Nhập sản phẩm dự kiến

### Bước 3: Tạo giáo án
Nhấn nút **"🚀 Bắt đầu soạn giáo án"** và đợi 30-60 giây

### Bước 4: Tải xuống
Nhấn **"📥 Tải xuống File Word"** để lưu giáo án

## 🛠️ Cài đặt cho Developer

### Yêu cầu
- Python 3.11+
- Google API Key (Gemini)

### Các bước cài đặt

1. **Clone repository:**
```bash
git clone https://github.com/honguyenquynhnhu84-prog/hotrothietkebaidaystem.git
cd hotrothietkebaidaystem
```

2. **Tạo môi trường ảo:**
```bash
python -m venv .venv
source .venv/bin/activate  # Linux/Mac
.venv\Scripts\activate     # Windows
```

3. **Cài đặt dependencies:**
```bash
pip install -r requirements.txt
pip install google-generativeai
```

4. **Cấu hình API Key:**

Tạo file `.streamlit/secrets.toml`:
```toml
GOOGLE_API_KEY = "your-api-key-here"
```

Lấy API key tại: https://makersuite.google.com/app/apikey

5. **Chạy ứng dụng:**
```bash
streamlit run streamlit_app.py
```

Mở trình duyệt tại: http://localhost:8502

## 🌐 Deploy lên Streamlit Cloud

1. Push code lên GitHub
2. Truy cập https://streamlit.io/cloud
3. Đăng nhập và chọn "New app"
4. Chọn repository này
5. Thêm `GOOGLE_API_KEY` vào Secrets
6. Deploy!

Chi tiết: [HUONG_DAN_SU_DUNG.md](HUONG_DAN_SU_DUNG.md)

## 📦 Cấu trúc dự án

```
hotrothietkebaidaystem/
├── streamlit_app.py          # File chính của ứng dụng
├── requirements.txt           # Danh sách thư viện
├── .streamlit/
│   └── secrets.toml          # API keys (không commit)
├── README.md                  # Tài liệu này
├── HUONG_DAN_SU_DUNG.md     # Hướng dẫn chi tiết
└── LICENSE                    # Giấy phép
```

## 🎯 Công nghệ sử dụng

- **Streamlit** - Framework web Python
- **Google Gemini AI** - AI tạo nội dung
- **python-docx** - Xuất file Word
- **Python 3.11** - Ngôn ngữ lập trình

## 📝 Giấy phép

MIT License - Xem file [LICENSE](LICENSE) để biết thêm chi tiết

## 🤝 Đóng góp

Mọi đóng góp đều được chào đón! Vui lòng:
1. Fork repository
2. Tạo branch mới (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Tạo Pull Request

## 📧 Liên hệ

Nếu có câu hỏi hoặc cần hỗ trợ, vui lòng tạo Issue trên GitHub.

---

**Phát triển bởi:** honguyenquynhnhu84-prog  
**Mục đích:** Hỗ trợ giáo viên Toán học THCS trong việc soạn giáo án STEM
