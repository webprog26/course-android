﻿# Занятие 4. Intent.

1. Понятие намерений
2. Виды и категории намерений
3. Передача аргументов намерением
4. Что с помощью них можно делать
5. BroadcastReceiver
6. IntentFilters

### Что нужно знать
* Говоря просто - объект Intent дает нам возможность указать, какое действие мы желаем совершить. Открыть активность, отослать SMS или сделать фото с камеры - создаем Intent, и либо явно указываем желаемое действие, либо можем оставить выбор способа исполнения на усмотрение системы. За счет возможности вызвать из разрабатываемого приложения, к примеру, activity галереи, выбрать фото, и вернуть его в приложение -  достигается некоторая "бесшовность" Android OS, очень удобная для разработчиков.
* Возможности Intent велики, и необходимо четко понимать их механизм и способы использования. 
* http://developer.android.com/intl/ru/reference/android/content/Intent.html - читаем документацию на официальном сайте. Там много полезных штук, а главное - все методы и константы, ознакомиться с ними очень желательно.
* http://habrahabr.ru/post/131041/ - читаем хабр. Там четко и понятно показаны примеры того, как вы можете использовать Intent. 
* http://developer.alexanderklimov.ru/android/theory/intent.php - эта статья во многом повторяет официальную документацию, но некоторые моменты автор поясняет более просто.
* Также необходимо ознакомиться с понятиями IntentFilter и BroadcastReceiver. IntentFilter позволяет нам задать действие, которое может выполнять Activity, а BroadcastReceiver позволяет отслеживать необходимые Intent, таким образом осуществляется коммуникация. 

### Результаты
* Тема довольно объемная, но без нее нельзя. Понятие намерений одно из базовых в Андроиде, и без четкого понимания что это, как и зачем, а также как пользоваться, далеко не запрограммируешь. 
* Цель - поучить четкое понимание интентов, ресивера и фильтров.

### Задание 
Пишем будильник. Начальные знания о вьюшках имеем, сервисы-интенты знаем, можно написать будильник. Хм, если напишем криво - будем просыпать на работу ;) Воспитываем ответственность. 
