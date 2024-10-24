### Сборка образа

```
docker build ./ --tag webpython:0.0.1
```

### Запуск контейнера

```
docker run --name my_app -d -p 8000:8000 webpython:0.0.1
```