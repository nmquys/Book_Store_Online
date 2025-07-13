# BookShopWeb

Dự án Java Web xây dựng một Shop Bán Sách

| (1)                                                                                                                                                   | (2)                                                                                                                                                      | (3)                                                                                                                                                    |
| ----------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <img src="https://user-images.githubusercontent.com/60851390/228592577-87976ca7-76c6-44c8-ab18-e664cce7493d.png" alt="Home" width="200" />            | <img src="https://user-images.githubusercontent.com/60851390/228592589-fa4302d4-a82e-4697-b22a-f84115885946.png" alt="Signup" width="200" />             | <img src="https://user-images.githubusercontent.com/60851390/228592594-fb3cec7c-7aac-47a4-8c4b-33a8792a2578.png" alt="Signin" width="200" />           |
| <img src="https://user-images.githubusercontent.com/60851390/228592602-8fe8fc00-89cb-4bc4-bb4b-b6c4e172dcfd.png" alt="Category" width="200" />        | <img src="https://user-images.githubusercontent.com/60851390/228592605-cf258cf4-3afe-4814-b649-2e5cfa3dc7f2.png" alt="Product" width="200" />            | <img src="https://user-images.githubusercontent.com/60851390/228592610-afc17126-f5da-45a2-b0b6-c4b89e39bf35.png" alt="Cart" width="200" />             |
| <img src="https://user-images.githubusercontent.com/60851390/228592611-c41f8048-48fc-45a4-82db-91e8f4dcc808.png" alt="User" width="200" />            | <img src="https://user-images.githubusercontent.com/60851390/228592615-1785a568-bc06-4556-a53b-3253dd782945.png" alt="Order" width="200" />              | <img src="https://user-images.githubusercontent.com/60851390/228592619-eb6d56ba-49ba-461a-9616-83926d3e794c.png" alt="Order Detail" width="200" />     |
| <img src="https://user-images.githubusercontent.com/60851390/228592622-47b20682-7314-4033-b35f-232630d2cf4b.png" alt="Wishlist" width="200" />        | <img src="https://user-images.githubusercontent.com/60851390/228592628-be226989-3b7d-4bca-9d8a-1cdfc60b6aca.png" alt="Search" width="200" />             | <img src="https://user-images.githubusercontent.com/60851390/228592633-fe3bc1c0-bfc8-4600-9cae-2038221bba9d.png" alt="Edit Review" width="200" />      |
| <img src="https://user-images.githubusercontent.com/60851390/228592634-df36905e-e377-442e-82f1-89eb5c921960.png" alt="Admin Dashboard" width="200" /> | <img src="https://user-images.githubusercontent.com/60851390/228592637-09d61699-6f0e-404b-b32b-e969ab864e78.png" alt="Product Management" width="200" /> | <img src="https://user-images.githubusercontent.com/60851390/228592639-3cc4767f-ce03-4521-a7de-9f993d4cbe2c.png" alt="Create Product" width="200" />   |
| <img src="https://user-images.githubusercontent.com/60851390/228592645-0ffedb14-78d6-47c2-9577-59a802159251.png" alt="Update Product" width="200" />  | <img src="https://user-images.githubusercontent.com/60851390/228592649-c7325684-cf12-406d-9fc7-b4980b668c7d.png" alt="Review Management" width="200" />  | <img src="https://user-images.githubusercontent.com/60851390/228592653-99341b4d-f200-4890-b556-a59bccefb789.png" alt="Order Management" width="200" /> |

## A. Set up project BookShopWeb



### 1. Tạo database

Mở MySQL Workbench → Open SQL Script → Execute [bookshopdb.sql](https://github.com/nmquys/Book_Store_Online/blob/master/init/bookshopdb.sql)

### 2. Nạp project vào IDEA

Mở IDEA → Get from VCS (màn hình Welcome) hoặc File → New → Project from Version Control (màn hình bình thường) → Clone project theo URL: https://github.com/nmquys/Book_Store_Online.git

### 3. Cấu hình Tomcat

- Edit Configurations  →  Add new configurations  →  Tomcat Local  → Application Server: Tomcat 10.1.39
- Fix: war exploded
  
-> Apply

### 4. Run (Shift+F10)

## B. Cấu hình utils.ConstantUtils
Theo mặc định: 
-	DB_PORT là 3306 nếu sử dụng MySQL
-	SERVER_NAME là localhost
-	DB_NAME là bookshopdb
-	DB_USERNAME là root
-	DB_PASSWORD là 12345
-	IMAGE_PATH là nơi để folder var_webapp_images vd: D:\\Web_J2EE\\BookShopWeb\\init\\var-webapp-images.
  
  (Có thể thay đổi nếu như khác)


# Sơ đồ CSDL

![DatabaseDesignBSW](https://user-images.githubusercontent.com/60851390/184755435-bb97a62a-4cdd-408d-9a5a-526430f50c64.svg)

## Dữ liệu mẫu

| Bảng             | Số lượng record mẫu |
| ---------------- | ------------------- |
| user             | 5                   |
| product          | 100                 |
| product_review   | 150                 |
| category         | 15                  |
| product_category | 100                 |
| cart             | 2                   |
| cart_item        | 5                   |
| orders           | 25                  |
| order_item       | 60                  |
| wishlist_item    | 30                  |

# Cấu hình phần mềm

- IntelliJ IDEA 2024.3.4.1 trở lên
- MySQL Workbench 8.0
- Tomcat 10.1 trở lên (Vì dưới 10.1 sẽ bị lỗi thư viện)
- Oracle OpenJDK 23.0.2 (MS JDK 11 sẽ bị lỗi)

