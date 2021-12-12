#euroka
http://18.136.126.140:8761/
#get all user ko jwt
http://18.136.126.140:8000/user/
#cloud config
http://18.136.126.140:8888/
#relimiter cho get user by id 
http://18.136.126.140:8000/user/retry/1

#lấy post có redis
http://18.142.162.108:8001/post/redis/
#lấy post có retry
http://18.142.162.108:8001/post/retry/
#lấy post kiểu bt nhưng có giới hạn khi spam
http://18.142.162.108:8001/post/
#api gateway
http://18.142.162.108:9191
#UI

UI không sử dụng retry, redis:
https://eurekaredis.herokuapp.com/login

bên post đều có relimiter,retry chỗ có uri retry
bên user thì chỉ có relimiter cho getuserbyID
