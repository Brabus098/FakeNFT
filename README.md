# FakeNFT - Каталог NFT-коллекций

![Swift](https://img.shields.io/badge/Swift-5.9-FA7343?logo=swift)
![iOS](https://img.shields.io/badge/iOS-17.0+-lightgrey?logo=apple)
![SwiftUI](https://img.shields.io/badge/UI-SwiftUI-1E8CBE?logo=swift&color=FA7343)
![MVVM](https://img.shields.io/badge/Architecture-MVVM-FA7343?style=for-the-badge)
![Swift Concurrency](https://img.shields.io/badge/Concurrency-async/await-FA7343?logo=swift)

**FakeNFT** - современное iOS-приложение для просмотра и имитации покупки NFT-токенов. Каталог коллекций, избранное, корзина, рейтинг пользователей и персонализированный профиль в едином стиле.

<p align="center">
  <img src="https://github.com/Brabus098/FakeNFT/raw/main/NftLent.png" width="200" alt="Лента NFT">
  <img src="https://github.com/Brabus098/FakeNFT/raw/main/NftCollection.png" width="200" alt="Коллекция NFT">
  <img src="https://github.com/Brabus098/FakeNFT/raw/main/MyNFT.png" width="200" alt="Мои NFT">
</p>

<p align="center">
    <img src="https://github.com/Brabus098/FakeNFT/raw/main/Cart.png" width="200" alt="Корзина">
  <img src="https://github.com/Brabus098/FakeNFT/raw/main/PaymentMethod.png" width="200" alt="Способы оплаты">
  <img src="https://github.com/Brabus098/FakeNFT/raw/main/Profile.png" width="200" alt="Профиль">
</p>

## 🚀 Возможности

### 🖼️ Каталог и коллекции
- **Просмотр NFT-коллекций** с обложками, названиями и количеством
- **Детальная информация** о коллекции с описанием и ссылкой на автора
- **Сетка NFT** с рейтингом, ценой и интерактивными кнопками
- **Сортировка** по различным критериям с сохранением настроек

### ❤️ Избранное и корзина
- **Добавление в избранное** с визуальной обратной связью
- **Управление корзиной** - добавление, удаление, подтверждение
- **Имитация оплаты** с выбором валюты и пользовательским соглашением
- **Подтверждение удаления** с деталями NFT

### 👤 Профиль и статистика
- **Персональный профиль** с фото, именем, описанием и сайтом
- **Мои NFT** - список приобретенных токенов
- **Избранные NFT** - коллекция понравившихся токенов

### 🎨 Пользовательский опыт
- **Полная поддержка темной темы**
- **Локализация интерфейса**
- **Обработка сетевых ошибок** с алертами
- **Интеграция с Яндекс Метрикой** (опционально)

## 🛠 Технологический стек

**Язык программирования:**  
![Swift](https://img.shields.io/badge/Swift-FA7343?style=for-the-badge&logo=swift&logoColor=white)

**UI Фреймворк:**  
![SwiftUI](https://img.shields.io/badge/SwiftUI-FA7343?style=for-the-badge&logo=swift&logoColor=white)

**Архитектура:**  
![MVVM](https://img.shields.io/badge/MVVM-FA7343?style=for-the-badge)
![ObservableObject](https://img.shields.io/badge/ObservableObject-FA7343?style=for-the-badge)
![@Published](https://img.shields.io/badge/@Published-FA7343?style=for-the-badge)

**Сеть и данные:**  
![URLSession](https://img.shields.io/badge/URLSession-FA7343?style=for-the-badge&logo=apple&logoColor=white)
![REST API](https://img.shields.io/badge/REST_API-FA7343?style=for-the-badge)
![JSON](https://img.shields.io/badge/JSON-FA7343?style=for-the-badge)
![Codable](https://img.shields.io/badge/Codable-FA7343?style=for-the-badge)
![Sendable](https://img.shields.io/badge/Sendable-FA7343?style=for-the-badge)

**Хранение данных:**  
![UserDefaults](https://img.shields.io/badge/UserDefaults-FA7343?style=for-the-badge)
![@AppStorage](https://img.shields.io/badge/@AppStorage-FA7343?style=for-the-badge)

**Многопоточность:**  
![async/await](https://img.shields.io/badge/async/await-FA7343?style=for-the-badge)
![async let](https://img.shields.io/badge/async_let-FA7343?style=for-the-badge)
![TaskGroup](https://img.shields.io/badge/TaskGroup-FA7343?style=for-the-badge)
![@MainActor](https://img.shields.io/badge/@MainActor-FA7343?style=for-the-badge)

**Инструменты:**  
![Xcode](https://img.shields.io/badge/Xcode-FA7343?style=for-the-badge&logo=xcode&logoColor=white)
![Git](https://img.shields.io/badge/Git-FA7343?style=for-the-badge&logo=git&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-FA7343?style=for-the-badge&logo=figma&logoColor=white)
![Swift Package Manager](https://img.shields.io/badge/SPM-FA7343?style=for-the-badge&logo=swift&logoColor=white)

**WebView:**  
![WKWebView](https://img.shields.io/badge/WKWebView-FA7343?style=for-the-badge)

## ⚙️ Установка и запуск

### Требования
- macOS 14.0+
- Xcode 15.0+
- iOS 17.0+

### Быстрый старт

```bash
git clone https://github.com/Brabus098/FakeNFT.git
cd FakeNFT
open FakeNFT.xcodeproj
```
1. Выберите симулятор или подключите устройство
2. Нажмите `Cmd + R` для сборки и запуска
3. Исследуйте каталог NFT и тестируйте функционал!

---

## 🏗 Архитектура

Проект реализован с использованием **MVVM + Swift Concurrency**:
- **View Models** используют `@Observable` или `ObservableObject` с `@Published`
- **Сервисы** реализованы через `actor` для потокобезопасности
- **Данные** помечены `Sendable` для безопасной передачи между потоками
- **Обновление UI** строго через `@MainActor`

---

## 🎯 Особенности реализации

### 🌐 Сетевое взаимодействие
- **Actor-based сервисы** для безопасного доступа к данным
- **Sendable модели** для потокобезопасности
- **async/await запросы** к mock-серверу
- **Обработка ошибок** с пользовательскими алертами

### ⚡ Современная многопоточность
- **Только Swift Concurrency** (без GCD)
- **async let** для параллельных запросов
- **TaskGroup** для групповых операций
- **@MainActor** для гарантированного обновления UI

### 📱 Пользовательский интерфейс
- **Чистый SwiftUI** + UIKit контроллер для показа  увеличенной NFT 
- **LazyVGrid** для коллекций NFT
- **WKWebView через UIViewRepresentable** для ссылок
- **Кастомные алерты** для подтверждения действий

---

## 📈 Статус разработки

### ✅ Завершено
- Каталог коллекций с сортировкой
- Детальный просмотр коллекции NFT
- Система избранного и корзины
- Профиль пользователя с редактированием
- Рейтинг пользователей и профили
- Интеграция с mock-сервером
- Сохранение настроек сортировки
- Локализация** (русский/английский)
- Темная тема** с поддержкой системы
- Кастомный launch screen

### 🔄 В активной разработке
- **Экран онбординга** для новых пользователей
- **Интеграция с Яндекс Метрикой**

### 🗓 В планах
- Поиск по коллекциям
- Экран авторизации
- Алерт с предложением оценить приложение

---

## 👨‍💻 Автор

**Vladimir** - iOS Developer

<p align="center">
  <a href="https://t.me/Vov4eg777">
    <img src="https://img.shields.io/badge/Telegram-FA7343?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram"/>
  </a>
  <a href="mailto:olsh0988@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-FA7343?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/>
  </a>
  <a href="https://docs.google.com/document/d/18caT1lR7wfQcId3kl3MaWkGpnjQqEGYBz7goR_59zEw/edit?usp=sharing">
    <img src="https://img.shields.io/badge/Resume-FA7343?style=for-the-badge&logo=google-drive&logoColor=white" alt="Resume"/>
  </a>
</p>

---
