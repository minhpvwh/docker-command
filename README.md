# Tìm kiếm image trên hub
docker search <từ khóa>
# Xóa image
docker image rm <REPOSITORY>:<TAG>
docker image rm <IMAGE ID>
# Run docker
docker run -it <IMAGE ID>
docker run -it <REPOSITORY>:<TAG>
# Kiểm tra container đang chạy
docker ps
# Lấy tất cả các container đang chạy
docker ps -a
# Start container
docker start <IMAGE ID>
docker start <NAMES>
# truy cập lại container của docker đang chạy trên tab khác
docker attach <CONTAINER ID>
docker attach <NAMES>
# thoát container nhưng vẫn muốn container chạy
ctrl+p+q
# chạy đặt tên và host cho container
docker run -it --name <tên_đặt> -h <host_đặt> <REPOSITORY>:<TAG>
# muốn xóa container trong khi container đang chạy
docker rm -f <NAMES>
docker rm -f <CONTAINER ID>
# đứng ở ngoài mà vẫn muốn chạy lệnh ở trong container
docker exec <HOST> <command>
# kết nối terminal container
docker exec -it <HOST> bash
# build container thành image
docker commit <NAMES>
docker commit <CONTAINER ID> <IMAGE:TAG>
# build image ra file
docker save --output <path muốn lưu>/<tên nén>.rar <IMAGE ID>
# load file ra image
docker load -i <path lưu file image>
# đặt tag cho image or repository
docker tag <IMAGE ID> <đặt tên REPOSITORY>:<đặt tên TAG>

