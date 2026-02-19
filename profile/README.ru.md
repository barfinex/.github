<!-- ========================================================== -->
<!-- 🦸‍♂️  Barfinex README — Открытая Платформа для Алгоритмической Торговли и Рыночной Аналитики -->
<!-- ========================================================== -->

<p >
  🌐 <b>Языки:</b>  
  <a href="README.md"><code>🇬🇧 English</code></a> ·
  <a href="README.ru.md?cache=20251030092013"><code>🇷🇺 Русский</code></a> ·
  <code style="color:gray;">🇰🇿 Қазақша</code> ·
  <code style="color:gray;">🇨🇳 中文</code>
</p>

<p align="center">
  <a href="https://barfinex.com">
    <picture>
      <source srcset="https://raw.githubusercontent.com/barfinex/.github/main/profile/superhero_small.webp" type="image/webp">
      <img src="https://raw.githubusercontent.com/barfinex/.github/main/profile/superhero_small.png" alt="Barfinex Hero" width="300">
    </picture>
  </a>
</p>

<div>

[![ghcr](https://img.shields.io/badge/GHCR-ghcr.io%2Fbarfinex%2Fprovider-blue?logo=github&logoColor=white)](https://ghcr.io/barfinex/provider)
[![dockerhub](https://img.shields.io/badge/DockerHub-barfinex%2Fprovider-blue?logo=docker&logoColor=white)](https://hub.docker.com/r/barfinex/provider)
[![image-size](https://img.shields.io/docker/image-size/barfinex/provider/latest?label=image%20size)](https://ghcr.io/barfinex/provider)
[![version](https://img.shields.io/badge/version-auto--updated-success)](https://ghcr.io/barfinex/provider)

[![license](https://img.shields.io/badge/license-Apache%202.0-lightgrey)](LICENSE)
[![website](https://img.shields.io/badge/website-barfinex.com-red?logo=firefoxbrowser)](https://barfinex.com)

---

# Открытая Платформа для Алгоритмической Торговли и Рыночного Интеллекта

**Barfinex** — это **модульная, корпоративного уровня открытая торговая экосистема**, созданная для ускорения разработки финансовых приложений, алгоритмических стратегий и аналитических решений.  
Наша миссия — предоставить **трейдерам, разработчикам и исследователям** единую платформу, объединяющую **данные, интеллект и исполнение** в разных рынках и на различных биржах.  

Благодаря комбинации **масштабируемых микросервисов, общих библиотек и подключаемых компонентов**, Barfinex обеспечивает гибкость и точность, необходимые для современной количественной аналитики и цифровых активов.  

</div>

---

## 🚀 Обзор Экосистемы  

### 🧩 Приложения  

| Приложение | Описание |
|-------------|-----------|
| [**Provider**](https://github.com/barfinex/app-provider) | Высокопроизводительная инфраструктура рыночных данных и торговых операций, обеспечивающая единый доступ к множеству бирж. Является низколатентным фундаментом экосистемы Barfinex, агрегируя потоковые данные, стаканы и шлюзы исполнения под единым API. |
| [**Detector**](https://github.com/barfinex/app-detector) | Основной событийно-ориентированный движок стратегий, обеспечивающий генерацию торговых сигналов в реальном времени, автоматическое выполнение правил и историческое тестирование. Поддерживает расширения через модульные плагины и интеграцию с аналитическими пайплайнами. |
| **Advisor** *(только Enterprise)* | Интеллектуальный **AI-агент** для управления портфелем и поддержки решений. Объединяет количественную аналитику, адаптивное моделирование рисков и методы обучения с подкреплением, предлагая оптимизацию активов и динамическую настройку стратегий под рыночные условия. |
| **Inspector** *(только Enterprise)* | Комплексная среда **риск-менеджмента и аналитики** для мониторинга экспозиции, ликвидности и эффективности капитала в реальном времени. Позволяет визуализировать потоки ордеров, диагностировать производительность и выявлять аномалии торгового поведения на мульти-активных рынках. |

---

## 📦 Обзор npm-пакетов  

<div align="center">

[![npm organization](https://img.shields.io/badge/npm-@barfinex-cb3837?logo=npm&logoColor=white)](https://www.npmjs.com/org/barfinex)
[![packages](https://img.shields.io/badge/packages-12%2B-blue?logo=github&labelColor=gray)](https://www.npmjs.com/org/barfinex)
[![downloads](https://img.shields.io/badge/downloads-growing-success?logo=trendmicro)](https://www.npmjs.com/org/barfinex)
[![license](https://img.shields.io/badge/license-Apache%202.0-lightgrey)](LICENSE)

</div>

Barfinex поддерживает набор **TypeScript-библиотек и плагинов корпоративного уровня**, опубликованных под  
организацией [`@barfinex`](https://www.npmjs.com/org/barfinex) в npm.  
Каждый пакет следует строгому семантическому версионированию, обладает полной типизацией и едиными принципами API-дизайна, обеспечивая согласованность  
между приложениями, аналитическими модулями и торговыми сервисами.

---

### 📚 Основные библиотеки  

| npm | Библиотека | Описание |
|-----|-------------|-----------|
| [**@barfinex/types**](https://www.npmjs.com/package/@barfinex/types) | Общие типы, обеспечивающие строгую типизацию на уровне компиляции для всех сервисов и плагинов Barfinex. |
| [**@barfinex/utils**](https://www.npmjs.com/package/@barfinex/utils) | Набор утилит: математика, время, форматирование и торговые помощники, оптимизированные по производительности. |
| [**@barfinex/config**](https://www.npmjs.com/package/@barfinex/config) | Централизованная система конфигурации с безопасной типизацией и валидацией окружения. |
| [**@barfinex/key**](https://www.npmjs.com/package/@barfinex/key) | Безопасное управление ключами и учетными данными с шифрованием и проверкой в рантайме. |
| [**@barfinex/connectors**](https://www.npmjs.com/package/@barfinex/connectors) | Унифицированные клиенты API для основных бирж (Binance, Alpaca, Tinkoff, MOEX и др.) с поддержкой REST и WebSocket. |
| [**@barfinex/plugin-driver**](https://www.npmjs.com/package/@barfinex/plugin-driver) | Основной движок плагинов для динамического поиска, загрузки и управления жизненным циклом модулей. |
| [**@barfinex/orders**](https://www.npmjs.com/package/@barfinex/orders) | Фреймворк управления ордерами с поддержкой спота, фьючерсов и песочницы. |
| [**@barfinex/provider-ws-bridge**](https://www.npmjs.com/package/@barfinex/provider-ws-bridge) | Мост WebSocket для ретрансляции потоков данных провайдера через Redis Pub/Sub-каналы. |
| [**@barfinex/detector**](https://www.npmjs.com/package/@barfinex/detector) | Высокоуровневый аналитический модуль для исполнения стратегий, оценки сигналов и оркестрации плагинов. |
| [**@barfinex/telegram**](https://www.npmjs.com/package/@barfinex/telegram) | Telegram-сервис для уведомлений, управления и интерактивных команд. |

---

## 🔌 Плагины Detector  
> **Расширения корпоративного уровня для продвинутой аналитики, журналирования и анализа ордер-флоу.**  
> Ядро аналитических модулей, расширяющих возможности движка `Detector` через подключаемые интеграции для анализа ликвидности, потоков и поведения рынка.

| npm | Плагин | Описание |
|-----|---------|-----------|
| [**@barfinex/detector-plugin-orderflow-trade-analytics**](https://www.npmjs.com/package/@barfinex/detector-plugin-orderflow-trade-analytics) | **Orderflow & Trade Analytics (Лайт-версия)** — ключевые метрики потока ордеров: Delta Ratio, CVD, распределение объема. Позволяет в реальном времени отслеживать микроструктуру рынка для розничных и институциональных стратегий. Полная Enterprise-версия включает расширенные метрики (отклонения VWAP, кластеры объема, давление ликвидности и тепловые карты сделок). |
| [**@barfinex/detector-plugin-trade-journal**](https://www.npmjs.com/package/@barfinex/detector-plugin-trade-journal) | **Trade Journal (Лайт-версия)** — модуль журналирования сделок: запись, классификация и анализ эффективности стратегий. Enterprise-версия добавляет поведенческую аналитику, атрибуцию PnL и психологическую оценку трейдов. |
| 📈 | **@barfinex/indicators** *(только Enterprise)* | Полный набор количественных и объемных индикаторов (VWAP, POI, Delta, Candle Volume и др.) с мульти-таймфреймной агрегацией. |

---

## 🛠️ Технологический стек  

| Уровень | Технологии |
|----------|-------------|
| **Основная платформа** | **TypeScript**, **NestJS**, **Node.js** |
| **Визуализация данных** | **klinecharts** с кастомными индикаторами и оверлеями |
| **Инфраструктура данных** | **Redis**, **MongoDB**, **PostgreSQL** — для хранения, кэширования и потоковой обработки |
| **Развертывание и DevOps** | **Docker**, **GitHub Actions**, **Semantic Release**, полная CI/CD-автоматизация |

---

## 💡 Архитектурные принципы  

- **Модульность:** каждый компонент изолирован и переиспользуем.  
- **Наблюдаемость:** единая система логирования, трейсинга и метрик.  
- **Масштабируемость:** горизонтально масштабируемая архитектура с низкой задержкой.  
- **Расширяемость:** открытый интерфейс для сторонних плагинов, индикаторов и AI-моделей.  
- **Прозрачность:** открытая экосистема с четкими API-контрактами и версионированием.  

---

## 🧭 Почему Barfinex  

Barfinex объединяет **данные, аналитику и исполнение** в единой экосистеме, позволяя командам:

- Разрабатывать и внедрять торговые алгоритмы быстрее и безопаснее.  
- Использовать стандартизированные API для получения, моделирования и исполнения данных.  
- Интегрировать AI-модули принятия решений и исследовательские пайплайны.  
- Работать совместно в открытой архитектуре, готовой к росту и масштабированию.  

---

## 📄 Лицензия
Проект распространяется под [лицензией Apache 2.0](LICENSE) с дополнительными ограничениями.

**Основные условия:**
1. **Атрибуция:** необходимо указывать авторство «Barfin Network Limited» и ссылку на официальный репозиторий или сайт.  
2. **Некомерческое использование:** коммерческое использование **запрещено** без письменного разрешения.  
3. **Требования к отображению:**  
   - Название «Barfin Network Limited»  
   - Официальный логотип  
   - Активная ссылка на [https://barfinex.com](https://barfinex.com)

Для получения разрешения обращайтесь через  
[https://barfinex.com](https://barfinex.com)

---

## 🌍 Ссылки
- 🌐 [Сайт](https://barfinex.com)  
- 🧭 [Trading Studio](https://studio.barfinex.com)  
- 💼 [GitHub-организация](https://github.com/barfinex)  
- 🧱 [Docker-пакеты](https://ghcr.io/barfinex)

---

<div align="center">
  <sub>© 2025 Barfin Network Limited — Разум Финансовых Рынков</sub><br/>
  <sub><em>Данные. Стратегия. Исполнение.</em></sub>
</div>
