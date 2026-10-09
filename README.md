# Báo Cáo Thực Hành: Kiểm Thử API Bằng Postman

- **Họ và tên:** Tuyển Hoàng Trung
- **Mã số sinh viên:** 23010188
- **Tài liệu tham khảo:** [Postman Api Testing Tutorial for beginners - Codemify](https://www.youtube.com/watch?v=MFxk5BZulVU)

---

## 1. Giới thiệu tổng quan
Báo cáo ghi lại quy trình thực hành kiểm thử API cơ bản bằng công cụ Postman, bao gồm tạo Collection, gửi Request kiểm tra mã phản hồi (Status Code), cấu hình tham số truy vấn (Query Params), viết kịch bản kiểm thử tự động (Test Script) và thực thi bộ kiểm thử thông qua Collection Runner.

---

## 2. Các bước thực hiện & Kết quả minh họa

### Bước 1: Khởi tạo Collection và Request
Tạo collection `Postman Test Demo` và cấu hình Request GET gửi tới endpoint API.

![Tạo Request](images/01_collection_request.png.png)

---

### Bước 2: Gửi Request và phân tích Response
Gửi request và nhận kết quả phản hồi với mã trạng thái `200 OK`, dữ liệu trả về theo định dạng JSON Pretty.

![Kết quả Response](images/02_get_response.png.png)

---

### Bước 3: Thêm tham số Query Parameters
Cấu hình Query Params `page=2` để lọc và phân trang dữ liệu trả về từ máy chủ.

![Cấu hình Parameters](images/03_params.png.png)

---

### Bước 4: Viết Test Script tự động
Viết script kiểm tra mã phản hồi trả về bằng JavaScript trong tab Scripts/Tests. Kết quả kiểm thử đạt trạng thái `PASSED`.

![Viết Test Script](images/04_test_script.png.png)

---

### Bước 5: Chạy kiểm thử tự động với Collection Runner
Sử dụng công cụ Collection Runner để thực thi tự động toàn bộ danh sách request trong Collection. Toàn bộ các kiểm thử đều vượt qua (All tests passed).

![Chạy Collection Runner](images/05_runner_result.png.png)

---

## 3. Đánh giá và Kết luận
- **Ưu điểm:** Postman hỗ trợ giao diện trực quan, dễ thao tác gửi nhận dữ liệu và hỗ trợ tự động hóa kiểm thử nhanh chóng bằng JavaScript.
- **Kết quả đạt được:** Nắm vững cấu trúc HTTP Request/Response, cách quản lý kịch bản kiểm thử theo Collection và thực thi kiểm thử hồi quy tự động với Runner.
