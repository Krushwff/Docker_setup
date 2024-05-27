<h1>Докер контейнер для работы с Laravel</h1>
<li><b>docker compose build</b> - используем для сборки образов Docker</li>
<li><b>make up</b> - вводим для запуска контейнера(docker compose up)</li>
<h2>Для установки Laravel</h2>
<li><b>make cli</b> - вводим для доступа к вводу php команд в терминале (docker compose exec php-cli bash)</li>

<li><b>compose create-project laravel/laravel example-app</b> - используем для создания Laravel</li>
<li><b>exit</b> - используем для выхода из доступа к php в терминале</li>
<li><b>mv example-app/* ./</b> - переносим все файлы из папки example-app в корневую</li>
<li><b>mv example-app/.* ./</b> - переносим все файлы с точкой из папки example-app в корневую</li>
<li><b>ls example-app</b> - проверяем папку example-app на содержимое файлов</li>
<li><b>rm -rf example-app</b> - удаляем папку example-app</li>
<li><b>sudo chmod 777 -R storage</b> - делаем так, что любой пользователь d системе может читать, писать и выполнять файлы в каталоге storage и во всех его подкаталогах и файлах.</li>
