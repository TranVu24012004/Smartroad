# Smartroad - Hệ thống Nhận diện Hư hỏng Mặt đường bằng AI

## 🚧 Giới thiệu

**Smartroad** là hệ thống quản lý và phát hiện hư hỏng đường bộ thông minh. Bằng cách ứng dụng trí tuệ nhân tạo (AI), hệ thống giúp tự động nhận diện, phân loại và đánh giá mức độ nghiêm trọng của các điểm hư hỏng (như ổ gà, vết nứt). Từ đó, cung cấp thông tin trực quan trên bản đồ giúp các cơ quan chức năng dễ dàng lên kế hoạch bảo trì.

### 🎯 Tính năng nổi bật

* **🤖 Nhận diện bằng AI:** Sử dụng các mô hình tiên tiến như YOLO và Vision Transformer (ViT) để phát hiện hư hỏng chính xác.
* **🗺️ Bản đồ tương tác:** Hiển thị trực tiếp các điểm báo cáo hư hỏng trên bản đồ với tọa độ rõ ràng.
* **⚡ Cập nhật theo thời gian thực:** Thông báo ngay lập tức khi có báo cáo mới.
* **📊 Bảng điều khiển (Dashboard):** Cung cấp biểu đồ thống kê và phân tích chi tiết về tình trạng đường bộ.
* **🔐 Bảo mật & Phân quyền:** Hệ thống đăng nhập an toàn, chia quyền rõ ràng cho từng nhóm người dùng.

---

## 🏗️ Công nghệ sử dụng

* **Frontend (Giao diện):** React, TailwindCSS (Thiết kế), React Leaflet (Bản đồ).
* **Backend (Máy chủ):** Node.js, Express, MongoDB (Lưu trữ dữ liệu).
* **AI/Machine Learning:** Python, YOLO (Khoanh vùng hư hỏng), ViT (Phân loại hư hỏng).

---

## 🚀 Hướng dẫn cài đặt nhanh

### Yêu cầu hệ thống

* Node.js 18+
* Python 3.8+
* MongoDB

### Các bước cài đặt

**1. Tải mã nguồn về máy**

```bash
git clone https://github.com/your-username/smartroad.git
cd smartroad

```

**2. Cài đặt thư viện cho giao diện (Frontend)**

```bash
npm install

```

**3. Cài đặt thư viện cho máy chủ (Backend)**

```bash
cd BACKEND
npm install

```

**4. Cài đặt thư viện cho AI (Python)**

```bash
pip install -r requirements.txt

```

**5. Cấu hình môi trường**
Tạo file `.env` ở thư mục gốc và điền các thông tin sau:

```env
MONGO_URI=mongodb://localhost:27017/Smartroad
PORT=5000
JWT_SECRET=khoa-bao-mat-cua-ban

```

**6. Chạy ứng dụng**
Mở 2 cửa sổ Terminal (dòng lệnh) khác nhau:

* **Terminal 1 (Chạy Frontend):** `npm run dev`
* **Terminal 2 (Chạy Backend):** `cd BACKEND` rồi gõ `npm start`

Trang web sẽ hoạt động tại: `http://localhost:5173`

---

## 👥 Vai trò người dùng

Hệ thống **Smartroad** được thiết kế cho 3 nhóm người dùng chính:

1. **🏠 Người dân:**
* Chụp và tải ảnh đường hỏng lên hệ thống.
* Xem các báo cáo.
* Theo dõi tiến độ xử lý.


2. **👨‍💼 Quản trị viên (Admin):**
* Duyệt các báo cáo từ người dân.
* Quản lý tài khoản người dùng.
* Xem bảng thống kê toàn hệ thống.


3. **🏛️ Cơ quan chức năng:**
* Xem danh sách các điểm cần sửa chữa theo mức độ ưu tiên.
* Điều phối và cập nhật trạng thái bảo trì.



---