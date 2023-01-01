FROM ubuntu:20.04
RUN apt update && apt install -y python3
WORKDIR /var/www/html
CMD ["python3", "-u", "-m", "http.server"]
# COPY ["index.html", "."] 
# host index.html copy to WORKDIR path

# RUN 빌드가 되는 시점에 실행되는 명령어, 이미지에 반영
# CMD 컨테이너가 실행될떄 실행됨, 컨터이너에 반영
#     자동으로 실행하기 싫을떄
#     run할떄 pwd하고 쳐면 된다.
#     CMD 대신 PWD가 실행된다.(overriding)

# docker build -t web-server-build .;
# docker rm --force web-server;
# docker run -p 8888:8000 --name web-server web-server-build pwd;
# docker run -p 8888:8000 --name web-server web-server-build