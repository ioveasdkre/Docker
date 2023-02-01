FROM alpine:latest
#RUN echo "I am in the image building process..." #輸出
#RUN ls -l / #列出資料夾內的所有檔案
RUN apk --update add apache2
RUN rm -rf /var/cache/apk/*
ENTRYPOINT ["httpd", "-D", "FOREGROUND"] #預設啟動指令