<!-- ========================================================== -->
<!-- 🦸‍♂️  Barfinex README — The Open Framework for Algorithmic Trading & Market Intelligence -->
<!-- ========================================================== -->

<p align="center">
  <a href="https://barfin.network/">
    <picture>
      <source srcset="superhero_optimized.webp" type="image/webp" width="450" >
      <img src="superhero_optimized.png" alt="Barfinex Hero" width="450">
    </picture>
  </a>
</p>

<div>

[![docker](https://img.shields.io/badge/docker-ghcr.io%2Fbarfinex-blue?logo=docker)](https://ghcr.io/barfinex)
[![license](https://img.shields.io/badge/license-Apache%202.0-lightgrey)](LICENSE)
[![website](https://img.shields.io/badge/website-barfin.network-red?logo=firefoxbrowser)](https://barfin.network/)

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
| **Advisor** | AI-powered decision engine providing portfolio optimization, market sentiment analysis, and adaptive strategy recommendations. |
| **Detector** | Core signal engine for real-time strategy execution, backtesting, and event-driven alert generation. |
| **Inspector** | Interactive analytics and visualization environment for order-flow analysis, performance diagnostics, and strategy validation. |
| **Provider** | Unified market-data and trading gateway integrating multiple exchanges (spot, futures, and institutional APIs) under a single interface. |

---

### 📚 Core Libraries  

| Library | Description |
|----------|-------------|
| [**@barfinex/types**](https://www.npmjs.com/package/@barfinex/types) ![npm](https://img.shields.io/npm/v/@barfinex/types?color=cb3837&logo=npm) | Shared type definitions ensuring strong compile-time safety across all Barfinex services and plugins. |
| [**@barfinex/utils**](https://www.npmjs.com/package/@barfinex/utils) ![npm](https://img.shields.io/npm/v/@barfinex/utils?color=cb3837&logo=npm) | Foundational utility toolkit including math, time, formatting, and trading data helpers optimized for performance. |
| [**@barfinex/config**](https://www.npmjs.com/package/@barfinex/config) ![npm](https://img.shields.io/npm/v/@barfinex/config?color=cb3837&logo=npm) | Centralized configuration system providing type-safe schema validation and environment management. |
| [**@barfinex/key**](https://www.npmjs.com/package/@barfinex/key) ![npm](https://img.shields.io/npm/v/@barfinex/key?color=cb3837&logo=npm) | Secure key and credential management with encryption, scoped secrets, and runtime validation. |
| [**@barfinex/connectors**](https://www.npmjs.com/package/@barfinex/connectors) ![npm](https://img.shields.io/npm/v/@barfinex/connectors?color=cb3837&logo=npm) | Unified API clients for major exchanges (Binance, Alpaca, Tinkoff, MOEX, etc.) supporting both REST and WebSocket streams. |
| [**@barfinex/plugin-driver**](https://www.npmjs.com/package/@barfinex/plugin-driver) ![npm](https://img.shields.io/npm/v/@barfinex/plugin-driver?color=cb3837&logo=npm) | Core plugin engine enabling dynamic discovery, loading, and lifecycle management of modular components. |
| [**@barfinex/orders**](https://www.npmjs.com/package/@barfinex/orders) ![npm](https://img.shields.io/npm/v/@barfinex/orders?color=cb3837&logo=npm) | Order execution and management framework supporting multiple market types and connectors (spot, futures, sandbox). |
| [**@barfinex/alerts**](https://www.npmjs.com/package/@barfinex/alerts) ![npm](https://img.shields.io/npm/v/@barfinex/alerts?color=cb3837&logo=npm) | Multi-channel alerting framework with Telegram, WebSocket, and custom webhook integrations. |
| [**@barfinex/provider-ws-bridge**](https://www.npmjs.com/package/@barfinex/provider-ws-bridge) ![npm](https://img.shields.io/npm/v/@barfinex/provider-ws-bridge?color=cb3837&logo=npm) | Real-time WebSocket bridge connecting provider streams to external consumers via Redis-based pub/sub channels. |
| [**@barfinex/detector**](https://www.npmjs.com/package/@barfinex/detector) ![npm](https://img.shields.io/npm/v/@barfinex/detector?color=cb3837&logo=npm) | High-level analytics core for strategy execution, signal evaluation, and plugin orchestration. |
| [**@barfinex/advisor**](https://www.npmjs.com/package/@barfinex/advisor) ![npm](https://img.shields.io/npm/v/@barfinex/advisor?color=cb3837&logo=npm) | Machine-learning and rules-based advisor service for strategy scoring, decision-making, and portfolio balancing. |
| [**@barfinex/indicators**](https://www.npmjs.com/package/@barfinex/indicators) ![npm](https://img.shields.io/npm/v/@barfinex/indicators?color=cb3837&logo=npm) | Library of quantitative and volume-based indicators (VWAP, POI, CVD, Candle Volume, Delta Ratio, etc.). |
| [**@barfinex/plugins**](https://www.npmjs.com/package/@barfinex/plugins) ![npm](https://img.shields.io/npm/v/@barfinex/plugins?color=cb3837&logo=npm) | Plugin management and metadata registry for marketplace discovery, installation, and lifecycle integration. |
| [**@barfinex/telegram**](https://www.npmjs.com/package/@barfinex/telegram) ![npm](https://img.shields.io/npm/v/@barfinex/telegram?color=cb3837&logo=npm) | Telegram bot service for alert delivery, control commands, and event-driven interaction. |
| [**@barfinex/plugin-orderflow-trade-analytics**](https://www.npmjs.com/package/@barfinex/plugin-orderflow-trade-analytics) ![npm](https://img.shields.io/npm/v/@barfinex/plugin-orderflow-trade-analytics?color=cb3837&logo=npm) | Advanced microstructure analytics module analyzing trade deltas, volume distribution, and CVD aggregation. |
| [**@barfinex/plugin-trade-journal**](https://www.npmjs.com/package/@barfinex/plugin-trade-journal) ![npm](https://img.shields.io/npm/v/@barfinex/plugin-trade-journal?color=cb3837&logo=npm) | Structured journaling module for trade lifecycle tracking, tagging, and performance attribution. |
| [**@barfinex/volume-follow**](https://www.npmjs.com/package/@barfinex/volume-follow) ![npm](https://img.shields.io/npm/v/@barfinex/volume-follow?color=cb3837&logo=npm) | Execution strategy module for detecting and following large-volume events in live orderflow. |


---

### 🔌 Detector Plugins  

| Plugin | Functionality |
|---------|----------------|
| **Orderflow & Trade Analytics** | Advanced microstructure analysis — Delta Ratio, CVD, VWAP, order book imbalance, and liquidity metrics. |
| **Trade Journal** | Structured trade logging with tagging, performance tracking, and behavioral metrics. |
| **Indicators** | Comprehensive technical toolkit including VWAP, POI, Candle Volume, and more custom indicators. |

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
