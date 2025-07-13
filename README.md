# BookShopWeb

Dự án Java Web xây dựng một Shop Bán Sách



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

