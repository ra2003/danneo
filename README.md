# danneo
Danneo CMS 1.5.5 (Next)

Модульная, мультиязычная, мультисайтовая, мультиплатформенная, с открытым исходным 
кодом, система управления сайтами.

Простая установка, легкость в управлении, минимальная нагрузка на сервер, а так же 
широкая базовая комплектация позволяет построить интерактивный веб-сайт любой сложности, 
и в дальнейшем эффективно им управлять.

Распространяется в соответствии с лицензией GNU General Public 2.
http://danneo.ru/license

ВОЗМОЖНОСТИ
-----------
http://danneo.ru/feature

БАЗОВЫЕ МОДУЛИ
--------------
http://danneo.ru/modules


СИСТЕМНЫЕ ТРЕБОВАНИЯ
--------------------
База данных MySQL версии 5.0 или выше.
Интерпретатор PHP версии 5.3 или выше, предпочтительно установленный как модуль (mod_php).
Обязательные модули и расширения: GD, Zlib, ZIP, cURL, mbString, JSON.

Подробнее: http://danneo.ru/requirements


УСТАНОВКА
=========
1. Распаковать архив, загрузить файлы и папки на сервер.
2. Установить права на запись (777) для файлов и папок:
   cache/
   up/
   core/config.php
3. В браузере ввести http://ваш_сайт/setup/
4. Далее следовать инструкциям установки.


ОБНОВЛЕНИЕ
==========
1. Сделать резервную копию файла: core/config.php
2. Распаковать архив, загрузить файлы и папки из каталога www на сервер (с заменой).
3. Восстановить файл core/config.php из резервной копии.
4. В браузере ввести http://ваш_сайт/setup/
5. Далее следовать инструкциям установки.

!!! ВАЖНО !!!
При обновлении, выполнить 1 и 3 пункты в логической последовательности.


СПИСОК ИЗМЕНЕНИЙ
================
29 Июня 2017
1. Исправлена ошибка сохранения ключевых слов (поле keywords), при редактировании новости.
2. Изменения в функционале хлебных крошек (навигационная цепочка).
    Для удобства работы с шаблоном, первый пункт перенесен из функциональной части в шаблон.
    Название первого пункта изменено, теперь по умолчанию, это "Главная", вместо названия сайта.
    Название, а также оформление данного пункта можно изменить непосредственно в шаблоне:
    template/Lite/breadcrumb.tpl

3 Июня 2017
1. Исправлено кеширование блочных позиций.
2. Исправлена ошибка проверки артикула при пересохранении товара.
3. Исправлены ошибки при добавлении Доп. поля "Многострочное текстовое поле", в каталоге товаров.

23 Мая 2017
1. Добавлен класс Video, импорт данных видео из популярных сервисов.
2. Доработан класс Image. Добавлены методы urlimg(), tmpfile(), unique(), url_thumb().

18 Мая 2017
1. Исправлена ошибка в расчете доставки, в каталоге товаров.
2. Исправлена ошибка добавления фото в моде Фотогалерея. Не сохранялись теги.
3. Исправлен вывод ссылок в Фотогалерее (на сайте), в разделе "Поделиться". Изменены относительные на прямые.

4 Мая 2017
1. Исправлена ошибка листинга (постраничной разбивки) в разделе "Перелинковка", в панели управления.
2. Исправлено форматирование цены свойства price стандарта schema.org, в каталоге товаров.
3. Доработки в настройках валют, в каталоге товаров.
    а) В поле "Разделитель тысячных" добавлен пункт "Пробел".
    б) В поле "Количество знаков после запятой" добавлена возможность указывать 0 или пусто.

14 Апреля 2017

Модуль "Организации" для Danneo
https://github.com/NukeVlad/dn-mod-firms

Добавлена возможность отправки SMS-сообщений в сети мобильных операторов.
Создан функционал для работы с API онлайн сервисов SMS-центр и SMS.RU
Сервис включен в виде отдельного нода "Сервисы SMS", в разделе "Управление системой".
1. Общие настройки
    а) Включить SMS оповещение (Да / Нет).
    б) Выбрать сервис SMS
2. Отдельные страницы настроек для сервисов SMS-центр и SMS.RU
    С подробными описаниями методов классов, а также проверок работы сервиса.

ДОПОЛНИТЕЛЬНЫЕ МОДУЛИ
================
Модуль "Тендеры" для Danneo CMS
https://github.com/NukeVlad/dn-mod-tender

Модуль "Организации" для Danneo
https://github.com/NukeVlad/dn-mod-firms

Модуль "Отзывы" для Danneo CMS 1.5.1 (Next)
https://github.com/NukeVlad/dn-mod-respond

ФОРУМ ПОДДЕРЖКИ
================
http://forum.danneo.ru

Надеемся, что наши разработки окажутся полезными для вас!
Danneo Team.
