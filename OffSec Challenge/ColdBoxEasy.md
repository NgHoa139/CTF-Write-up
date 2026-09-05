# ColdBoxEasy

- Bài lab cho chúng ta một địa chỉ IP : ```192.168.52.239``` yêu cầu chúng ta tìm kiếm người dùng và leo quyền để lấy được flag. 
<img width="304" height="165" alt="image" src="https://github.com/user-attachments/assets/f61b6b0d-a1be-4910-b71f-ceb1836c8a67" />

- Sau khi truy cập trang web chúng ta thử dùng wpscan bằng câu lệnh : wpscan --url http://192.168.52.239/ -e
<img width="846" height="515" alt="image" src="https://github.com/user-attachments/assets/0f272200-74b9-43cc-ba69-d85f03f8028b" />

- Ta có thể thấy các user có khả năng đăng nhập được do có phần login error : **c0ldd, hugo, philip**
- Ta tiến hành brute-force user c0ldd bằng file rockyou.txt : wpscan --url http://192.168.52.239/ -U c0ldd -P /home/kali/Downloads/rockyou-master/rockyou.txt
<img width="854" height="284" alt="image" src="https://github.com/user-attachments/assets/453cc3e4-fa39-4add-8b88-8313592f83b7" />

- Ta có được tài khoản và mật khẩu ta đăng nhập vào trang web 
