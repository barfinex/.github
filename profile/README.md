<!-- ========================================================== -->
<!-- Barfinex README - Open Core + Enterprise Platform -->
<!-- ========================================================== -->

<p>
  🌐 <b>Languages:</b>
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

# Open Core + Enterprise Platform for Algorithmic Trading and Market Intelligence

**Barfinex** is a **modular trading platform** that combines an **open-core engineering foundation** with **enterprise analytics and governance layers**.

It is no longer just a standalone open-source toolkit: the project now evolves as a **production-grade ecosystem** for strategy automation, market intelligence, AI-assisted decisioning, and risk supervision across multiple trading venues.

Built on **TypeScript + NestJS microservices**, Barfinex unifies **market data, signal generation, execution orchestration, telemetry, and operational APIs** in one architecture.

</div>

---

## Ecosystem Overview

### Applications

| Application | Description |
|--------------|-------------|
| [**Provider**](./apps/provider) | High-performance market data and execution gateway. Aggregates connectors, streams candles/orderflow, exposes REST/WebSocket APIs, and acts as the primary integration edge for external clients and internal services. |
| [**Detector**](./apps/detector) | Core strategy runtime for real-time signal generation, replay/backtest flows, detector lifecycle control, and routing policies for multi-strategy orchestration. |
| [**Advisor**](./apps/advisor) | AI-assisted decision layer for signal interpretation, policy composition, and adaptive strategy support. Includes hybrid integration with Signal Engine and enterprise ML workflows. |
| [**Inspector**](./apps/inspector) | Post-trade risk and supervision domain for portfolio diagnostics, operational monitoring, anomaly inspection, and risk-focused analytics. |

---

## npm Packages Overview

<div align="center">

