Основы Gradle
==========================

Gradle это новая мощная система управления зависимостей для Java. Если вкратце -- до Gradle было очень плохо, сейчас стало просто отлично. 
Gradle комбинирует в себе декларативный и процедурный подходы. То есть, мы составляем нужную конфигурацию, но при необходимости всегла можем добавить свом собственные обработчики файлов, классов или ресурсов.

## Материалы
Вводная статья [тут (Codepath)](https://github.com/codepath/android_guides/wiki/Getting-Started-with-Gradle).

[Официальная документация](https://developer.android.com/studio/build/index.html), как маст-рид (главный раздел [и](https://developer.android.com/studio/build/build-variants.html) [все](https://developer.android.com/studio/build/configure-apk-splits.html) [подразделы](https://developer.android.com/studio/build/manifest-merge.html)).

Кроме того, ознакомьтесь с [проблемой лимита в 65 тысяч](https://developer.android.com/studio/build/multidex.html) методов и [работой Proguard](https://developer.android.com/studio/build/shrink-code.html). 

## Результаты
1. Понимать, зачем нужны flavors.
2. Multidex -- что это.
3. Уметь настроить подпись приложения ключом для релиз-конфигурации.

## Задание
1. У нас есть два абсолютно одинаковых приложения (с точки зрения кодовой базы). Различия:
  * название;
  * набор иконок;
  * использование встроенных покупок в одном их них (*Advanced*).
Сделать настройку для данной конфигурации. Встроенные покупки изобразить схематично с помощью пустого класса или просто константы. Про ресурсы читайте в [этом уроке](https://github.com/shpp-android/course-android/blob/master/Android%20Intro%20-%20Resources.md).
2. (*Hacker edition*) [Как известно](https://www.google.sk/url?sa=t&rct=j&q=&esrc=s&source=video&cd=1&cad=rja&uact=8&ved=0ahUKEwjU5pmg6c3PAhXKC8AKHTVSA9cQtwIIGjAA&url=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DHzs6OBcvNQE&usg=AFQjCNHUJ80GT0KjKARyAcawCJiplWO-Zw&sig2=cNBkYXCl71EQWlE94t-kyw&bvm=bv.135258522,d.ZGg), использование enum в Андроид коде не рекомендуется. С помощью Gradle при запуске сборки искать в исходниках все enum и выдавать предупреждение. 
