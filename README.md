# nginx-php-fpm

## 构建
```sh
docker build -t web .
```

## 拉去镜像
```sh
docker pull johnstevin/nginx-php-fpm
```

## 创建容器
```sh
docker run -d -p 80:80 -v /Users/pro/nginx-php-fpm/html/:/var/www/html/ --name web johnstevin/nginx-php-fpm
```