# Занятие 11. Многопоточность.

1. [Понятие многопоточности](https://habrahabr.ru/post/164487/)
2. [В Android](https://github.com/codepath/android_guides/wiki/Managing-Threads-and-Custom-Services#understanding-the-main-thread).
3. [AsyncTask](https://github.com/codepath/android_guides/wiki/Managing-Threads-and-Custom-Services#using-an-asynctask), еще в [видео](https://www.youtube.com/watch?v=jtlRNNhane0).
4. [HandlerThread](https://github.com/codepath/android_guides/wiki/Managing-Threads-and-Custom-Services#using-a-handlerthread).
5. [ThreadPoolExecutor](https://github.com/codepath/android_guides/wiki/Managing-Threads-and-Custom-Services#using-a-threadpoolexecutor).

### Результаты
* Понимать, как жизненный цикл приложения Android OS связан с жизненным циклом потоков (ЭТО ВАЖНО).
* Как использовать общие переменные и данные в разных потоках (*synchronized*, *volatile*, приметка "этот класс не синхронизирован" в описании классов типа HashMap в документации).
* Догадываться, когда нужно использовать тот или иной инструмент. (https://www.youtube.com/watch?v=0Z5MZ0jL2BM).

### Задание
Написать даунлоадер картинок котиков с интернета. Должен использовать пулл потоков для скачивания.
Например, список состоит из 100 элементов. Создается 5 потоков, которые скачивают эти элементы.
Используйте [HttpUrlConnection](http://developer.android.com/reference/java/net/HttpURLConnection.html) для скачивания. 
Базовая реализация -- локальный список url картинок в файле.
Должна быть реализация расчета приблизиилельного времени скачивания всех картинок.
После скачивания (или во время) показать все картинки списком (или другим способом).

*Hacker edition 1*: Даунлоадер самобалансирующийся. Если картинка качается долго, создавать больше потоков, если быстро - уменьшать. Для симуляции делайте паузу по времени внутри скачивателя картинки (Thread.sleep()).
*Hacker edition 2*: Использовать API сервиса с картинками (Flikr, Google Images), получить котеек оттуда. Можно использовать сторонние реализации SDK.
