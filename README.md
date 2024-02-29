# android_marathon_Activity

### Первый запуск

![1](https://github.com/kekuchh/android_marathon_Activity/assets/98802601/7a2c28ef-8061-4e94-b1cb-ebdc65962603)


```
2024-02-28 23:10:04.314  7524-7524  MainActivity LOG        com.example.businesscard             D  onCreate
2024-02-28 23:10:04.347  7524-7524  MainActivity LOG        com.example.businesscard             D  onStart
2024-02-28 23:10:04.348  7524-7524  MainActivity LOG        com.example.businesscard             D  onResume
```

Вызываются 3 метода на создание Activity в последовательности: 
  - onCreate() - создание Activity из Layot
  - onStart() - показ макета пользоветелю
  - onResume() - взаимодействие с пользователем

### Поворот экрана

![2](https://github.com/kekuchh/android_marathon_Activity/assets/98802601/ef4613e2-c9cc-4395-b452-2f98b4b304e4)


```
2024-02-28 23:15:23.748  7524-7524  MainActivity LOG        com.example.businesscard             D  onPause
2024-02-28 23:15:23.753  7524-7524  MainActivity LOG        com.example.businesscard             D  onStop
2024-02-28 23:15:23.765  7524-7524  MainActivity LOG        com.example.businesscard             D  onDestroy
2024-02-28 23:15:23.821  7524-7524  MainActivity LOG        com.example.businesscard             D  onCreate
2024-02-28 23:15:23.826  7524-7524  MainActivity LOG        com.example.businesscard             D  onStart
2024-02-28 23:15:23.827  7524-7524  MainActivity LOG        com.example.businesscard             D  onResume
```

При повороте экрана всё заново отрисовывается - вначале вызываются методы для уничтожения текущего Activity, затем вызываются 3 метода для создания Activity, как при первом запуске приложения.

### Сворачивание приложения

![3](https://github.com/kekuchh/android_marathon_Activity/assets/98802601/67badc62-7224-4131-9eaa-0c5b37e4022b)


```
2024-02-28 23:16:37.185  7524-7524  MainActivity LOG        com.example.businesscard             D  onPause
2024-02-28 23:16:38.077  7524-7524  MainActivity LOG        com.example.businesscard             D  onStop
```

При сворачивании приложения вначале вызывается onPause(), т.к. пользователь не может взаимодействовать с приложением, затем onStop() - пользователь не видит приложение

### При вызове finish() в onCreate()

![4](https://github.com/kekuchh/android_marathon_Activity/assets/98802601/c1ebbdaa-0131-40af-bcb0-5c312c8329fc)


```
2024-02-28 23:20:41.857  8273-8273  MainActivity LOG        com.example.businesscard             D  onCreate
2024-02-28 23:20:42.041  8273-8273  MainActivity LOG        com.example.businesscard             D  onDestroy
```

Сразу после создания приложения вызвается метод finish() => уничтожение приложение методом onDestroy()
