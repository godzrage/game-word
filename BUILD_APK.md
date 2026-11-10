# Сборка APK «Цепочка слов»

Игра упакована через Capacitor (папка `android/`).

## Вариант 1 — на своём компьютере
Нужны: Node 20+, Android Studio (или JDK 21 + Android SDK).
```
npm install
npm run build
npx cap sync android
cd android && ./gradlew assembleDebug      # Windows: gradlew.bat assembleDebug
```
Готовый файл: `android/app/build/outputs/apk/debug/app-debug.apk`.
Либо `npx cap open android` и Build → Build APK(s) в Android Studio.

## Вариант 2 — через GitHub
Залейте проект в GitHub: Actions → «Build APK» соберёт APK автоматически (artifact `word-chain-apk`).

## Вариант 3 — без сборки
Откройте сайт в Chrome на телефоне → меню → «Установить приложение».
