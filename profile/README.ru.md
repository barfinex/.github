<!-- ========================================================== -->
<!-- Barfinex README - Open Core + Enterprise Platform (RU) -->
<!-- ========================================================== -->

<p>
  🌐 <b>Языки:</b>
  <a href="README.md"><code>🇬🇧 English</code></a> ·
  <a href="README.ru.md"><code>🇷🇺 Русский</code></a> ·
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

[![license](https://img.shields.io/badge/license-Apache%202.0%20%2B%20Additional%20Terms-lightgrey)](LICENSE)
[![website](https://img.shields.io/badge/website-barfinex.com-red?logo=firefoxbrowser)](https://barfinex.com)

---

# Open Core + Enterprise: платформа алгоритмической торговли и рыночной аналитики

**Barfinex** — **модульная торговая платформа**, объединяющая **открытое ядро** с **корпоративными аналитикой и управлением**.

Это не просто набор открытых инструментов: проект развивается как **production-ready экосистема** для автоматизации стратегий, рыночной аналитики, решений с поддержкой ИИ и контроля рисков на разных торговых площадках.

На базе **TypeScript + NestJS микросервисов** Barfinex объединяет **рыночные данные, генерацию сигналов, оркестрацию исполнения, телеметрию и операционные API** в единой архитектуре.

</div>

---

## Обзор экосистемы

### Приложения

| Приложение | Описание |
|--------------|-------------|
| [**Provider**](./apps/provider) | Высокопроизводительный шлюз рыночных данных и исполнения. Агрегирует коннекторы, стримит свечи/orderflow, предоставляет REST/WebSocket API и выступает основным интеграционным краем для внешних клиентов и внутренних сервисов. |
| [**Detector**](./apps/detector) | Ядро рантайма стратегий: генерация сигналов в реальном времени, реплей/бэктест, управление жизненным циклом детекторов и политики маршрутизации для оркестрации нескольких стратегий. |
| [**Advisor**](./apps/advisor) | Слой решений с поддержкой ИИ: интерпретация сигналов, составление политик и адаптивная поддержка стратегий. Включает гибридную интеграцию с Signal Engine и корпоративные ML-процессы. |
| [**Inspector**](./apps/inspector) | Пост-трейд риски и надзор: диагностика портфеля, операционный мониторинг, проверка аномалий и аналитика, ориентированная на риски. |

---

## Обзор npm-пакетов

<div align="center">

[![npm organization](https://img.shields.io/badge/npm-@barfinex-cb3837?logo=npm&logoColor=white)](https://www.npmjs.com/org/barfinex)
[![stack](https://img.shields.io/badge/stack-open--core%20%2B%20enterprise-blue)](https://github.com/barfinex)
[![license](https://img.shields.io/badge/license-Apache%202.0%20%2B%20Additional%20Terms-lightgrey)](LICENSE)

</div>

Barfinex поддерживает экосистему пакетов на TypeScript под [`@barfinex`](https://www.npmjs.com/org/barfinex): библиотеки открытого ядра и продвинутые доменные движки для корпоративных приложений.

---

### Основные библиотеки

| npm | Библиотека | Описание |
|-----|----------|-------------|
| [![npm](https://img.shields.io/npm/v/@barfinex/types?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/types) | [**@barfinex/types**](https://www.npmjs.com/package/@barfinex/types) | Общие доменные контракты и строго типизированные интерфейсы для всех сервисов Barfinex. |
| [![npm](https://img.shields.io/npm/v/@barfinex/utils?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/utils) | [**@barfinex/utils**](https://www.npmjs.com/package/@barfinex/utils) | Утилиты: математика, время, форматирование и общие рантайм-сценарии. |
| [![npm](https://img.shields.io/npm/v/@barfinex/config?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/config) | [**@barfinex/config**](https://www.npmjs.com/package/@barfinex/config) | Централизованная конфигурация и управление окружением на основе схем. |
| [![npm](https://img.shields.io/npm/v/@barfinex/key?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/key) | [**@barfinex/key**](https://www.npmjs.com/package/@barfinex/key) | Работа с ключами и учётными данными, безопасность. |
| [![npm](https://img.shields.io/npm/v/@barfinex/connectors?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/connectors) | [**@barfinex/connectors**](https://www.npmjs.com/package/@barfinex/connectors) | Единые адаптеры для подключения к биржам и брокерам через REST и WebSocket. |
| [![npm](https://img.shields.io/npm/v/@barfinex/plugin-driver?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/plugin-driver) | [**@barfinex/plugin-driver**](https://www.npmjs.com/package/@barfinex/plugin-driver) | Рантайм плагинов: обнаружение модулей и оркестрация жизненного цикла. |
| [![npm](https://img.shields.io/npm/v/@barfinex/orders?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/orders) | [**@barfinex/orders**](https://www.npmjs.com/package/@barfinex/orders) | Жизненный цикл ордеров и абстракции исполнения для мульти-рынков. |
| [![npm](https://img.shields.io/npm/v/@barfinex/provider-ws-bridge?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/provider-ws-bridge) | [**@barfinex/provider-ws-bridge**](https://www.npmjs.com/package/@barfinex/provider-ws-bridge) | WebSocket-мост и раздача стримов для потребителей в реальном времени. |
| ![subscription](https://img.shields.io/badge/access-paid%20subscription-orange) | **@barfinex/provider-mcp** *(Подписка)* | Интеграция Model Context Protocol для инструментов Provider API и автоматизации. Доступно по платной подписке; контакт: [barfinex.com](https://barfinex.com). |
| [![npm](https://img.shields.io/npm/v/@barfinex/detector?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/detector) | [**@barfinex/detector**](https://www.npmjs.com/package/@barfinex/detector) | Ядро рантайма детекторов: управление стратегиями, маршрутизация и событийное исполнение. |
| ![subscription](https://img.shields.io/badge/access-paid%20subscription-orange) | **@barfinex/signal-engine** *(Подписка)* | Классификация сигналов и слой решений по тренду/режиму для стратегической логики. Доступно по платной подписке; контакт: [barfinex.com](https://barfinex.com). |
| ![subscription](https://img.shields.io/badge/access-paid%20subscription-orange) | **@barfinex/risk-engine** *(Подписка)* | Pre-trade контроль рисков и политики для безопасного исполнения. Доступно по платной подписке; контакт: [barfinex.com](https://barfinex.com). |
| ![subscription](https://img.shields.io/badge/access-paid%20subscription-orange) | **@barfinex/portfolio-engine** *(Подписка)* | Аллокация и оркестрация на уровне портфеля для мульти-стратегий. Доступно по платной подписке; контакт: [barfinex.com](https://barfinex.com). |
| ![subscription](https://img.shields.io/badge/access-paid%20subscription-orange) | **@barfinex/backtest-engine** *(Подписка)* | Движок исторической симуляции для валидации стратегий и сравнения результатов. Доступно по платной подписке; контакт: [barfinex.com](https://barfinex.com). |
| ![subscription](https://img.shields.io/badge/access-paid%20subscription-orange) | **@barfinex/capital-engine** *(Подписка)* | Логика аллокации капитала с учётом эффективности и рисков. Доступно по платной подписке; контакт: [barfinex.com](https://barfinex.com). |
| [![npm](https://img.shields.io/npm/v/@barfinex/telegram?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/telegram) | [**@barfinex/telegram**](https://www.npmjs.com/package/@barfinex/telegram) | Интеграция с Telegram: уведомления, команды и операционные сценарии. |

---

## Плагины Detector
> Модульные аналитические расширения для рантайма Detector.

| npm | Плагин | Описание |
|-----|---------|-------------|
| [![npm](https://img.shields.io/npm/v/@barfinex/detector-plugin-orderflow-trade-analytics?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/detector-plugin-orderflow-trade-analytics) | [**@barfinex/detector-plugin-orderflow-trade-analytics**](https://www.npmjs.com/package/@barfinex/detector-plugin-orderflow-trade-analytics) | Аналитика ордерфлоу: метрики delta/CVD для интерпретации микроструктуры рынка. |
| [![npm](https://img.shields.io/npm/v/@barfinex/detector-plugin-trade-journal?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/detector-plugin-trade-journal) | [**@barfinex/detector-plugin-trade-journal**](https://www.npmjs.com/package/@barfinex/detector-plugin-trade-journal) | Журнал сделок: структурированные события стратегий, трассы исполнения и пост-анализ. |
| ![subscription](https://img.shields.io/badge/access-paid%20subscription-orange) | **@barfinex/indicators** *(Подписка)* | Набор индикаторов для сигнальных пайплайнов и модулей стратегий (тренд, импульс, волатильность и производные). Доступно по платной подписке; контакт: [barfinex.com](https://barfinex.com). |

---

## Технологический стек

| Слой | Технологии |
|-------|---------------|
| **Ядро платформы** | **TypeScript**, **NestJS**, **Node.js** |
| **Интеграция** | **REST**, **WebSocket**, **MCP (Model Context Protocol)** |
| **Данные** | **Redis**, **MongoDB**, **PostgreSQL**, **QuestDB** |
| **Развёртывание и DevOps** | **Docker**, **GitHub Actions**, **Semantic Release**, **CI/CD** |

---

## Принципы архитектуры

- **Open Core, готовность к enterprise:** открытое ядро с корпоративными модулями для продвинутых операций.
- **Модульность:** чёткие границы сервисов и пакетов для композируемой архитектуры и независимой поставки.
- **Масштабируемость:** событийные потоки, оптимизированные под низкую задержку и высокую пропускную способность.
- **Разделение рисков:** явное разделение pre-trade (`risk-engine`) и пост-трейд (`inspector`) контроля.
- **Эволюция с учётом ИИ:** Advisor и сигнальный домен поддерживают гибридные ML/правила для решений.

---

## Зачем Barfinex

Barfinex объединяет **рыночные данные, логику стратегий, управление исполнением и надзорную аналитику** в одной экосистеме, чтобы команды могли:

- Быстрее разрабатывать и итерировать алгоритмические стратегии.
- Переиспользовать общие движки для бэктеста, аллокации капитала и контроля рисков.
- Встраивать сценарии решений с поддержкой ИИ без нарушения детерминированных границ безопасности.
- Эксплуатировать как открытое ядро, так и корпоративные развёртывания на общей архитектуре.

---

## Включение/отключение модулей по подписке

Корпоративные библиотеки можно включать и отключать без поломки старта открытого ядра:

- Установите `BARFINEX_DISABLE_SUBSCRIPTION_LIBS=true` для принудительного использования адаптеров открытого ядра.
- Точки входа для разработки в режиме open-core:
  - `npm run start:detector:open:dev`
  - `npm run start:advisor:open:dev`
  - `npm run start:mcp:provider:open:dev`
- При отключении корпоративные модули переходят в безопасный fallback и пишут соответствующие сообщения в логах.

---

## Лицензия
Проект распространяется по **Apache License 2.0** с **дополнительными условиями и ограничениями** в [`LICENSE`](./LICENSE).

**Основные пункты:**
1. **Обязательная атрибуция** Barfin Network Limited.
2. **Ограничение коммерческого использования** без предварительного письменного согласия.
3. **Требования к отображению** названия/логотипа/ссылки в производных дистрибутивах и публичном использовании.

По вопросам коммерческого использования и юридическим запросам: [https://barfinex.com](https://barfinex.com).

---

## Ссылки
- [Сайт](https://barfinex.com)
- [Trading Studio](https://studio.barfinex.com)
- [Организация на GitHub](https://github.com/barfinex)
- [Container Registry](https://hub.docker.com/u/barfinex)

---

<div align="center">
  <sub>© 2026 Barfin Network Limited</sub><br/>
  <sub><em>Данные. Стратегия. Исполнение. Управление.</em></sub>
</div>
