# Описание

Docker-compose настроен таким образом, чтобы все данные складывались в соотвествующие директории для сервисов и данные переживали включение/выключение контейнеров.

# Запуск

## Все сервисы/БД

```
docker-compose up -d
```

## Выборочный запуск

```
docker-compose up postgres -d 
```

# Отключение контейнеров

```
docker-compose down
```

# Подключение к работающему контейнеру (по label из docker-compose)

```
docker exec -it dockerdev_postgres_1 bash
```