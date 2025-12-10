# Zero Messenger

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![React Native](https://img.shields.io/badge/React_Native-0.74-green.svg)](https://reactnative.dev/)

Open-source P2P-мессенджер, работающий без интернета (через Wi-Fi Direct/Bluetooth). Вдохновлён Telegram, но децентрализован для оффлайн-сценариев (глушилки, протесты, походы). End-to-end шифрование, кастомизация UI, группы в разработке.

## 🚀 Особенности
- **Оффлайн P2P**: Обнаруживает устройства рядом (~50-100м), чат без сервера.
- **E2EE**: Сообщения шифруются на устройстве (libsodium).
- **UI как в Telegram**: Пузыри, автоскролл, статус "онлайн через P2P".
- **Кастомизация**: Темы, стикеры (Redux).
- **Кросс-платформа**: Android/iOS (React Native).
- **Open-source**: Apache 2.0, вклады приветствуются!

## 🛠 Технологии
- **Frontend**: React Native 0.74 + React Navigation + Redux.
- **P2P**: react-native-wifi-p2p + react-native-tcp-socket (fallback на Bluetooth).
- **Шифрование**: react-native-sodium.
- **Backend (hybrid)**: Python + Flask (для онлайн-синхронизации, опционально).

## 📱 Установка и запуск
### Требования
- Node.js 18+
- Android Studio (для Android) или Xcode (для iOS).
- Включи Wi-Fi и GPS на устройствах для P2P.

### Клонируй и запусти
```bash
git clone https://github.com/Fromix1234/zero-messanger.git
cd zero-messanger/frontend
npm install
npx react-native run-android  # или run-ios
