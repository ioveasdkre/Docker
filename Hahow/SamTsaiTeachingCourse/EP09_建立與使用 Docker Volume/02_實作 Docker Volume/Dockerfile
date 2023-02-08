# 設定映像檔
FROM alpine:latest

# 設定共用變數
ENV myworkdir /var/www/localhost/htdocs/
# 設定參數
ARG whoami=Benson

# Define the working directory
WORKDIR ${myworkdir}

# 新增 apache2
RUN apk update && \
    apk add apache2 && \
    rm -rf /var/cache/apk/*

# 設置默認命令啟動apache2
ENTRYPOINT ["httpd", "-D", "FOREGROUND"] #預設啟動指令