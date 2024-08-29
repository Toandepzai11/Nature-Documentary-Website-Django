Django Project: Trinh Huu Phuc Toan's Website
Project Overview
This Django project consists of two main applications:
    app: The homepage application that includes the main layout (navbar) and various extended pages.

    accounts: The application responsible for user signup and login functionalities.

Project Structure
app:
Contains the main layout (base.html), which includes a navbar and extends other pages.
Handles the general content of the website.

accounts:
Manages user authentication (signup and login).
User information is stored in the db.sqlite3 file under the "auth_user" table.



Setup
Prerequisites
Ensure you have Django installed. You can install Django using pip:

pip install django
Configuration
Database:

The project uses SQLite as the database, which is configured in settings.py.
Installed Apps:

app: Added to the INSTALLED_APPS list in settings.py.
accounts: Added to the INSTALLED_APPS list in settings.py.
URLs Configuration:

The accounts app is included in the urls.py of the project folder (line 22).
Templates:

The base.html file is located in the templates folder within the app directory. It includes a navbar that checks if a user is logged in or not.
Running the Project
Apply Migrations:

python manage.py migrate
Create a Superuser (for admin access):

python manage.py createsuperuser
Run the Development Server:

python manage.py runserver
Access the Website:

Open a web browser and navigate to http://127.0.0.1:8000/ to view the homepage.
THIS WEBSITE IS USING supabase DATABASE 
NAME: The database name, after the last / in the connection string.
USER: The part before the first : in the connection string.
PASSWORD: The part between the first : and the @ symbol.
HOST: The part between the @ and the first : after it.
PORT: The number after the : following the host (typically 5432 for PostgreSQL).
Notes
The project uses Django's built-in authentication system for user management.
Ensure you have the necessary templates and static files set up as per Django’s documentation.
License
This project is licensed under the MIT License. See the LICENSE file for more details.





*****************************************************************************************




Welcome to Trinh Huu Phuc Toan's Django Project!
Overview
Welcome to the project by Trinh Huu Phuc Toan! This Django-based website is built with two main apps:

app: This is the core of the website, featuring the homepage and various extended pages. It includes a dynamic navbar for seamless navigation.
accounts: This app manages user authentication, including signup and login functionalities. All user data is securely stored in the db.sqlite3 database.
Project Structure
app:

Contains base.html, the main template for the site’s layout, which features a responsive navbar.
Includes other pages that extend base.html to provide a consistent look and feel across the site.
accounts:

Handles user registration and login.
User credentials are stored in the auth_user table within the db.sqlite3 database.
Setup Instructions
Prerequisites
Make sure Django is installed. If it’s not, you can install it using pip install django.

Configuration
Database:

The project uses SQLite, which is configured in settings.py.
Installed Apps:

app and accounts are both listed in INSTALLED_APPS in settings.py.
URL Routing:

The accounts app is included in the project's urls.py file (see line 22).
Templates:

base.html is located in the templates folder within the app directory. It features a dynamic navbar that updates based on user login status.
Getting Started
Apply Migrations:

Run python manage.py migrate to set up the database.
Create a Superuser:

Run python manage.py createsuperuser to create an admin account.
Start the Development Server:

Run python manage.py runserver to start the server.
Visit Your Site:

Open a web browser and go to http://127.0.0.1:8000/ to see the homepage.
Notes
This project uses Django's built-in authentication system for managing users.
Ensure your templates and static files are set up according to Django’s guidelines.
License
This project is licensed under the MIT License. See the LICENSE file for details.

*****************************************************************************************
***************************** VIETNAMESE*************************************************

Dưới đây là bản dịch README sang tiếng Việt:

Chào mừng đến với Dự án Django của Trịnh Hữu Phúc Toàn!
Tổng Quan
Chào mừng đến với dự án của Trịnh Hữu Phúc Toàn! Trang web dựa trên Django này được xây dựng với hai ứng dụng chính:

app: Đây là phần cốt lõi của trang web, bao gồm trang chính và các trang mở rộng khác. Nó bao gồm một thanh điều hướng động để người dùng dễ dàng điều hướng.
accounts: Ứng dụng này quản lý xác thực người dùng, bao gồm chức năng đăng ký và đăng nhập. Tất cả dữ liệu người dùng được lưu trữ an toàn trong cơ sở dữ liệu db.sqlite3.
Cấu Trúc Dự Án
app:

Chứa base.html, mẫu chính cho giao diện của trang web, bao gồm thanh điều hướng đáp ứng.
Bao gồm các trang khác mở rộng base.html để cung cấp giao diện nhất quán trên toàn trang web.
accounts:

Quản lý việc đăng ký và đăng nhập người dùng.
Thông tin người dùng được lưu trữ trong bảng auth_user của cơ sở dữ liệu db.sqlite3.
Hướng Dẫn Cài Đặt
Yêu Cầu
Đảm bảo rằng Django đã được cài đặt. Nếu chưa, bạn có thể cài đặt nó bằng cách sử dụng pip install django.

