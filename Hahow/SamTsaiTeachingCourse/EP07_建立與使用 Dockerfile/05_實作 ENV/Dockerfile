FROM alpine:latest
MAINTAINER MyName
ENV myworkdir /var/www/localhost/htdocs #設定共用變數
RUN apk --update add apache2
RUN rm -rf /var/cache/apk/*
RUN cd ${myworkdir} \
	&& echo "<h3>I am Sam. Iam taking this great Docker Course. Round 01</h3>" >> index.html
RUN cd ${myworkdir} \
	&& echo "<h3>I am Sam. Iam taking this great Docker Course. Round 02</h3>" >> index.html
RUN cd ${myworkdir} \
	&& echo "<h3>I am Sam. Iam taking this great Docker Course. Round 03</h3>" >> index.html
	
ENTRYPOINT ["httpd"] #預設啟動指令
CMD ["-D", "FOREGROUND"]