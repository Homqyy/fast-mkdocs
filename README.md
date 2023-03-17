# fast-mkdocs
基于mkdcos快速创建个人网站

## 快速运行

运行以下命令，完成后用浏览器访问8000端口：

```
docker-compose up -d
```

## 编写自己的文章

首先将个人的Markdown的文章放到`docs`目录下

1. 构建markdown文章

```
docker-compose run --rm mkdocs build
```

2. 本地运行

```
docker-compose run --rm mkdocs serve
```
