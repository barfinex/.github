<!-- ========================================================== -->
<!-- 🦸‍♂️  Barfinex README — The Open Framework for Algorithmic Trading & Market Intelligence -->
<!-- ========================================================== -->

<p align="center">
  <a href="https://barfin.network/">
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
[![website](https://img.shields.io/badge/website-barfin.network-red?logo=firefoxbrowser)](https://barfin.network/)


<p align="center">
  <a href="README.md">
    <img src="https://img.shields.io/badge/🇬🇧_English-2E86DE?style=flat-square" alt="English" />
  </a>
  <a href="README.ru.md">
    <img src="https://img.shields.io/badge/🇷🇺_Русский-2980B9?style=flat-square" alt="Русский" />
  </a>
  <img src="https://img.shields.io/badge/🇰🇿_Қазақша-7F8C8D?style=flat-square" alt="Қазақша (скоро)" />
  <img src="https://img.shields.io/badge/🇨🇳_中文-7F8C8D?style=flat-square" alt="中文 (скоро)" />
</p>


---

# The Open Framework for Algorithmic Trading & Market Intelligence

**Barfinex** is a **modular, enterprise-grade open trading ecosystem** designed to accelerate the development of financial applications, algorithmic trading strategies, and market analytics solutions.  
Our mission is to empower **traders, developers, and researchers** with a unified, extensible framework that bridges **data, intelligence, and execution** across multiple markets and exchanges.  

Through a combination of **scalable microservices, shared libraries, and plug-and-play components**, Barfinex delivers the flexibility and precision required for modern quantitative finance and digital asset markets.  

</div>

---

## 🚀 Ecosystem Overview  

### 🧩 Applications  

| Application | Description |
|--------------|-------------|
| [**Provider**](https://github.com/barfinex/app-provider) | High-performance market data and trading infrastructure providing unified access to multiple exchanges. Acts as the low-latency foundation of the Barfinex ecosystem, aggregating tick-level data, streaming order books, and execution gateways under a consistent API. |
| [**Detector**](https://github.com/barfinex/app-detector) | Core event-driven strategy engine enabling real-time signal generation, automated rule execution, and historical backtesting. Designed for extensibility through modular plugins and seamless integration with custom analytics pipelines. |
| **Advisor** *(Enterprise only)* | Intelligent **AI Agent** for portfolio governance and decision support. Combines quantitative analytics, adaptive risk modeling, and reinforcement learning to provide actionable insights, optimize asset allocation, and adjust trading strategies in dynamic market conditions. |
| **Inspector** *(Enterprise only)* | Comprehensive **risk management and analytics environment** for real-time supervision of portfolio exposure, liquidity stress, and capital efficiency. Enables visualization of order-flow dynamics, performance diagnostics, and automated detection of anomalous trading behavior across multi-asset environments. |



---

## 📦 npm Packages Overview  

<div align="center">

[![npm organization](https://img.shields.io/badge/npm-@barfinex-cb3837?logo=npm&logoColor=white)](https://www.npmjs.com/org/barfinex)
[![packages](https://img.shields.io/badge/packages-12%2B-blue?logo=github&labelColor=gray)](https://www.npmjs.com/org/barfinex)
[![downloads](https://img.shields.io/badge/downloads-growing-success?logo=trendmicro)](https://www.npmjs.com/org/barfinex)
[![license](https://img.shields.io/badge/license-Apache%202.0-lightgrey)](LICENSE)

</div>

Barfinex maintains a collection of **TypeScript-first, enterprise-grade libraries and plugins** published under the  
[`@barfinex`](https://www.npmjs.com/org/barfinex) organization on npm.  
Each package follows strict semantic versioning, full type safety, and unified API design principles to ensure consistency  
across applications, analytics modules, and trading services.

---

### 📚 Core Libraries  

| npm | Library | Description |
|-----|----------|-------------|
| [![npm](https://img.shields.io/npm/v/@barfinex/types?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/types) | [**@barfinex/types**](https://www.npmjs.com/package/@barfinex/types) | Shared type definitions ensuring strong compile-time safety across all Barfinex services and plugins. |
| [![npm](https://img.shields.io/npm/v/@barfinex/utils?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/utils) | [**@barfinex/utils**](https://www.npmjs.com/package/@barfinex/utils) | Foundational utility toolkit including math, time, formatting, and trading data helpers optimized for performance. |
| [![npm](https://img.shields.io/npm/v/@barfinex/config?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/config) | [**@barfinex/config**](https://www.npmjs.com/package/@barfinex/config) | Centralized configuration system providing type-safe schema validation and environment management. |
| [![npm](https://img.shields.io/npm/v/@barfinex/key?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/key) | [**@barfinex/key**](https://www.npmjs.com/package/@barfinex/key) | Secure key and credential management with encryption, scoped secrets, and runtime validation. |
| [![npm](https://img.shields.io/npm/v/@barfinex/connectors?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/connectors) | [**@barfinex/connectors**](https://www.npmjs.com/package/@barfinex/connectors) | Unified API clients for major exchanges (Binance, Alpaca, Tinkoff, MOEX, etc.) supporting both REST and WebSocket streams. |
| [![npm](https://img.shields.io/npm/v/@barfinex/plugin-driver?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/plugin-driver) | [**@barfinex/plugin-driver**](https://www.npmjs.com/package/@barfinex/plugin-driver) | Core plugin engine enabling dynamic discovery, loading, and lifecycle management of modular components. |
| [![npm](https://img.shields.io/npm/v/@barfinex/orders?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/orders) | [**@barfinex/orders**](https://www.npmjs.com/package/@barfinex/orders) | Order execution and management framework supporting multiple market types and connectors (spot, futures, sandbox). |
| [![npm](https://img.shields.io/npm/v/@barfinex/provider-ws-bridge?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/provider-ws-bridge) | [**@barfinex/provider-ws-bridge**](https://www.npmjs.com/package/@barfinex/provider-ws-bridge) | Real-time WebSocket bridge connecting provider streams to external consumers via Redis-based pub/sub channels. |
| [![npm](https://img.shields.io/npm/v/@barfinex/detector?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/detector) | [**@barfinex/detector**](https://www.npmjs.com/package/@barfinex/detector) | High-level analytics core for strategy execution, signal evaluation, and plugin orchestration. |
| [![npm](https://img.shields.io/npm/v/@barfinex/telegram?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/telegram) | [**@barfinex/telegram**](https://www.npmjs.com/package/@barfinex/telegram) | Telegram bot service for alert delivery, control commands, and event-driven interaction. |


---

## 🔌 Detector Plugins  
> **Enterprise-grade extensions for advanced analytics, journaling, and order-flow intelligence.**  
> Core analytical modules that extend the capabilities of the `Detector` engine with plug-and-play integrations for real-time market interpretation, trade journaling, and liquidity analysis.


| npm | Plugin | Description |
|-----|---------|-------------|
| [![npm](https://img.shields.io/npm/v/@barfinex/detector-plugin-orderflow-trade-analytics?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/detector-plugin-orderflow-trade-analytics) | [**@barfinex/detector-plugin-orderflow-trade-analytics**](https://www.npmjs.com/package/@barfinex/detector-plugin-orderflow-trade-analytics) | **Orderflow & Trade Analytics (Light Edition)** — Provides essential order-flow metrics such as Delta Ratio, CVD, and Volume Distribution. Enables real-time monitoring of market microstructure for retail and institutional strategies. The full Enterprise edition includes extended analytics (VWAP deviations, volume clusters, liquidity pressure, and trade heatmaps). |
| [![npm](https://img.shields.io/npm/v/@barfinex/detector-plugin-trade-journal?color=cb3837&logo=npm)](https://www.npmjs.com/package/@barfinex/detector-plugin-trade-journal) | [**@barfinex/detector-plugin-trade-journal**](https://www.npmjs.com/package/@barfinex/detector-plugin-trade-journal) | **Trade Journal (Light Edition)** — Simplified structured journaling module for recording and reviewing executed trades, strategy tags, and performance snapshots. The Enterprise edition extends functionality with advanced behavioral metrics, PnL attribution, and psychological trade scoring models. |
| 📈 | **@barfinex/indicators** *(Enterprise only)* | Complete suite of quantitative and volume-based indicators, including enhanced VWAP, POI, Delta, and Candle Volume models with multi-resolution aggregation. Delivered as part of the Enterprise analytics bundle. |


---

## 🛠️ Technology Stack  

| Layer | Technologies |
|-------|---------------|
| **Core Platform** | **TypeScript**, **NestJS**, **Node.js** |
| **Data Visualization** | **klinecharts** with custom indicators and overlays |
| **Data Infrastructure** | **Redis**, **MongoDB**, **PostgreSQL** for storage, caching, and streaming |
| **Deployment & DevOps** | **Docker**, **GitHub Actions**, **Semantic Release**, and full CI/CD automation |

---

## 💡 Architecture Principles  

- **Modularity:** Every component is isolated, reusable, and composable.  
- **Observability:** Unified logging, tracing, and monitoring across all services.  
- **Scalability:** Horizontally scalable architecture optimized for low latency and high throughput.  
- **Extensibility:** Plug-and-play interface for third-party plugins, indicators, and AI models.  
- **Transparency:** Open ecosystem governed by clear API contracts and semantic versioning.  

---

## 🧭 Why Barfinex  

Barfinex unifies **market data, analytics, and execution pipelines** within a single ecosystem, enabling teams to:  

- Develop and deploy trading algorithms faster with minimal boilerplate.  
- Access standardized APIs for data ingestion, simulation, and execution.  
- Integrate AI-driven decision modules and research pipelines seamlessly.  
- Collaborate within a shared open-source architecture built for growth.  

---

## 📄 License
This project is licensed under the [Apache License 2.0](LICENSE) with additional restrictions.

**Key Terms:**
1. **Attribution**: Proper credit must be given to the original author. Include  
   “Barfin Network Limited” and a link to the official repository or website.  
2. **Non-Commercial Use**: Commercial use is **prohibited** without explicit written permission.  
3. **Display Requirements**:  
   - The name “Barfin Network Limited”  
   - The official logo  
   - A working link to [https://barfin.network](https://barfin.network)

For permission requests, contact **Barfin Network Limited** via  
[https://barfin.network](https://barfin.network)

---

## 🌍 Links
- 🌐 [Website](https://barfin.network)  
- 🧭 [Trading Studio](https://studio.barfinex.com)  
- 💼 [GitHub Organization](https://github.com/barfinex)  
- 🧱 [Docker Packages](https://ghcr.io/barfinex)

---

<div align="center">
  <sub>© 2025 Barfin Network Limited — Empowering Financial Intelligence</sub><br/>
  <sub><em>Data. Strategy. Execution.</em></sub>
</div>
