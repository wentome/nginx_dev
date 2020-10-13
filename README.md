# nginx_dev
cd nginx-1.14.2

./configure --prefix=/opt/soft/nginx  --with-http_ssl_module --add-module=../echo-nginx-module-0.62rc1

make  && make install 
