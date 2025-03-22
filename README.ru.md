# 🚀 Next.js + tRPC + TON Monorepo

<div align="center">

[![GitHub звёзды](https://img.shields.io/github/stars/DKeken/turborepo-ton-trpc?style=for-the-badge)](https://github.com/DKeken/turborepo-ton-trpc/stargazers)
[![GitHub форки](https://img.shields.io/github/forks/DKeken/turborepo-ton-trpc?style=for-the-badge)](https://github.com/DKeken/turborepo-ton-trpc/network/members)
[![GitHub наблюдатели](https://img.shields.io/github/watchers/DKeken/turborepo-ton-trpc?style=for-the-badge)](https://github.com/DKeken/turborepo-ton-trpc/watchers)
[![Лицензия: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)](https://nextjs.org/)
[![TON](https://img.shields.io/badge/TON-0088CC?style=for-the-badge&logo=telegram&logoColor=white)](https://ton.org/)

</div>

<p align="center">
  <strong>Современный, типобезопасный и масштабируемый шаблон монорепозитория для создания приложений на блокчейне TON</strong>
</p>

<p align="center">
  <a href="#-фичи">Фичи</a> •
  <a href="#-технологический-стек">Технологический стек</a> •
  <a href="#-структура-проекта">Структура проекта</a> •
  <a href="#-начало-работы">Начало работы</a> •
  <a href="#-переменные-окружения">Переменные окружения</a> •
  <a href="#-разработка">Разработка</a> •
  <a href="#-деплоймент">Деплоймент</a> •
  <a href="#-вклад-в-проект">Вклад в проект</a> •
  <a href="#-лицензия">Лицензия</a>
</p>

<p align="center">
  <a href="README.ru.md">🇷🇺 Русская версия</a>
</p>

---

## ✨ Фичи

- **🔒 Типобезопасность и производительность**

  - Полноценный стек TypeScript с строгой проверкой типов
  - Сквозная типобезопасность с tRPC
  - Оптимизированные сборки с использованием Turborepo
  - Возможности реального времени с помощью KeyDB pub/sub

- **🎨 Современный UI/UX**

  - Адаптивный дизайн с использованием Tailwind CSS
  - Переключение между тёмной и светлой темами
  - Поддержка интернационализации (i18n)
  - Красивые UI-компоненты от shadcn/ui
  - Состояния загрузки и обработка ошибок

- **🌐 Интеграция с Web3**

  - Подключение TON кошелька
  - Аутентификация через Web3
  - Обработка транзакций
  - Взаимодействие со смарт-контрактами
  - Blueprint - фреймворк для разработки смарт-контрактов TON

- **🚀 Удобство для разработчиков**

  - Конфигурация ESLint + Prettier
  - Git-хуки с Husky

- **📊 Мониторинг и аналитика**

  - Система логирования с использованием Pino

## 🛠️ Технологический стек

### Frontend

- **Next.js 15** - Фреймворк React с использованием App Router
- **React 19** - Библиотека для создания пользовательских интерфейсов
- **TailwindCSS** - Утилитарный CSS-фреймворк
- **shadcn/ui** - Красиво оформленные компоненты
- **next-themes** - Поддержка тёмного режима
- **next-intl** - Поддержка интернационализации

### Backend

- **Bun** - Молниеносный JavaScript-рантайм
- **tRPC** - Сквозной типобезопасный API
- **Drizzle ORM** - ORM для TypeScript
- **PostgreSQL** - База данных
- **KeyDB** - Высокопроизводительная альтернатива Redis

### Web3

- **TON Connect** - Интеграция с блокчейном TON
- **@ton/ton** - SDK для TON
- **Blueprint** - Фреймворк для разработки смарт-контрактов TON

### DevOps и инструменты

- **Turborepo** - Система сборки для монорепозитория
- **Bun** - JavaScript-рантайм
- **Docker** - Контейнеризация

## 📦 Структура проекта

```
turborepo-ton-trpc/
├── apps/                      # Пакеты приложений
│   ├── web/                   # Фронтенд-приложение на Next.js
│   ├── server/                # tRPC API сервер
│   └── blueprint/             # Смарт-контракты TON
├── packages/                  # Общие пакеты
│   ├── configs/               # Общие конфигурации
│   ├── database/              # Схема базы данных и утилиты
│   ├── logger/                # Утилиты логирования
│   └── tonconnect-ui-react/   # Исправление для TON Connect React
├── turbo.json                 # Конфигурация Turborepo
└── package.json               # Корневой package.json
```

## 🚀 Начало работы

### Предварительные требования

- [Node.js](https://nodejs.org/) (версия 18 или новее)
- [Bun](https://bun.sh/) (версия 1.2.5 или новее)

## 💻 Разработка

```bash
bun dev
```

### Запуск тестов

```bash
bun test        # Запустить все тесты
```

### Проверка стиля и форматирования

```bash
bun lint     # Запустить ESLint
bun format   # Запустить Prettier
```

## 👥 Вклад в проект

Вклады приветствуются! Пожалуйста, не стесняйтесь отправлять Pull Request.

1. Сделайте форк репозитория
2. Создайте новую ветку для своей фичи (`git checkout -b feature/amazing-feature`)
3. Закоммитьте изменения (`git commit -m 'Добавлена потрясающая фича'`)
4. Запушьте ветку (`git push origin feature/amazing-feature`)
5. Откройте Pull Request

## 📄 Лицензия

Этот проект лицензирован под лицензией MIT – см. файл [LICENSE](LICENSE) для подробностей.
