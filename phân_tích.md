
Phần 1 : phân tích 

- Dựa vào đoạn code thì trong requestMatchers đang là ("/).premisAll() nên chấp nhận mọi request đi  vào mà không kiểm tra role
- và Quy tắc .anyRequest().authenticated() chỉ yêu cầu người dùng đăng nhập là đủ, không kiểm tra vai trò
 ->  Vì vậy, sau khi đăng nhập bằng tài khoản "user" (role USER), người dùng vẫn có thể truy cập /admin/orders

















