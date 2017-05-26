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
    
    
[LensKit]: http://lenskit.org
[gradle]: http://gradle.org
[mailing list]: https://wwws.cs.umn.edu/mm-cs/listinfo/lenskit
[LensKitRS]: http://twitter.com/LensKitRS
