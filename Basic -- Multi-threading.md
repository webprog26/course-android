# Многопоточность
Очень часто возникает потребность выполнить какую-то ресурсоемкую задачу. 
Но если выполнять ее, не создавая отдельный поток, она полностью заблокирует пользовательский интерфейс и пользователь может решить, что программа зависла и не функционирует.
Вообще, любую операцию длинее 100 миллисекунд (в среднем) лучше переносить в отдельный поток. Хотя конечно, всегда нужно руководствоваться прежде всего здравым смыслом.
Также нужно учитывать, что то, что работает быстро на новом устройстве, существенно "повесит" интерфейс на старом. 

В Android SDK многопоточность реализуется с помощью классов из Java SDK
(например [Thread](https://developer.android.com/reference/java/lang/Thread.html), 

Кроме этого, есть вспомогательные классы уже в самом Android SDK ([AsyncTask](https://developer.android.com/reference/android/os/AsyncTask.html), 
[IntentService](https://developer.android.com/reference/android/app/IntentService.html)).

## Ссылки
[Базовый гайд по многопоточности](https://developer.android.com/training/multiple-threads/index.html).

А также [Keeping Your App Responsive](https://developer.android.com/training/articles/perf-anr.html).

[Гайд на codepath](https://github.com/codepath/android_guides/wiki/Managing-Threads-and-Custom-Services).

Еще очень рекомендую канал [Android Developers](https://www.youtube.com/channel/UCVHFbqXqoYvEWM1Ddxl0QDg) на Youtube, а именно [Performance](https://www.youtube.com/playlist?list=PLWz5rJ2EKKc9CBxr3BVjPTPoDPLdPIFCE).
Конкретные видео:
https://www.youtube.com/watch?v=qk5F6Bxqhr4&list=PLWz5rJ2EKKc9CBxr3BVjPTPoDPLdPIFCE&index=1
https://www.youtube.com/watch?v=0Z5MZ0jL2BM&list=PLWz5rJ2EKKc9CBxr3BVjPTPoDPLdPIFCE&index=2

## Результаты
* Понимать, как жизненный цикл приложения Android OS связан с жизненным циклом потоков (ЭТО ВАЖНО).
* Как использовать общие переменные и данные в разных потоках (*synchronized*, *volatile*, приметка "этот класс не синхронизирован" в описании классов типа HashMap в документации).
* Догадываться, когда нужно использовать тот или иной инструмент. (https://www.youtube.com/watch?v=0Z5MZ0jL2BM).

# Задания
1. Сделать поиск по каталогу с видео и фотками. Показать самые старые фотографии и видео. В этом уроке используйте один дополнительный поток. 
2. Из трех фоток из интернета нужно выбрать фотографию с самым большим разрешением и показать ее. Скачивать можно самым простым способом из доступных.