Cấu Hình
Cơ Sở Dữ Liệu:

Dự án sử dụng SQLite, được cấu hình trong settings.py.
Ứng Dụng Đã Cài Đặt:

app và accounts đều được liệt kê trong INSTALLED_APPS trong settings.py.
Định Tuyến URL:

Ứng dụng accounts được bao gồm trong tệp urls.py của dự án (xem dòng 22).
Mẫu:

base.html nằm trong thư mục templates của thư mục app. Nó có thanh điều hướng động cập nhật dựa trên trạng thái đăng nhập của người dùng.
Bắt Đầu
Áp Dụng Di Chuyển:

Chạy python manage.py migrate để thiết lập cơ sở dữ liệu.
Tạo Tài Khoản Quản Trị:

Chạy python manage.py createsuperuser để tạo tài khoản quản trị.
Khởi Động Máy Chủ Phát Triển:

Chạy python manage.py runserver để khởi động máy chủ.
Truy Cập Trang Web:

Mở trình duyệt web và truy cập http://127.0.0.1:8000/ để xem trang chính.
CÓ THỂ THAY ĐỔI USER BẰNG CÁCH VÀO ADMIN CỦA WEB
Ghi Chú
Dự án này sử dụng hệ thống xác thực tích hợp sẵn của Django để quản lý người dùng.
Đảm bảo rằng các mẫu và tệp tĩnh của bạn được thiết lập theo hướng dẫn của Django.
Giấy Phép
Dự án này được cấp phép theo Giấy phép MIT. Xem tệp LICENSE để biết chi tiết.

*****************************************************************************************
*****************************************************************************************
*****************************************************************************************
Chào mừng đến với Dự án Django của Trịnh Hữu Phúc Toàn!
Tổng Quan
Chào mừng đến với dự án của Trịnh Hữu Phúc Toàn! Trang web dựa trên Django này được xây dựng với hai ứng dụng chính:

app: Đây là phần cốt lõi của trang web, bao gồm trang chính và các trang mở rộng khác. Nó bao gồm một thanh điều hướng động để người dùng dễ dàng điều hướng.
accounts: Ứng dụng này quản lý xác thực người dùng, bao gồm chức năng đăng ký và đăng nhập. Tất cả dữ liệu người dùng được lưu trữ an toàn trong cơ sở dữ liệu db.sqlite3.
Cấu Trúc Dự Án
app:

Chứa base.html, mẫu chính cho giao diện của trang web, bao gồm thanh điều hướng đáp ứng.
Bao gồm các trang khác mở rộng base.html để cung cấp giao diện nhất quán trên toàn trang web.
accounts:

Quản lý việc đăng ký và đăng nhập người dùng.
Thông tin người dùng được lưu trữ trong bảng auth_user của cơ sở dữ liệu db.sqlite3.
Hướng Dẫn Cài Đặt
Yêu Cầu
Đảm bảo rằng Django và các tiện ích mở rộng cần thiết đã được cài đặt. Bạn có thể cài đặt Django bằng cách sử dụng pip install django.

Tiện Ích Mở Rộng
Django Extensions: Cung cấp các công cụ và tiện ích bổ sung cho Django. Cài đặt bằng lệnh pip install django-extensions.
SQLite: Cơ sở dữ liệu được sử dụng trong dự án. Không cần cài đặt riêng biệt vì nó được tích hợp sẵn với Django.
Cấu Hình
Cơ Sở Dữ Liệu:

Dự án sử dụng SQLite, được cấu hình trong settings.py.
Ứng Dụng Đã Cài Đặt:

app và accounts đều được liệt kê trong INSTALLED_APPS trong settings.py.
Định Tuyến URL:

Ứng dụng accounts được bao gồm trong tệp urls.py của dự án (xem dòng 22).
Mẫu:

base.html nằm trong thư mục templates của thư mục app. Nó có thanh điều hướng động cập nhật dựa trên trạng thái đăng nhập của người dùng.
Bắt Đầu
Áp Dụng Di Chuyển:

Chạy python manage.py migrate để thiết lập cơ sở dữ liệu.
Tạo Tài Khoản Quản Trị:

Chạy python manage.py createsuperuser để tạo tài khoản quản trị.
Khởi Động Máy Chủ Phát Triển:

Chạy python manage.py runserver để khởi động máy chủ.
Truy Cập Trang Web:

Mở trình duyệt web và truy cập http://127.0.0.1:8000/ để xem trang chính.
Ghi Chú
Dự án này sử dụng hệ thống xác thực tích hợp sẵn của Django để quản lý người dùng.
Đảm bảo rằng các mẫu và tệp tĩnh của bạn được thiết lập theo hướng dẫn của Django.
Giấy Phép
Dự án này được cấp phép theo Giấy phép MIT. Xem tệp LICENSE để biết chi tiết.