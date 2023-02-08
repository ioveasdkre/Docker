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

# 將內容添加到 index.html 文件中
RUN echo "<h3>I am ${whoami}. Iam taking this great Docker Course. Round 01<h3>" >> index.html && \
	echo "<h3>I am ${whoami}. Iam taking this great Docker Course. Round 02<h3>" >> index.html && \
	echo "<h3>I am ${whoami}. Iam taking this great Docker Course. Round 03<h3>" >> index.html

# 設置維護者標籤
LABEL maintainer="MyName"

# 設置默認命令啟動apache2
ENTRYPOINT ["httpd", "-D", "FOREGROUND"] #預設啟動指令