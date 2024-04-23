FROM nginx:latest

# 设置作者信息
LABEL Author xiaolou

# 复制nginx.conf文件到容器内部
COPY default.conf /etc/nginx/conf.d/default.conf

# 将dist目录中的文件拷贝到nginx的html目录下
COPY dist/ /usr/share/nginx/html/
COPY dist/css/ /usr/share/nginx/html/css/
COPY dist/js/ /usr/share/nginx/html/js/

# 指定容器运行时使用的端口号
EXPOSE 8489