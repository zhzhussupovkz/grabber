## Grabber
=======

Web-паук который  вытаскивает из страниц все существующие изображения.

### Как запускать?

    linux$ ./grab.rb  google.com tmp

- grab.rb - название программы, который принимает два аргумента
- Первый аргумент url страницы, откуда нужно скачать все изображения, здесь это google.com
- Второй аргумент название директории куда нужно скачать файлы, здесь tmp.


### Как работает?

Программа скачивает исходный код страницы google.com с помощью библиотеки open-uri.  
Находит из этой страницы все теги img и запоминет атрибуты src используя регулярные выражения и MatchData.
Затем скачивает их в директорию указанную в качестве второго аргумента программы.
