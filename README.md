# BÁO CÁO BÀI TẬP: KIỂM THỬ TỰ ĐỘNG VỚI SELENIUM

## 1. Kịch Bản Kiểm Thử (Test Cases)

Bài tập thực hiện kiểm thử tự động trên website: https://www.saucedemo.com/

| Mã TC | Tên Chức Năng              | Các Bước Thực Hiện                                                                                                                                                                                       | Kết Quả Mong Đợi                                                           | Trạng Thái |
| ----- | -------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------- | ---------- |
| TC01  | Đăng nhập thành công       | 1. Truy cập trang đăng nhập. <br> 2. Nhập username `standard_user`. <br> 3. Nhập password `secret_sauce`. <br> 4. Nhấn nút **Login**.                                                                    | Hệ thống đăng nhập thành công và chuyển đến trang **Products**.            | PASSED     |
| TC02  | Tìm kiếm sản phẩm          | 1. Đăng nhập vào hệ thống. <br> 2. Nhập từ khóa tìm kiếm hoặc kiểm tra danh sách sản phẩm. <br> 3. Tìm sản phẩm **Sauce Labs Backpack**.                                                                 | Sản phẩm **Sauce Labs Backpack** được hiển thị trong danh sách sản phẩm.   | PASSED     |
| TC03  | Thêm sản phẩm vào giỏ hàng | 1. Đăng nhập vào hệ thống. <br> 2. Nhấn nút **Add to cart** của sản phẩm Sauce Labs Backpack. <br> 3. Kiểm tra số lượng hiển thị trên biểu tượng giỏ hàng. <br> 4. Mở giỏ hàng và kiểm tra tên sản phẩm. | Giỏ hàng hiển thị số lượng **1** và chứa sản phẩm **Sauce Labs Backpack**. | PASSED     |

---

## 2. Kết Quả Thực Hiện

Sau khi chạy chương trình, Selenium tự động mở trình duyệt Google Chrome và thực hiện lần lượt 03 test case:

* TC01: Đăng nhập thành công.
* TC02: Tìm kiếm sản phẩm.
* TC03: Thêm sản phẩm vào giỏ hàng.

Kết quả kiểm thử:

```text
test_login_success ........ PASSED
<img width="1919" height="1138" alt="image" src="https://github.com/user-attachments/assets/01e1c25a-9f85-4dba-b731-a80a48dc5991" />

test_search_product ....... PASSED
<img width="1919" height="1142" alt="image" src="https://github.com/user-attachments/assets/ef695fbf-1c61-44e7-a909-bf33193a4793" />

test_add_product_to_cart .. PASSED
<img width="1918" height="1137" alt="image" src="https://github.com/user-attachments/assets/fb5e53ec-9dcb-4c6f-bb67-487e6379111c" />

```

Tất cả các test case đều thực hiện thành công và đạt trạng thái PASSED.

---

## 6. Kết Luận

Bài tập đã áp dụng Selenium WebDriver kết hợp với Pytest để xây dựng các kịch bản kiểm thử tự động cho website SauceDemo. Các chức năng được kiểm thử bao gồm:

* Đăng nhập hệ thống.
* Tìm kiếm/kiểm tra hiển thị sản phẩm.
* Thêm sản phẩm vào giỏ hàng.

Kết quả cho thấy các chức năng hoạt động đúng theo yêu cầu và toàn bộ test case đều đạt trạng thái PASSED.
