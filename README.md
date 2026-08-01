# Awesome-5g-Network-Analytics

## Similar Projects to 5G Network Analytics Platforms

**5G Network Analytics** platforms collect, process, and analyze performance data from Radio Access Networks (RAN), core networks, and user equipment. They support KPI monitoring, anomaly detection, root-cause analysis, capacity planning, experience management, and AI/ML-driven insights for 5G (and 4G) networks. Leading commercial tools include Nokia AVA, Ericsson Expert Analytics, Viavi, EXFO, Accedian, Mobileum, Subex, Cellwize, Infovista, and Matellio Telecom Analytics.

Below is a **curated list** of notable platforms and their open-source equivalents. Fully featured commercial-grade 5G analytics suites with multi-vendor correlation and large-scale AI are rare in pure open source. The emphasis is on **open-source building blocks**, 5G core/RAN stacks with analytics capabilities, O-RAN monitoring tools, and general observability platforms that can be adapted for telecom use cases.

## 🏢 SaaS / Hosted Platforms

- **[Nokia AVA](https://www.nokia.com/)** — AI-powered analytics and automation suite for multi-domain network assurance, optimization, and predictive insights.
- **[Ericsson Expert Analytics](https://www.ericsson.com/)** — Advanced analytics platform focused on network performance, subscriber experience, and operational intelligence.
- **[Viavi](https://www.viavisolutions.com/)** — Network testing, assurance, and analytics solutions covering RAN, core, and service quality for 5G.
- **[EXFO](https://www.exfo.com/)** — Test, monitoring, and analytics portfolio for fiber, 5G, and service assurance.
- **[Accedian](https://www.accedian.com/)** — Performance analytics and assurance focused on quality of experience and network visibility.
- **[Mobileum](https://www.mobileum.com/)** — Analytics and security platform for roaming, fraud, and network intelligence.
- **[Subex](https://www.subex.com/)** — Revenue assurance, fraud management, and network analytics solutions for telecom operators.
- **[Cellwize](https://www.cellwize.com/)** (now part of larger portfolios) — RAN automation and analytics platform.
- **[Infovista](https://www.infovista.com/)** — Network performance management, planning, and analytics for mobile operators.
- **[Matellio Telecom Analytics](https://www.matellio.com/)** and similar specialized telecom analytics offerings — Custom and productized analytics solutions for 5G networks.

## 🔓 Open-Source Software

### 5G Core / RAN Stacks with Analytics Capabilities
- **[Free5GC](https://github.com/free5gc/free5gc)** — Popular open-source 5G core network implementation. Community and research projects add **NWDAF** (Network Data Analytics Function) support for event-driven analytics, subscription/notification, and predictive insights.
- **[Open5GS](https://github.com/open5gs/open5gs)** — Open-source 5G core (and 4G EPC) frequently used in testbeds; can be instrumented for performance monitoring and analytics.
- **[OpenAirInterface (OAI)](https://openairinterface.org/)** — Full-stack open-source 5G RAN and core. Widely used for research, with extensions for telemetry, xApps, and analytics.
- **[srsRAN](https://github.com/srsran/srsRAN_Project)** — Open-source 4G/5G RAN software suite. Useful for generating realistic traffic and KPIs in lab environments.
- **Open-source NWDAF implementations** — Multiple research and community projects integrate NWDAF with Free5GC, Open5GS, or OAI to provide standardized 5G analytics (event exposure, ML-based insights, closed-loop automation).

### O-RAN & RAN Intelligent Controller (RIC) Monitoring
- **[FlexRIC](https://gitlab.eurecom.fr/mosaic5g/flexric)** / SD-RAN related projects — Open near-real-time RIC frameworks that enable xApps for RAN monitoring, KPI collection, and analytics.
- **[5G-Spector](https://github.com/5GSEC/5G-Spector)** and similar O-RAN xApps — Security and monitoring xApps that extract fine-grained RAN telemetry (e.g., MobiFlow) for analysis and anomaly detection.
- Community O-RAN monitoring stacks that combine E2 interface metrics with Prometheus/Grafana or Zabbix.

### General Observability & Analytics Tooling (Highly Adaptable)
- **[Prometheus](https://prometheus.io/) + [Grafana](https://grafana.com/)** — De-facto open-source monitoring and visualization stack. Widely used to scrape and dashboard 5G KPIs, logs, and metrics from open-source cores and RANs.
- **[OpenTelemetry](https://opentelemetry.io/)** — Vendor-neutral observability framework for traces, metrics, and logs; increasingly applied to telecom workloads.
- **ELK / OpenSearch stack** — For log aggregation, search, and analytics of network events and KPIs.
- **[MobileInsight](https://github.com/mobileinsight-project)** (and 5G extensions) — UE-side protocol tracing and analytics tool for cellular networks.

### Supporting & Research-Oriented Tools
- **5G Trace Analyzer** and similar open-source sequence/trace analysis tools for decoding and visualizing 5G signaling.
- **NVIDIA Aerial** components (parts being open-sourced) — CUDA-accelerated RAN and digital-twin related software useful for AI-native analytics research.
- Various GitHub projects for 5G KPI anomaly detection, root-cause analysis (RAG-based assistants), and traffic generators that feed analytics pipelines.

### Typical Open-Source Approach
Operators and researchers commonly assemble:
1. An open 5G core/RAN (Free5GC, Open5GS, OAI, or srsRAN)
2. Telemetry collection via NWDAF, xApps, or exporters
3. Prometheus + Grafana (or OpenTelemetry) for storage and dashboards
4. Optional ML pipelines for anomaly detection and prediction

This stack provides strong visibility and experimentation capability, though it requires more integration effort than commercial multi-vendor analytics platforms.

---

**How to contribute**  
Fork this repository, add a new project (with link + short description + category), and open a pull request.  
Prefer actively maintained open-source projects related to 5G analytics, NWDAF, O-RAN monitoring, or telecom observability.

**License**  
This list is public domain / CC0. Feel free to copy into your own awesome list or README.

Star the projects you find useful — open 5G analytics and observability tooling continues to grow with the O-RAN and open-source 5G ecosystems! 📶

