# Контейнеризация семинары №5


![](https://github.com/nadushka89/docker_3/blob/main/source/docker.jpg?raw=true)

## Урок 5. Docker Compose и Docker Swarm

Задание:
1) создать docker compose файл, состоящий из 2 различных контейнеров: 1 - веб, 2 - БД
2) запустить docker compose файл
3) по итогу на БД контейнере должно быть 2 реплики, на админере должна быть 1 реплика. Всего должно получиться 3 контейнера
4) выводы зафиксировать

**Задание:**

Создадим в папке файл docker-compose.yml, Dockerfile.
В Dockerfile пропишем:

![](https://github.com/nadushka89/docker_5/blob/main/source/6.png)

В docker-compose.yml пропишем

![](https://github.com/nadushka89/docker_5/blob/main/source/5.png)

Запустим сервисы, определенные в файле docker-compose.yml, с помощью Docker Compose:


```
docker compose up
```
![](https://github.com/nadushka89/docker_5/blob/main/source/1.png)

Проверим запустились ли контейнеры:

```
docker ps
```

![](https://github.com/nadushka89/docker_5/blob/main/source/2.png)

Зайдем в браузер и проверим запустился ли Adminer (который был прописан в файле docker-compose.yml)

![](https://github.com/nadushka89/docker_5/blob/main/source/4.png)

![](https://github.com/nadushka89/docker_5/blob/main/source/3.png)