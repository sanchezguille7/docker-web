FROM nginx

WORKDIR /usr/share/nginx/html/

RUN apt update \
    && apt install git -y

RUN git clone https://github.com/josejuansanchez/2048.git && mv 2048/* .

EXPOSE 80

ENTRYPOINT [ "nginx", "-g", "daemon off;" ]