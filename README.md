# android_marathon_Activity

### Первый запуск

<img width="1792" alt="Screenshot 2024-02-28 at 23 12 39" src="https://github.com/kekuchh/android_marathon_Activity/assets/98802601/0021eb39-5fcb-4420-a1f3-fb1e72ad6aab">

```
2024-02-28 23:10:04.314  7524-7524  MainActivity LOG        com.example.businesscard             D  onCreate
2024-02-28 23:10:04.347  7524-7524  MainActivity LOG        com.example.businesscard             D  onStart
2024-02-28 23:10:04.348  7524-7524  MainActivity LOG        com.example.businesscard             D  onResume
```

### Поворот экрана

<img width="1792" alt="Screenshot 2024-02-28 at 23 15 55" src="https://github.com/kekuchh/android_marathon_Activity/assets/98802601/03cf4b6c-03c2-43c0-8e91-59805d54bb33">

```
2024-02-28 23:15:23.748  7524-7524  MainActivity LOG        com.example.businesscard             D  onPause
2024-02-28 23:15:23.753  7524-7524  MainActivity LOG        com.example.businesscard             D  onStop
2024-02-28 23:15:23.765  7524-7524  MainActivity LOG        com.example.businesscard             D  onDestroy
2024-02-28 23:15:23.821  7524-7524  MainActivity LOG        com.example.businesscard             D  onCreate
2024-02-28 23:15:23.826  7524-7524  MainActivity LOG        com.example.businesscard             D  onStart
2024-02-28 23:15:23.827  7524-7524  MainActivity LOG        com.example.businesscard             D  onResume
```

### Сворачивание приложения

<img width="1792" alt="Screenshot 2024-02-28 at 23 16 58" src="https://github.com/kekuchh/android_marathon_Activity/assets/98802601/e4e0ea8e-5b45-47e5-bd44-083b2104d537">

```
2024-02-28 23:16:37.185  7524-7524  MainActivity LOG        com.example.businesscard             D  onPause
2024-02-28 23:16:38.077  7524-7524  MainActivity LOG        com.example.businesscard             D  onStop
```

### При вызове finish() в onCreate()

<img width="1792" alt="Screenshot 2024-02-28 at 23 20 48" src="https://github.com/kekuchh/android_marathon_Activity/assets/98802601/d3d2c314-2cbb-4d94-8745-2daa19139596">

```
2024-02-28 23:20:41.857  8273-8273  MainActivity LOG        com.example.businesscard             D  onCreate
2024-02-28 23:20:42.041  8273-8273  MainActivity LOG        com.example.businesscard             D  onDestroy
```