[![npm organization](https://img.shields.io/badge/npm-@barfinex-cb3837?logo=npm&logoColor=white)](https://www.npmjs.com/org/barfinex)
[![stack](https://img.shields.io/badge/stack-open--core%20%2B%20enterprise-blue)](https://github.com/barfinex)
[![license](https://img.shields.io/badge/license-Apache%202.0%20%2B%20Additional%20Terms-lightgrey)](LICENSE)

</div>

Barfinex maintains a TypeScript-first package ecosystem under [`@barfinex`](https://www.npmjs.com/org/barfinex), including open-core infrastructure libraries and advanced domain engines used by enterprise applications.

---

### Core Libraries

| npm | Library | Description |
|-----|----------|-------------|
| [![npm](https://img.shields.io/npm/v/@barfinex/types?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/types) | [**@barfinex/types**](https://www.npmjs.com/package/@barfinex/types) | Shared domain contracts and strongly typed interfaces across all Barfinex services. |
| [![npm](https://img.shields.io/npm/v/@barfinex/utils?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/utils) | [**@barfinex/utils**](https://www.npmjs.com/package/@barfinex/utils) | Utility layer with reusable helpers for math, time, formatting, and common runtime workflows. |
| [![npm](https://img.shields.io/npm/v/@barfinex/config?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/config) | [**@barfinex/config**](https://www.npmjs.com/package/@barfinex/config) | Centralized configuration and schema-driven environment management. |
| [![npm](https://img.shields.io/npm/v/@barfinex/key?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/key) | [**@barfinex/key**](https://www.npmjs.com/package/@barfinex/key) | Key and credential handling library with security-oriented helpers. |
| [![npm](https://img.shields.io/npm/v/@barfinex/connectors?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/connectors) | [**@barfinex/connectors**](https://www.npmjs.com/package/@barfinex/connectors) | Unified adapters for exchange and broker connectivity via REST and WebSocket channels. |
| [![npm](https://img.shields.io/npm/v/@barfinex/plugin-driver?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/plugin-driver) | [**@barfinex/plugin-driver**](https://www.npmjs.com/package/@barfinex/plugin-driver) | Plugin runtime for dynamic module discovery and lifecycle orchestration. |
| [![npm](https://img.shields.io/npm/v/@barfinex/orders?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/orders) | [**@barfinex/orders**](https://www.npmjs.com/package/@barfinex/orders) | Order lifecycle and execution abstractions for multi-market integrations. |
| [![npm](https://img.shields.io/npm/v/@barfinex/provider-ws-bridge?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/provider-ws-bridge) | [**@barfinex/provider-ws-bridge**](https://www.npmjs.com/package/@barfinex/provider-ws-bridge) | WebSocket bridge and stream fan-out layer for real-time consumers. |
| ![subscription](https://img.shields.io/badge/access-paid%20subscription-orange) | **@barfinex/provider-mcp** *(Subscription)* | Model Context Protocol integration layer for Provider API tooling and automation flows. Available via paid subscription; contact us at [barfinex.com](https://barfinex.com). |
| [![npm](https://img.shields.io/npm/v/@barfinex/detector?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/detector) | [**@barfinex/detector**](https://www.npmjs.com/package/@barfinex/detector) | Detector runtime core for strategy management, routing, and event-driven execution. |
| ![subscription](https://img.shields.io/badge/access-paid%20subscription-orange) | **@barfinex/signal-engine** *(Subscription)* | Signal classification and trend/regime decision layer for higher-level strategy logic. Available via paid subscription; contact us at [barfinex.com](https://barfinex.com). |
| ![subscription](https://img.shields.io/badge/access-paid%20subscription-orange) | **@barfinex/risk-engine** *(Subscription)* | Pre-trade risk controls and policy primitives for safe execution gating. Available via paid subscription; contact us at [barfinex.com](https://barfinex.com). |
| ![subscription](https://img.shields.io/badge/access-paid%20subscription-orange) | **@barfinex/portfolio-engine** *(Subscription)* | Portfolio-level allocation and orchestration helpers for multi-strategy environments. Available via paid subscription; contact us at [barfinex.com](https://barfinex.com). |
| ![subscription](https://img.shields.io/badge/access-paid%20subscription-orange) | **@barfinex/backtest-engine** *(Subscription)* | Historical simulation engine for strategy validation and performance comparison. Available via paid subscription; contact us at [barfinex.com](https://barfinex.com). |
| ![subscription](https://img.shields.io/badge/access-paid%20subscription-orange) | **@barfinex/capital-engine** *(Subscription)* | Capital allocation logic for efficiency-aware and risk-aware deployment scenarios. Available via paid subscription; contact us at [barfinex.com](https://barfinex.com). |
| [![npm](https://img.shields.io/npm/v/@barfinex/telegram?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/telegram) | [**@barfinex/telegram**](https://www.npmjs.com/package/@barfinex/telegram) | Telegram integration for notifications, commands, and operational workflows. |

---

## Detector Plugins
> Modular analytics extensions for the Detector runtime.

| npm | Plugin | Description |
|-----|---------|-------------|
| [![npm](https://img.shields.io/npm/v/@barfinex/detector-plugin-orderflow-trade-analytics?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/detector-plugin-orderflow-trade-analytics) | [**@barfinex/detector-plugin-orderflow-trade-analytics**](https://www.npmjs.com/package/@barfinex/detector-plugin-orderflow-trade-analytics) | Orderflow analytics plugin with delta/CVD-focused metrics for market microstructure interpretation. |
| [![npm](https://img.shields.io/npm/v/@barfinex/detector-plugin-trade-journal?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/detector-plugin-trade-journal) | [**@barfinex/detector-plugin-trade-journal**](https://www.npmjs.com/package/@barfinex/detector-plugin-trade-journal) | Trade journaling plugin for structured strategy events, execution traces, and post-analysis workflows. |
| [![npm](https://img.shields.io/npm/v/@barfinex/indicators?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/indicators) | [**@barfinex/indicators**](https://www.npmjs.com/package/@barfinex/indicators) | Indicator toolkit used by signal pipelines and strategy modules (trend, momentum, volatility, and derived transforms). |

---

## Technology Stack

| Layer | Technologies |
|-------|---------------|
| **Core Platform** | **TypeScript**, **NestJS**, **Node.js** |
| **Integration** | **REST**, **WebSocket**, **MCP (Model Context Protocol)** |
| **Data Infrastructure** | **Redis**, **MongoDB**, **PostgreSQL**, **QuestDB** |
| **Deployment & DevOps** | **Docker**, **GitHub Actions**, **Semantic Release**, **CI/CD pipelines** |

---

## Architecture Principles

- **Open Core, Enterprise Ready:** Open engineering foundation with enterprise modules for advanced operations.
- **Modularity:** Service and package boundaries enable composable architecture and independent delivery.
- **Scalability:** Event-driven workflows optimized for low-latency, high-throughput market processing.
- **Risk Separation:** Explicit split between pre-trade (`risk-engine`) and post-trade (`inspector`) controls.
- **AI-Native Evolution:** Advisor and signal domains support hybrid ML/rule-based decision strategies.

---

## Why Barfinex

Barfinex unifies **market data, strategy logic, execution control, and supervisory analytics** into one ecosystem so teams can:

- Build and iterate on algorithmic strategies faster.
- Reuse shared engines for backtesting, capital allocation, and risk control.
- Integrate AI-assisted decision workflows without breaking deterministic safety boundaries.
- Operate both open-core and enterprise deployments on a common architecture.

---

## License
This project uses **Apache License 2.0** with **additional terms and restrictions** defined in [`LICENSE`](./LICENSE).

**Key terms include:**
1. **Attribution required** to Barfin Network Limited.
2. **Commercial use restriction** without prior written consent.
3. **Display requirements** for name/logo/link in derivative distributions and public-facing usage.

For commercial permissions and legal requests, contact via [https://barfinex.com](https://barfinex.com).

---

## Links
- [Website](https://barfinex.com)
- [Trading Studio](https://studio.barfinex.com)
- [GitHub Organization](https://github.com/barfinex)
- [Container Registry](https://ghcr.io/barfinex)

---

<div align="center">
  <sub>© 2026 Barfin Network Limited</sub><br/>
  <sub><em>Data. Strategy. Execution. Governance.</em></sub>
</div>
