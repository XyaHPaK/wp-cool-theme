Windows

1. Установить node.js , если еще не установлен. Проверить установлен ли node на вашем
компьютере можно через команду в консоли/терминале:
node -v
Если он установлен в консоли отобразиться версия среды. В противном случаи скачиваем
актуальную LTS версию - https://nodejs.org/en/ и во время установки обязательно убедиться что
npm manger включен
2. Устанавливаем node-sass, инструмент для компиляции scss файлов. В командной строке
пропишем данную команду:
npm i node-sass -g (для MacOS добавляем sudo)
Тем самым мы установим node-sass глобально, а не только для данного проекта (флаг -g) и
сможем его запускать в любой папке.
3. Устанавливаем browser-sync, инструмент позволяющий вести разработке в реальном времени,
перезагрузка браузера происходит автоматически:
npm i browser-sync -g (для MacOS добавляем sudo)
4. Устанавливаем postcss, пакет, который в дальнейшем позволит запустить автопрефиксер
npm i postcss -g (для MacOS добавляем sudo)
5. Устанавливаем postcss-cli, пакет-надстройка для пакета выше, что дает возможность им
управлять через командную строку
npm i postcss-cli -g (для MacOS добавляем sudo)
6. Устанавливаем autoprefixer, данный пакета проставляет вендорные префиксы для всех
необходимых свойств, в зависимости от указанных поддерживаемых браузеров
npm i autoprefixer -g (для MacOS добавляем sudo)
7. Базовая настройка компьютера закончена, теперь переходим в проект. Для работы установленных
инструментов нам понадобиться 2 файла package.json (файл с заготовленными скриптами для
вотчинга изменений в файлах стилей и для запуска локального сервера) и bs-config.js (настройки
для локального сервера).

MacOS

1. Чтобы установить node на мак сначала необходимо скачать и установить node version manager
a. Находясь в домашней директории (~ user$) создать файл:
touch .bash_profile
b. После этого установить сам менеджер:

curl -o-
https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh |

bash
Если во время установки не было ошибок, можно проверить работоспособность пакета:
nvm -v
c. И уже после этого установить последнюю актуальную версию node:
nvm install --lts

2. Далее продолжить установка аналогично с Windows
