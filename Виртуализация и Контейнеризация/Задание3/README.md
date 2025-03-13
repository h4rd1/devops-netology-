
Задача 1

Сценарий выполнения задачи:

    Установите docker и docker compose plugin на свою linux рабочую станцию или ВМ.
    Если dockerhub недоступен создайте файл /etc/docker/daemon.json с содержимым: {"registry-mirrors": ["https://mirror.gcr.io", "https://daocloud.io", "https://c.163.com/", "https://registry.docker-cn.com"]}
    Зарегистрируйтесь и создайте публичный репозиторий с именем "custom-nginx" на https://hub.docker.com (ТОЛЬКО ЕСЛИ У ВАС ЕСТЬ ДОСТУП);
    скачайте образ nginx:1.21.1;
    Создайте Dockerfile и реализуйте в нем замену дефолтной индекс-страницы(/usr/share/nginx/html/index.html), на файл index.html с содержимым:

<html>
<head>
Hey, Netology
</head>
<body>
<h1>I will be DevOps Engineer!</h1>
</body>
</html>

    Соберите и отправьте созданный образ в свой dockerhub-репозитории c tag 1.0.0 (ТОЛЬКО ЕСЛИ ЕСТЬ ДОСТУП).
    Предоставьте ответ в виде ссылки на https://hub.docker.com/<username_repo>/custom-nginx/general .

![{0F98537F-C490-4CB3-90BB-9A8222437A1F}](https://github.com/user-attachments/assets/7eb47bc5-664d-4862-90a9-0f15e6c79ec7)

image [доступен h4rdl/kapustin-netology:1.0.0](https://hub.docker.com/repository/docker/h4rdl/kapustin-netology/general)

Задача 2

    Запустите ваш образ custom-nginx:1.0.0 командой docker run в соответвии с требованиями:

    имя контейнера "ФИО-custom-nginx-t2"
    контейнер работает в фоне
    контейнер опубликован на порту хост системы 127.0.0.1:8080

    Не удаляя, переименуйте контейнер в "custom-nginx-t2"
    Выполните команду date +"%d-%m-%Y %T.%N %Z" ; sleep 0.150 ; docker ps ; ss -tlpn | grep 127.0.0.1:8080  ; docker logs custom-nginx-t2 -n1 ; docker exec -it custom-nginx-t2 base64 /usr/share/nginx/html/index.html
    Убедитесь с помощью curl или веб браузера, что индекс-страница доступна.

В качестве ответа приложите скриншоты консоли, где видно все введенные команды и их вывод.


