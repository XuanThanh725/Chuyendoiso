<h2 align="center">
    <a href="https://dainam.edu.vn/vi/khoa-cong-nghe-thong-tin">
    🎓 Faculty of Information Technology (DaiNam University)
    </a>
</h2>
<h2 align="center">
    HỆ THỐNG PHÂN TÍCH TÀI CHÍNH HÒA PHÁT – WEB FLASK + POWER BI
</h2>
<div align="center">
    <p align="center">
        <img alt="Logo Hòa Phát" width="160" src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/88/Hoaphat_logo.svg/800px-Hoaphat_logo.svg.png" />
        <img alt="DaiNam University Logo" width="180" src="https://github.com/user-attachments/assets/77fe0fd1-2e55-4032-be3c-b1a705a1b574" />
        <img alt="Python Flask Logo" width="160" src="https://www.vectorlogo.zone/logos/pocoo_flask/pocoo_flask-ar21.svg" />
    </p>

[![AIoTLab](https://img.shields.io/badge/AIoTLab-green?style=for-the-badge)](https://www.facebook.com/DNUAIoTLab)
[![Faculty of Information Technology](https://img.shields.io/badge/Faculty%20of%20Information%20Technology-blue?style=for-the-badge)](https://dainam.edu.vn/vi/khoa-cong-nghe-thong-tin)
[![DaiNam University](https://img.shields.io/badge/DaiNam%20University-orange?style=for-the-badge)](https://dainam.edu.vn)

</div>

---

## 📖 1. Giới thiệu hệ thống
Dự án **Phân tích tài chính Tập đoàn Hòa Phát (HPG)** được xây dựng nhằm đánh giá hiệu quả hoạt động kinh doanh giai đoạn **2019–2023**, thông qua các báo cáo:
- Báo cáo kết quả kinh doanh  
- Bảng cân đối kế toán  
- Báo cáo lưu chuyển tiền tệ  

Hệ thống gồm hai phần chính:
- **Web Flask**: hiển thị giao diện doanh nghiệp, sản phẩm, tin tức, báo cáo tài chính và dashboard BI.
- **Power BI Dashboard**: trình bày dữ liệu trực quan, phân tích xu hướng tài chính theo thời gian.

Trang web giúp người dùng theo dõi **doanh thu, lợi nhuận, tài sản, nợ, ROA, ROE, dòng tiền**, hỗ trợ việc **phân tích dữ liệu và ra quyết định kinh doanh**.

---

## 🔧 2. Công nghệ sử dụng
#### 💻 Ngôn ngữ & Framework:
- **Python 3.11 + Flask** – xử lý backend và định tuyến trang  
- **HTML5 / CSS3 / Bootstrap 5** – thiết kế giao diện hiện đại  
- **JavaScript** – tạo tương tác động  
- **Power BI Embedded** – tích hợp dashboard tài chính trực quan  
- **Pandas / Numpy** – xử lý dữ liệu tài chính

#### 💾 Cơ sở dữ liệu:
- SQLite / PostgreSQL dùng để lưu trữ thông tin doanh nghiệp, báo cáo và sản phẩm.

#### 📊 Dữ liệu tài chính:
- Dữ liệu 5 năm (2019–2023) gồm doanh thu, lợi nhuận, EPS, tài sản, nợ phải trả, vốn chủ và lưu chuyển tiền tệ (CFO, CFI, CFF).

---

## 🚀 3. Cấu trúc & Cài đặt hệ thống
#### Cấu trúc thư mục:
```
hoaphat_bi_flask/
│
├── app.py                 # File Flask chính
├── requirements.txt       # Danh sách thư viện
├── static/                # CSS, JS, hình ảnh
├── templates/             # Giao diện HTML
├── data/                  # File dữ liệu (CSV/JSON)
└── venv/                  # Môi trường ảo
```

#### Cài đặt:
1️⃣ **Tạo môi trường ảo và cài thư viện**
```bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```

2️⃣ **Chạy web Flask**
```bash
python app.py
```

3️⃣ **Mở trình duyệt**:  
👉 http://127.0.0.1:5000  

---

## 💡 4. Giao diện và Dashboard
<p align="center">
  <img src="picture/1.png" alt="Trang chủ Hòa Phát" width="800"/>
  <em>Hình 1: Trang chủ website Hòa Phát</em>
</p>

<p align="center">
  <img src="picture/2.png" alt="Trang giới thiệu" width="800"/>
  <em>Hình 2: Trang giới thiệu tầm nhìn và sứ mệnh</em>
</p>


<p align="center">
  <img src="picture/bctc.png" alt="Báo cáo tài chính" width="800"/>
  <em>Báo cáo kết quả kinh doanh, bảng cân đối kế toán và lưu chuyển tiền tệ</em>
</p>

---
## 🧮 5. Tính năng chính
- Hiển thị **chuỗi giá trị luyện thép khép kín**  
- Cập nhật **tin tức Hòa Phát mới nhất**  
- Trình bày **báo cáo tài chính 5 năm** (2019–2023)  
- Phân tích **chỉ số ROA, ROE, EPS, D/E, biên lợi nhuận**  
- Dashboard Power BI giúp **theo dõi dữ liệu theo thời gian thực**

---

