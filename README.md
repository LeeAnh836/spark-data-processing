# Spark API - Data Processing Projects

Bộ tài liệu tập thực hành xử lý dữ liệu lớn sử dụng Apache Spark trên nền tảng Databricks. Các bài tập được thiết kế để giúp học viên nắm vững các kỹ năng cốt lõi trong xử lý dữ liệu phân tán.

---

## 📋 Danh sách các File

### 1. **TH_1_preview.ipynb** 
**Chủ đề:** Scala Collection Operations
- **Nội dung:** Giới thiệu cơ bản về xử lý dữ liệu với Scala
- **Bài tập:** 
  - Bình phương phần tử trong danh sách (map)
  - Lọc số lẻ và lập phương (filter, map)
  - Tính toán giá trị trung bình, trung vị
  - Tìm số nguyên lớn thứ 2
  - Tính độ dài từ trong danh sách chuỗi
- **Kỹ năng:** map, filter, sorted, groupBy, maxBy
- **Output:** Các giá trị số và danh sách Tuple

---

### 2. **TH2_upload_DBFS.ipynb** 
**Chủ đề:** Text Processing & Word Frequency Analysis
- **Nội dung:** Xử lý dữ liệu văn bản từ DBFS (Databricks File System)
- **Bài tập:**
  - Đếm số từ trong từng đoạn văn
  - Loại bỏ các từ phổ biến (stopwords)
  - Tính tần suất từ, xác định top 10 từ phổ biến nhất
  - Tìm từ có tần suất cao nhất trong mỗi đoạn văn
- **Kỹ năng:** Text parsing, groupBy, frequency analysis, sorting
- **Data Source:** Text file từ DBFS

---

### 3. **TH3_Spark_Dataframe.ipynb** 
**Chủ đề:** Spark DataFrame Operations với JSON Data
- **Nội dung:** Làm việc với dữ liệu JSON và thao tác DataFrame cơ bản
- **Bài tập:**
  - Đọc file JSON (1M.json) từ DBFS
  - Lọc bản ghi có speed > 0
  - Đếm số ProviderId duy nhất
  - Trích xuất biển số xe tỉnh và thống kê số lượng
  - Gọi API Nominatim để lấy tên địa điểm từ tọa độ GPS
- **Kỹ năng:** read JSON, filter, count, groupBy, API integration
- **Data Source:** 1M.json (file dữ liệu xe/GPS)

---

### 4. **TH4_Read_CSV.ipynb** 
**Chủ đề:** Reading CSV Files with Custom Schema
- **Nội dung:** Đọc file CSV với cấu hình tùy chỉnh và định nghĩa schema
- **Bài tập:**
  - Đọc file CSV với delimiter `;` (thay vì dấu phẩy mặc định)
  - Định nghĩa custom schema cho 21 cột dữ liệu
  - Kiểm tra và xác nhận kiểu dữ liệu
- **Kỹ năng:** spark.read.csv, custom delimiter, StructType, schema definition
- **Data Source:** full.csv (bank marketing dataset)
- **Columns:** age, job, marital, education, default, housing, loan, contact, month, dayOfWeek, duration, campaign, pdays, previous, poutcome, emVarRate, consPriceIdx, consConfIdx, euribor3m, nrEmployed, y

---

### 5. **TH5_Spark_Dataframe.ipynb** 
**Chủ đề:** Advanced DataFrame Analytics - NYC Taxi Data
- **Nội dung:** Phân tích dữ liệu chuyến đi taxi tại New York từ bảng tích hợp Databricks
- **Bài tập:**
  - Tính tiền trung bình cho chuyến đi > 2 miles
  - Tính thời gian trung bình chuyến đi
  - Tìm cặp zip code có quãng đường trung bình cao nhất
  - Hiển thị top 3 chuyến đi đắt tiền theo từng cặp zip code
  - Tính doanh thu theo ngày trong tuần
  - Join dữ liệu CSV tên quận với bảng trips
  - Tính doanh thu theo quận (borough)
- **Kỹ năng:** aggregation, join, window function, groupBy, sorting
- **Data Source:** samples.nyctaxi.trips (Databricks sample table)

---

### 6. **TH7_WriteFile.ipynb** 
**Chủ đề:** ETL Pipeline - Data Cleaning & Writing Files
- **Nội dung:** Thiết kế luồng ETL để làm sạch dữ liệu nhân viên và ghi ra các định dạng khác nhau
- **Bài tập:**
  - Đọc file nhân viên từ DBFS
  - Thống kê độ tuổi nhân viên (tính từ ngày sinh)
  - Tạo cột fullName, chuẩn hóa kiểu chữ, loại bỏ trùng lặp
  - Chuẩn hóa dữ liệu SSN (số bảo hiểm xã hội)
  - Ghi dữ liệu ra multiple format (CSV, Parquet, JSON) với compression
- **Kỹ năng:** data cleaning, deduplication, string manipulation, write with different formats/compression
- **Output Formats:** CSV, Parquet (snappy), JSON (gzip)
- **Data Source:** people-with-dups.txt

---

### 7. **TH8_Review.ipynb** 
**Chủ đề:** Comprehensive Review - Complex Data Aggregation
- **Nội dung:** Bài tập tổng hợp kỹ năng với dữ liệu sự kiện e-commerce
- **Bài tập:**
  - Đọc file JSON từ GitHub với schema phức tạp (nested structures)
  - Tính trung bình doanh thu (purchase_revenue) theo user_id
  - Các bài tập tiếp theo chưa được mô tả đầy đủ
- **Kỹ năng:** complex schema parsing, nested structures, groupBy aggregation, window functions
- **Data Source:** Events data từ GitHub (e-commerce transactions)
- **Schema:** Includes device, ecommerce (struct), items (array), geo (struct)

---

---

## 🎯 Kỹ năng Chính được Học

- ✨ **Scala Collections:** map, filter, sorted, groupBy, maxBy, distinct
- ✨ **Spark DataFrame:** read, select, filter, groupBy, join, aggregation
- ✨ **Data Formats:** JSON, CSV, Parquet, TXT
- ✨ **Data Processing:** text parsing, frequency analysis, deduplication, normalization
- ✨ **ETL Concepts:** data cleaning, transformation, loading, multiple output formats
- ✨ **File Systems:** DBFS, local file systems
- ✨ **Advanced Features:** nested structures, window functions, API integration

---

## 📝 Lưu ý

- Các file Scala (.ipynb) chạy trên Databricks platform
- Cần bật cluster Databricks để truy cập dữ liệu sample tables
- Một số file cần tải dữ liệu từ Google Classroom
- File TH8_Review tải dữ liệu động từ GitHub API
