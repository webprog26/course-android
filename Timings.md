#Ожидаемые тайминги по занятиям

## Basic
###1 неделя -- Основы основ
1. [Введение](/shpp-android/course-android/blob/master/Android%20Intro%20-%20Lesson%201%20-%20Introducing%20Android%20OS.md).
2. [Настройка окружения](/shpp-android/course-android/blob/master/Android%20Intro%20-%20Lesson%202%20-%20Setting%20up.md).
3. [Основные компоненты OS](/shpp-android/course-android/blob/master/Android%20Intro%20-%20Lesson%203%20-%20Android%20app%20components.md).

###2 неделя -- Компоненты ОС
1. [Основные компоненты OS](/shpp-android/course-android/blob/master/Android%20Intro%20-%20Lesson%203%20-%20Android%20app%20components.md)*(продолжение)*.
2. [Gradle basics](/shpp-android/course-android/blob/master/Android%20Intro%20-%20Gradle%20basics.md).
3. [Activity](/shpp-android/course-android/blob/master/Android%20Intro%20-%20Lesson%205%20-%20Welcome%20to%20Activity.md)

###3 неделя -- Компоненты ОС
1. [Intents](/shpp-android/course-android/blob/master/Android%20Intro%20-%20Lesson%204%20-%20Intent.md)
2. [Services](/shpp-android/course-android/blob/master/Android%20Intro%20-%20Lesson%206%20-%20%20Welcome%20to%20Sevices.md), IntentServices, foreground service.
3. [Ресурсы и Темы](/shpp-android/course-android/blob/master/Android%20Intro%20-%20Resources.md)

###4 неделя -- Multi-threading
1. [Multi-threading](/shpp-android/course-android/blob/master/Basic%20--%20Multi-threading.md).
2. [Пулл/очередь потоков, AsyncTask](/shpp-android/course-android/blob/master/Advanced%20-%20Multi-threading.md).

###5 неделя -- Адаптеры
1. Простой адаптер.
2. Паттерн ViewHolder.
3. Кнопки внутри адаптера.

###6 неделя -- коммуникация между процессами
1. Broadcast Receiver, LocalBroadcastReceiver
2. Коммуникация с Service. Обзорно AIDL (http://developer.android.com/guide/components/aidl.html)
3. Паттерн EventBus, third-party libs.
4. http://developer.android.com/guide/components/processes-and-threads.html

----
*дальше приблизительно, нуждается в дополнении*

###7, 8 неделя -- UI
1. [View, Menu](https://github.com/shpp-android/course-android/blob/master/Android%20Intro%20-%20Lesson%207%20-%20View%2C%20menu.md) ([Разделить, Issue #3](https://github.com/shpp-android/course-android/issues/3))

###9 неделя -- Network

###10 неделя -- [БД](https://github.com/shpp-android/course-android/blob/master/Android%20Intro%20-%20Lesson%208%20-%20Data%20is%20gold.md)
1. SQL, SQLite
2. ContentProviders
3. Обзор ORM
[Issue #4](https://github.com/shpp-android/course-android/issues/4)
4. CusorAdapter.

###11 неделя -- Fragments
1. Сами фрагменты [Fragments](https://github.com/shpp-android/course-android/blob/master/Android%20Intro%20-%20Lesson%209%20-%20Fragments.md).
2. Фрагменты + ресурсы = классическая задача про разный UI при разной ориентации экрана.
3. Подводные камни (типа commit() vs commitAllowingStateLoss()).

## Advanced
###12, 13 неделя -- Архитектура типичного приложения
1. MVC (как общий случай), MVP (как более схожий с архитектурой SDK Android OS), отличия.
(http://antonioleiva.com/mvp-android/)
(http://fernandocejas.com/2014/09/03/architecting-android-the-clean-way/)
2. Network stack.
3. Модели, сериализаторы (продолжение).
4. Объекты в БД.
5. Состояния контролов и экранов:
    * Экран -- успешно/ошибка/ввод данных
    * Контрол -- нажато/обычный/выбрано.
6. Loaders.

###14 неделя -- Material Design Concept
1. Читать, проникнуться.
2. Специальные контролы.
3. RecycleView.

###15 неделя -- Gradle Advanced
1. Flavors.
2. Plugins.
3. Пишем какую-то простую цель (target).
