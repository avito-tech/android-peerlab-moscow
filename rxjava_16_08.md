Мы обсуждали различные аспекты RxJava, о которых не говорят вслух.
В основном про ее переусложненность и бездонность для изучения.

Как пример - приключения с RxJava описанные здесь
https://habrahabr.ru/post/281312/

Неплохо понимать, что за человек пишет RxJava:
https://plus.google.com/113316559156085910174
https://github.com/akarnokd

Его блог Advanced Reactive Java
http://akarnokd.blogspot.ru/

Большая часть материала из его блога перекочевала в документацию RxJava
https://github.com/ReactiveX/RxJava/wiki

Но самая лучшая документация по RxJava - это ее юнит тесты, которые не только покажут
примеры использования, но и расскажут про скрытые FIXME и cornercases, например race conditions.

https://github.com/ReactiveX/RxJava/blob/2.x/src/test/java/io/reactivex/subjects/BehaviorSubjectTest.java

В блоге David Karnok можно прочитать про конкуретность в RxJava, а так же
как сложно стало писать кастомные конкурретные операторы в RxJava2

http://akarnokd.blogspot.ru/2015/05/operator-concurrency-primitives_11.html

Есть гораздо более щадящяя выжимка в статье от Артема Зинатуллина:
https://artemzin.com/blog/rxjava-thread-safety-of-operators-and-subjects/

Также мы поговорили о существовании RxJavaHooks и обработке ошибок
https://github.com/ReactiveX/RxJava/wiki/Plugins#rxjavaerrorhandler
https://github.com/ReactiveX/RxJava/wiki/Error-Handling

А еще вспомнили замечательный разговор c akarnokd на гитабе:

> implement your own reactive library as you see fit.

https://github.com/ReactiveX/RxJava/issues/5211

В целом сошлись на том, что нужно больше best practices.
На rx можно решить любую задачу, но не стоит использовать ее дальше собственного понимания,
как она работает, и не переусложнять.

С другой стороны, rx всегда обеспечит веселое времяпрепровождение!
