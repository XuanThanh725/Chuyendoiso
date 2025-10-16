<h2 align="center">
    <a href="https://www.hoaphat.com.vn">
    💼 TẬP ĐOÀN HÒA PHÁT
    </a>
</h2>

<h2 align="center">
   HỆ THỐNG PHÂN TÍCH DỮ LIỆU DOANH NGHIỆP HÒA PHÁT
</h2>

<div align="center">
    <p align="center">
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b7/Logo_Hoaphat_Group.svg/512px-Logo_Hoaphat_Group.svg.png" alt="HoaPhat Logo" width="180"/>
      <img src="https://img.shields.io/badge/Power%20BI-yellow?style=for-the-badge&logo=powerbi" alt="Power BI"/>
      <img src="https://img.shields.io/badge/SQL-blue?style=for-the-badge&logo=postgresql" alt="SQL"/>
      <img src="https://img.shields.io/badge/Visual%20Studio%20Code-0078d7?style=for-the-badge&logo=visualstudiocode" alt="VS Code"/>
      <img src="https://img.shields.io/badge/Python-3776ab?style=for-the-badge&logo=python" alt="Python"/>
      <img src="https://img.shields.io/badge/Java-orange?style=for-the-badge&logo=java" alt="Java"/>
    </p>
</div>

---

## 📖 1. Giới thiệu hệ thống

Dự án **Phân tích dữ liệu Công ty Hòa Phát** được xây dựng nhằm:
- Thu thập, xử lý và trực quan hóa dữ liệu **kinh doanh, tài chính, sản xuất và nhân sự**.
- Cung cấp các **dashboard Power BI** giúp lãnh đạo dễ dàng nắm bắt **tình hình hoạt động, lợi nhuận, doanh số, tồn kho, nhân sự** theo thời gian thực.
- Hỗ trợ ra quyết định bằng **dữ liệu trực quan và báo cáo thông minh**.

Hệ thống gồm 3 thành phần chính:
1. **Cơ sở dữ liệu (SQL Server / PostgreSQL)** – lưu trữ dữ liệu chi tiết.
2. **Backend xử lý dữ liệu (Python / Java)** – làm sạch, tổng hợp và xuất sang Power BI.
3. **Dashboard Power BI** – trình bày dữ liệu dạng biểu đồ, bảng tương tác, bản đồ, KPI.

---

## 🔧 2. Công nghệ sử dụng

| Công nghệ | Mô tả |
|------------|-------|
| 🐍 **Python 3.10+** | Dùng để xử lý dữ liệu, tự động hoá import/export dữ liệu sang Power BI |
| ☕ **Java** | Viết các module nghiệp vụ: quản lý nhân sự, đơn hàng, sản phẩm |
| 💾 **SQL Server / PostgreSQL** | Lưu trữ dữ liệu và truy vấn thống kê |
| 📊 **Power BI** | Tạo dashboard, biểu đồ doanh thu, chi phí, sản lượng |
| 💻 **Visual Studio Code** | IDE chính để lập trình và quản lý dự án |
| 🔄 **Power Query / Pandas** | Làm sạch, chuẩn hoá dữ liệu |

---

## 📈 3. Các bảng dữ liệu chính trong SQL

| Bảng | Mô tả |
|------|-------|
| `DoanhThu` | Doanh thu từng tháng / chi nhánh |
| `SanPham` | Danh sách sản phẩm, mã, nhóm hàng |
| `NhanSu` | Nhân viên, bộ phận, lương, năng suất |
| `Kho` | Tồn kho theo chi nhánh |
| `ChiPhi` | Chi phí vận hành, nguyên vật liệu |
| `KPI` | Chỉ số hiệu suất từng phòng ban |

---

## 🚀 4. Mô hình hoạt động

```text
[SQL Database] ---> [Python xử lý dữ liệu] ---> [Power BI Dashboard]
                       ↑
                       |
                   [Java module]
hoaphat_bi_project/
│
├── sql/
│   ├── create_tables.sql
│   ├── insert_data.sql
│
├── python/
│   ├── data_cleaning.py
│   ├── export_to_excel.py
│
├── java/
│   ├── src/
│   │   ├── main.java
│   │   └── kpi_module.java
│
├── powerbi/
│   ├── hoaphat_dashboard.pbix
│
├── requirements.txt
└── README.md
