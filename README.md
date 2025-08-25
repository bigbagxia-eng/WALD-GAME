# Dungeon Quest — FINAL (KayKit, Replit-ready)

Полноценный каркас 2D top‑down подземелья **с 12 уровнями** и **полным пакетом KayKit**, уже вложенным в `assets`.
Код — чистый HTML+JS (Canvas), без зависимостей.

## Возможности
- Процедурные уровни (12 этажей), растущая сложность, разные размеры.
- Игрок: ходьба, перекат со стаминой, ближняя атака.
- Враги: слаймы, скелеты, маги (патруль/преследование/дистанционные атаки).
- Предметы: монеты, зелья, ключи из сундуков.
- Ловушки, дверь/выход, победа/поражение.
- HUD, меню, пауза, сохранение (localStorage).
- Мобильные кнопки (виртуальный стик, атака/перекат).
- Используются ассеты **KayKit Dungeon Remastered** (вся папка включена).

## Старт в Replit
1. Импортируйте репозиторий (тип Repl: **HTML, CSS, JS**).
2. Нажмите **Run** — игра запустится.

## Сборка под iOS/Android (Capacitor)
- Установите Node.js, затем:
```bash
npm create vite@latest dq-final -- --template vanilla
cd dq-final
# Замените содержимое папки проекта файлами из этого репозитория (index.html, /src, /assets).
npm install @capacitor/core @capacitor/cli @capacitor/ios @capacitor/android
npx cap init "Dungeon Quest" "com.example.dungeonquest"
npx cap add ios
npx cap add android
npx cap copy
npx cap open ios   # откроется Xcode для сборки на iOS
npx cap open android # откроется Android Studio
```
- В Xcode/Android Studio включите необходимые разрешения, и соберите релиз.

## Лицензии
- Код: MIT (LICENSE).
- Ассеты KayKit: их лицензия (см. содержимое `assets/kaykit/`).
