# Advanced - Многопоточность.

1. Еще раз [понятие многопоточности](https://habrahabr.ru/post/164487/)
2. [HandlerThread - dev.android.com](https://developer.android.com/reference/android/os/HandlerThread.html)). 
3. [HandlerThread - Codepath](https://github.com/codepath/android_guides/wiki/Managing-Threads-and-Custom-Services#using-a-handlerthread).
4. [ThreadPoolExecutor - dev.android.com](https://developer.android.com/reference/java/util/concurrent/ThreadPoolExecutor.html), 
5. [ThreadPoolExecutor - Codepath](https://github.com/codepath/android_guides/wiki/Managing-Threads-and-Custom-Services#using-a-threadpoolexecutor).

### Задание
Написать даунлоадер картинок котиков с интернета. Должен использовать пулл потоков для скачивания.
Например, список состоит из 100 элементов. Создается 5 потоков, которые скачивают эти элементы.
Используйте [HttpUrlConnection](http://developer.android.com/reference/java/net/HttpURLConnection.html) для скачивания. 
Базовая реализация -- локальный список url картинок в файле.
Должна быть реализация расчета приблизиилельного времени скачивания всех картинок.
После скачивания (или во время) показать все картинки списком (или другим способом).

**Hacker edition 1**: Даунлоадер самобалансирующийся. Если картинка качается долго, создавать больше потоков, если быстро - уменьшать. Для симуляции делайте паузу по времени внутри скачивателя картинки (Thread.sleep()).

**Hacker edition 2**: Использовать API сервиса с картинками (Flikr, Google Images), получить котеек оттуда. Можно использовать сторонние реализации SDK.
