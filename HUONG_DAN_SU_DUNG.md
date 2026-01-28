# 📚 Hướng dẫn sử dụng Trợ lý Soạn Giáo án STEM Toán học

## 🌐 Cách 1: Sử dụng trực tuyến (Dành cho giáo viên)

### Bước 1: Truy cập link website
Giáo viên chỉ cần mở trình duyệt và truy cập link:
```
https://your-app-name.streamlit.app
```
*(Link này sẽ có sau khi deploy)*

### Bước 2: Sử dụng ứng dụng
1. **Nhập thông tin bài dạy** ở sidebar bên trái:
   - Chọn khối lớp (6, 7, 8, 9)
   - Nhập tên bài dạy (VD: Thiết kế kim tự tháp)
   - Chọn chu trình STEM
   - Chọn thời lượng
   - Nhập kiến thức nền Toán học
   - Nhập sản phẩm dự kiến

2. **Nhấn nút** "🚀 Bắt đầu soạn giáo án chuẩn 3089"

3. **Tải xuống** file Word bằng nút "📥 Tải xuống File Word (.docx)"

---

## 🚀 Cách 2: Deploy lên Streamlit Cloud (Dành cho người quản trị)

### Bước 1: Chuẩn bị
- Đảm bảo code đã được push lên GitHub
- Có tài khoản GitHub

### Bước 2: Deploy
1. Truy cập: https://streamlit.io/cloud
2. Đăng nhập bằng GitHub
3. Nhấn "New app"
4. Chọn repository: `honguyenquynhnhu84-prog/hotrothietkebaidaystem`
5. Branch: `main`
6. Main file: `streamlit_app.py`
7. Nhấn "Deploy"

### Bước 3: Cấu hình API Key (BẮT BUỘC)
1. Trong dashboard Streamlit Cloud, chọn app của bạn
2. Nhấn "⚙️ Settings" → "Secrets"
3. Thêm vào:
```toml
GOOGLE_API_KEY = "AIzaSyASQaA7s1vw_269h2HD5HAb4qXvC_i3RsU"
```
4. Nhấn "Save"

### Bước 4: Chia sẻ
- Lấy link ứng dụng (VD: `https://your-app-name.streamlit.app`)
- Chia sẻ link này cho giáo viên

---

## 💻 Cách 3: Chạy trên máy tính cá nhân

### Yêu cầu:
- Python 3.11 trở lên
- Internet để gọi API

### Các bước:

1. **Clone repository:**
```bash
git clone https://github.com/honguyenquynhnhu84-prog/hotrothietkebaidaystem.git
cd hotrothietkebaidaystem
```

2. **Tạo môi trường ảo:**
```bash
python -m venv .venv
source .venv/bin/activate  # Linux/Mac
# hoặc
.venv\Scripts\activate  # Windows
```

3. **Cài đặt thư viện:**
```bash
pip install -r requirements.txt
pip install google-generativeai
```

4. **Cấu hình API Key:**
Tạo file `.streamlit/secrets.toml` với nội dung:
```toml
GOOGLE_API_KEY = "your-api-key-here"
```

5. **Chạy ứng dụng:**
```bash
streamlit run streamlit_app.py
```

6. **Mở trình duyệt:** http://localhost:8502

---

## 🔑 Lấy Google API Key

1. Truy cập: https://makersuite.google.com/app/apikey
2. Đăng nhập Google
3. Nhấn "Create API Key"
4. Copy API key và dán vào file secrets.toml

---

## 📝 Tính năng chính

✅ Soạn giáo án STEM theo chuẩn CV 3089/BGDĐT-GDTrH  
✅ Hỗ trợ 5 hoạt động dạy học STEM  
✅ Tự động tạo phiếu học tập và rubric đánh giá  
✅ Xuất file Word chuẩn định dạng  
✅ Tối ưu cho giáo dục Toán học THCS  

---

## ❓ Gặp lỗi?

**Lỗi: "API Key không hợp lệ"**
- Kiểm tra lại API key trong file secrets.toml
- Đảm bảo API key còn quota sử dụng

**Lỗi: "Module not found"**
```bash
pip install google-generativeai
```

**Ứng dụng chạy chậm**
- Do AI đang xử lý, vui lòng đợi 30-60 giây

---

## 📧 Liên hệ hỗ trợ

Nếu gặp vấn đề, vui lòng tạo Issue trên GitHub hoặc liên hệ người phát triển.
