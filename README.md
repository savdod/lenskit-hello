# LensKit Demo Project

Построение рекомендательной системы с использованием коллаборативной фильтрации item 2 item.

Настройка конфигурации рекомендательного движка: etc/item-item.groovy

Java код здесь: org.grouplens.lenskit.hello.HelloLenskit. Есть комментарии, по которым можно понять что происходит на каждой стадии процесса.

Запускать можно через IDE, с указанием id пользователя в аргументах, или выполняя в командной строке:

	$ ./gradlew build
	$ /bin/sh build/install/lenskit-hello/bin/lenskit-hello <userid>

На Windows:

	C:\LensKit\lenskit-hello> .\gradlew.bat build
	C:\LensKit\lenskit-hello> .\build\install\lenskit-hello\bin\lenskit-hello.bat <userid>
    
## Проведение оценки

-   `build.gradle`: конфигурация оценки алгоритмов
-   `analyze-output.ipynb`: результаты оценок и построение графиков.
  
Запустить оценки:

    ./gradlew evaluate

Все файлы после оценки лежат в директории /build.
Для оценки новой конфигурации нужно будет предварительно применить ./gradlew clean

## Просмотр результатов

Запускать просмотр можно с использованием [Jupyter](http://jupyter.org/) notebook

Просмотр требует следующих пакетов:

- Jupyter (formerly IPython)
- Pandas
- matplotlib

Получить все эти пакеты можно установив [Anaconda Python](https://www.continuum.io/downloads).  Внутри нее есть все научные инструменты для Python на Windows, OS X и Linux.
