<h1>Bài tập nhỏ Kiến Trúc Thiết Kế Phần Mềm</h2>
<h2>Đề tài: User-Post</h4>
<h4>Mô tả: Code backend spring boot sử dụng Microservice</h4>
<h3>Thành viên:</h3>
<ul>
    <li>Võ Anh Hào - 18060441 -Nhóm trưởng</li>
    <li>Võ Quốc Khánh – 18058521</li>
    <li>Nguyễn Hoàng Lâm - 18058151</li>
    <li>Tằng Tiến Đạt - 18061351</li>
    <li>Nguyễn Thị Hoàng Nhi - 18068061</li>
</ul>
<h3>Sử dụng:</h3>
<ul>
    <li>Service call User</li>
    <li>Retry</li>
    <li>Ratelimiter</li>
    <li>Service discovery eureka client-service</li>
    <li>API gateway</li>
    <li>Cloud Confgi service</li>
    <li>Heroku, AWS</li>
    <li>Cache Redis</li>
    <li>JWT</li>
    <li>UI</li>
</ul>
 <h3>Mô tả cấu trúc:</h3>
 <img stype="width:100%" src="https://f20-group-zf.zdn.vn/8ec1002bfecf119148de/3234134756995282069"/>

<h3>Link demo: https://www.youtube.com/watch?v=EC5_lrbLVF4</h3>
<h3>Test:</h3>
<h4>-EC2: http://18.136.126.140</h4>
<h4>-EC2: http://18.142.162.108</h4>
<h4>-Heroku: https://eurekaredis.herokuapp.com/login</h4>
<h4>Euroka: http://18.136.126.140:8761/</h4>
<h4>Get all user không jwt (jwt cho post,delete): http://18.136.126.140:8000/user/</h4>
<h4>Cloud config: http://18.136.126.140:8888/</h4>
<h4>Lấy all post: http://18.142.162.108:8001/post/</h4>
<h4>Lấy all post có redis: http://18.142.162.108:8001/post/redis/ (Lần đầu chậm từ lần sau nhanh)</h4>
<h4>Lấy all post có retry: http://18.142.162.108:8001/post/retry/ (Ấn liên tục sẽ bị chậm do ratelimiter bên user gây error, post phải retry lại)</h4>
<h4>Euroka: http://18.136.126.140:8761/</h4>
<h4>API gateway: http://18.142.162.108:9191</h4>

User chỉ có relimiter cho getuserbyID lỗi timeout thì sẽ retry lại bên post

