# nginx-php-fpm

## 构建
```sh
docker build -t web .
```

## 拉去镜像
```sh
// 国外
docker pull johnstevin/nginx-php-fpm
// 国内
docker pull registry.cn-hangzhou.aliyuncs.com/cool2rong/nginx-php-fpm:1.0.3
```

## 本地项目目录结构

- /html/\<project\>/

## 创建容器
```sh
docker run -d -p 80:80 -v /Users/pro/nginx-php-fpm/html/:/var/www/html/ --name web johnstevin/nginx-php-fpm
// 或者
docker run -d -p 80:80 -p 81:81 -v /Users/pro/Develop/html/xiaoshuo/:/var/www/html/ --name web-xiaoshuo  --privileged=true registry.cn-hangzhou.aliyuncs.com/cool2rong/nginx-php-fpm:1.0.5
```