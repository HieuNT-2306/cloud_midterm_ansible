FROM mongo:latest

# Thiết lập biến môi trường cho MongoDB
ENV MONGO_INITDB_ROOT_USERNAME=admin
ENV MONGO_INITDB_ROOT_PASSWORD=password

# Tạo thư mục để chứa script khởi tạo
WORKDIR /docker-entrypoint-initdb.d

# Copy script khởi tạo vào thư mục
COPY ./init-mongo.js .

# Chạy MongoDB khi container được khởi động
CMD ["mongod"]