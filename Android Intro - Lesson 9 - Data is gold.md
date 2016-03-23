# Занятие 9. Хранение информации.

1. Preferences
2. SQLite
3. Работа с файлами

## Что нужно знать
### SQLite
Есть два основных способа доступа к БД в Андроид:
1. Доступ к БД напрямую с помощью [SQLiteOpenHelper](http://developer.android.com/intl/ru/training/basics/data-storage/databases.html). 
2. Доступ с помощью [ContentProvider](http://developer.android.com/intl/ru/guide/topics/providers/content-providers.html). Мы будем рассматривать его в будущем, но можно уже ознакомиться.
Замечательный гайд еще тут:
https://github.com/codepath/android_guides/wiki/Local-Databases-with-SQLiteOpenHelper
### Хранение простых данных
Все довольно просто, начать можно тут:
http://developer.android.com/intl/ru/training/basics/data-storage/index.html

Для SharedPreferences можно делать класс-обертку для удобного доступа к данным.

### Файлы
В общих чертах, чтобы открыть файл, нужно найти его расположение и открыть InputStream (лучше оборачивать в BufferedInputStream) или FileReader.
Информация тут:
http://developer.android.com/intl/ru/training/basics/data-storage/files.html

Операции с файлами нужно делать не в главном потоке, соотвественно нужно написать немного вспомогательных классов для работы с ними.

## Результаты
* Уметь хранить настройки в SharedPreferences. 
* Уметь составлять простые запросы на CRUD (Create, Read, Update, Delete) операции на языке SQL.
* Делать CRUD-операции с помощью SQLiteOpenHelper.
* Читать и записывать в файл.

## Задание 
Пишем экран логина и регистрации. Инофрмация пусть хранится в базе данных. Если пользователь прошел логин - отправляем на приветственное активити. Если нет - регистрируем. 

###Hacker edition
При регистрации нужно выбрать один из островов архипелага "Острова Кука". Список хранится в текстовом файле в assets. При первом старте нужно добавить этот список в таблицу БД, а потом при регистрации показать пользователю для выбора. В таблице пользователей нужно хранить айди острова. 
В SharedPreferences запоминать, логинился ли пользователь, если да - автоматически логинить, если нет - предлагать логин или регистрацию.
При логауте стирать SharedPreferences. 
