# Настройка Docker для работы с Laravel
<h2>Важно</h2>

>Перед работой проекта необходимо поменять названия для будущей БД
https://github.com/Krushwff/Docker_setup/blob/05dea06017d30ea565bfa34b94d1049907c8ffed/docker-compose.yml#L56

<b>Используем для сборки образов Docker<b>
```sh
docker compose build
```
<b>Для запуска контейнера(docker compose up)<b>
```sh
make up
```
<h2>Для установки Laravel</h2>

>ВАЖНО после создания проекта Laravel нужно изменить название БД в файле .env и добавить пароль 'secret'.

<b>Вводим следующую команду для доступа к вводу php команд в терминале (docker compose exec php-cli bash)<b>
```sh
make cli
```
<b>Используем для создания проекта Laravel<b>
```sh
composer create-project laravel/laravel example-app
```
<b>Вводим следующую команду для выхода из доступа к php<b>
```sh
exit
```
<b>Переносим все файлы из папки example-app в корневую<b>
```sh
mv example-app/* ./
```
<b>Преносим все файлы с точкой из папки example-app в корневую<b>
```sh
mv example-app/.* ./
```
<b>Проверяем папку example-app на содержимое файлов<b>
```sh
ls example-app
```
<b>Удаляем папку example-app<b>
```sh
rm -rf example-app
```
<b>Делаем так, что любой пользователь d системе может читать, писать и выполнять файлы в каталоге storage и во всех его подкаталогах и файлах.<b>
```sh
sudo chmod 777 -R storage
```
