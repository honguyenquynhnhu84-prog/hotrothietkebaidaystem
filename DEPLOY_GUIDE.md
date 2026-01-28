# 🚀 Hướng dẫn Deploy lên Streamlit Cloud

## Bước 1: Truy cập Streamlit Cloud
Truy cập: https://share.streamlit.io/

## Bước 2: Đăng nhập
- Click **"Sign in"**
- Chọn **"Continue with GitHub"**
- Cấp quyền cho Streamlit Cloud truy cập repository

## Bước 3: Tạo ứng dụng mới
1. Click nút **"New app"**
2. Điền thông tin:
   - **Repository:** `honguyenquynhnhu84-prog/hotrothietkebaidaystem`
   - **Branch:** `main`
   - **Main file path:** `streamlit_app.py`

## Bước 4: ⚠️ QUAN TRỌNG - Thêm Secrets (API Key)
1. Click vào **"Advanced settings"** ở dưới cùng
2. Trong phần **"Secrets"**, thêm nội dung sau:

```toml
GOOGLE_API_KEY = "AIzaSyBSiIHKvvsY2EzMLZkkDY-Vw-hvTgYiPmU"
```

3. Click **"Save"**

## Bước 5: Deploy
- Click nút **"Deploy!"**
- Chờ 2-3 phút để Streamlit cài đặt dependencies và khởi động ứng dụng

## Kết quả
Bạn sẽ nhận được URL công khai dạng:
```
https://your-app-name.streamlit.app
```

## Lưu ý
- ✅ File `secrets.toml` đã được bảo vệ bởi `.gitignore` nên không bị đẩy lên GitHub
- ✅ API Key chỉ tồn tại trên Streamlit Cloud, an toàn và bảo mật
- ✅ Mỗi lần bạn push code mới lên GitHub, Streamlit Cloud sẽ tự động cập nhật ứng dụng

## Nếu gặp lỗi
1. Kiểm tra lại phần **Secrets** có đúng format không
2. Đảm bảo không có khoảng trắng thừa trong API Key
3. Xem logs để biết lỗi cụ thể (click vào nút "Manage app" > "Logs")
