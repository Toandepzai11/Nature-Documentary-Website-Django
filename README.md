Django Project: Trinh Huu Phuc Toan's Website
Overview
This project is built using Django with two main applications:

app: The core of the website, featuring the homepage and various extended pages with a dynamic navigation bar.
accounts: Manages user authentication, including signup and login functionalities.
Project Structure
app: Contains the main template (base.html), which includes a dynamic navbar that updates based on user login status.
accounts: Handles user registration and login. User data is stored in a Supabase database.
Setup
Prerequisites
Ensure you have Django installed by running:

bash
Copy code
pip install django
Database Configuration
This project uses Supabase for the database. You need the following details from your Supabase project:

DATABASE_NAME: Found after the last / in the connection string.
USER: The part before the first : in the connection string.
PASSWORD: The part between the first : and the @ symbol.
HOST: The part between the @ and the first : after it.
PORT: Typically 5432 for PostgreSQL.
Add these credentials to your settings.py file under the DATABASES configuration.

Installed Apps
The app and accounts applications must be added to the INSTALLED_APPS section of your settings.py file.
URL Configuration
The accounts app is included in the urls.py file located in the main project folder.
Templates
The base.html file located in the app directory contains the layout of the website and includes a dynamic navbar.
Running the Project
Apply Migrations:

bash
Copy code
python manage.py migrate
Create a Superuser (for admin access):

bash
Copy code
python manage.py createsuperuser
Run the Development Server:

bash
Copy code
python manage.py runserver
Access the Website: Open your browser and navigate to http://127.0.0.1:8000/ to view the homepage.

Notes
This project uses Django's built-in authentication system.
Ensure your templates and static files are properly set up according to Django’s guidelines.
License
This project is licensed under the MIT License. See the LICENSE file for more details.

Dự Án Django: Trang Web Của Trịnh Hữu Phúc Toàn
Tổng Quan
Dự án này được xây dựng bằng Django với hai ứng dụng chính:

app: Phần cốt lõi của trang web, bao gồm trang chủ và nhiều trang mở rộng khác với thanh điều hướng động.
accounts: Quản lý việc xác thực người dùng, bao gồm chức năng đăng ký và đăng nhập.
Cấu Trúc Dự Án
app: Chứa mẫu chính (base.html), bao gồm thanh điều hướng động cập nhật theo trạng thái đăng nhập của người dùng.
accounts: Quản lý việc đăng ký và đăng nhập người dùng. Dữ liệu người dùng được lưu trữ trong cơ sở dữ liệu Supabase.
Hướng Dẫn Cài Đặt
Yêu Cầu
Đảm bảo rằng bạn đã cài đặt Django bằng cách chạy:

bash
Copy code
pip install django
Cấu Hình Cơ Sở Dữ Liệu
Dự án này sử dụng Supabase cho cơ sở dữ liệu. Bạn cần các thông tin sau từ dự án Supabase của mình:

DATABASE_NAME: Phần sau cùng của chuỗi kết nối.
USER: Phần trước dấu : đầu tiên trong chuỗi kết nối.
PASSWORD: Phần giữa dấu : đầu tiên và ký hiệu @.
HOST: Phần giữa @ và dấu : đầu tiên sau nó.
PORT: Thông thường là 5432 cho PostgreSQL.
Thêm các thông tin này vào tệp settings.py trong phần cấu hình DATABASES.

Ứng Dụng Đã Cài Đặt
Thêm app và accounts vào mục INSTALLED_APPS trong tệp settings.py.
Định Tuyến URL
Ứng dụng accounts đã được thêm vào tệp urls.py trong thư mục dự án chính.
Mẫu
Tệp base.html nằm trong thư mục app chứa bố cục của trang web và bao gồm thanh điều hướng động.
Chạy Dự Án
Áp Dụng Di Chuyển:

bash
Copy code
python manage.py migrate
Tạo Tài Khoản Quản Trị (để truy cập admin):

bash
Copy code
python manage.py createsuperuser
Khởi Động Máy Chủ Phát Triển:

bash
Copy code
python manage.py runserver
Truy Cập Trang Web: Mở trình duyệt và truy cập http://127.0.0.1:8000/ để xem trang chủ.

Ghi Chú
Dự án này sử dụng hệ thống xác thực tích hợp của Django.
Đảm bảo rằng các mẫu và tệp tĩnh của bạn được cấu hình chính xác theo tài liệu của Django.
Giấy Phép
Dự án này được cấp phép theo giấy phép MIT. Xem tệp LICENSE để biết thêm chi tiết.

