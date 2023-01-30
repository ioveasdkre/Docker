指令
docker container ls									列出所有在執行的容器
docker container ls	-a								列出本地所有容器
docker container stop containerID					停止運作容器
docker logout										登出
docker login										登入
docker images										查詢本地所有映像檔
docker push image名稱								推送到遠端庫
docker rmi image名稱								清理本地映像檔
docker rmi -f image名稱								強制清理本地映像檔
docker rm 本地conatiner								刪除本地容器
dokcer container run -d —name 命名 image檔			容器持續執行映像檔
dokcer run -d —name 命名 image檔					容器持續執行映像檔
dokcer run -d —name 命名 image檔 tail -f /dev/null	容器持續執行映像檔(持續追蹤 file的 log)
docker exce -it containerID /bin/sh					容器內執行 PowerShell
