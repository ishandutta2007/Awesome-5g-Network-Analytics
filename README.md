# Awesome-5g-Network-Analytics

## Similar Projects to 5G Network Analytics Platforms

**5G Network Analytics** platforms collect, process, and analyze performance data from Radio Access Networks (RAN), core networks, and user equipment. They support KPI monitoring, anomaly detection, root-cause analysis, capacity planning, experience management, and AI/ML-driven insights for 5G (and 4G) networks. Leading commercial tools include Nokia AVA, Ericsson Expert Analytics, Viavi, EXFO, Accedian, Mobileum, Subex, Cellwize, Infovista, and Matellio Telecom Analytics.

Below is a **curated list** of notable platforms and their open-source equivalents. Fully featured commercial-grade 5G analytics suites with multi-vendor correlation and large-scale AI are rare in pure open source. The emphasis is on **open-source building blocks**, 5G core/RAN stacks with analytics capabilities, O-RAN monitoring tools, and general observability platforms that can be adapted for telecom use cases.

## 🏢 SaaS / Hosted Platforms

| Platform | Description | Pricing | Free Tier / Limit | Company Size (Est. Revenue/Valuation) |
| :--- | :--- | :--- | :--- | :--- |
| **[Ericsson Expert Analytics](https://www.ericsson.com/)** | Advanced analytics platform focused on network performance, subscriber experience, and operational intelligence. | Custom (Contact Sales) | None | ~$25 Billion (Annual Revenue) |
| **[Nokia AVA](https://www.nokia.com/)** | AI-powered analytics and automation suite for multi-domain network assurance, optimization, and predictive insights. | Custom (Contact Sales) | None | ~$24 Billion (Annual Revenue) |
| **[Viavi](https://www.viavisolutions.com/)** | Network testing, assurance, and analytics solutions covering RAN, core, and service quality for 5G. | Custom (Contact Sales) | None | ~$1.1 Billion (Annual Revenue) |
| **[Accedian](https://www.accedian.com/)** | Performance analytics and assurance focused on quality of experience and network visibility. | Custom (Contact Sales) | None | ~$370 Million (Valuation on acquisition by Cisco) |
| **[Cellwize](https://www.cellwize.com/)** (now part of larger portfolios) | RAN automation and analytics platform. | Custom (Contact Sales) | None | ~$350 Million (Valuation on acquisition by Qualcomm) |
| **[EXFO](https://www.exfo.com/)** | Test, monitoring, and analytics portfolio for fiber, 5G, and service assurance. | Custom (Contact Sales) | None | ~$300 Million (Annual Revenue) |
| **[Mobileum](https://www.mobileum.com/)** | Analytics and security platform for roaming, fraud, and network intelligence. | Custom (Contact Sales) | None | ~$300 Million (Annual Revenue) |
| **[Infovista](https://www.infovista.com/)** | Network performance management, planning, and analytics for mobile operators. | Custom (Contact Sales) | None | ~$200 Million (Annual Revenue) |
| **[Subex](https://www.subex.com/)** | Revenue assurance, fraud management, and network analytics solutions for telecom operators. | Custom (Contact Sales) | None | ~$34 Million (Annual Revenue) |
| **[Matellio Telecom Analytics](https://www.matellio.com/)** | Custom and productized analytics solutions for 5G networks. | Custom (Contact Sales) | None | ~$15 Million (Annual Revenue) |


## 🔓 Open-Source Software

### 5G Core / RAN Stacks with Analytics Capabilities
- **[Open5GS](https://github.com/open5gs/open5gs)** [![Stars](https://img.shields.io/github/stars/open5gs/open5gs?style=social)](https://github.com/open5gs/open5gs/stargazers) — Open-source 5G core (and 4G EPC) frequently used in testbeds; can be instrumented for performance monitoring and analytics.
- **[Free5GC](https://github.com/free5gc/free5gc)** [![Stars](https://img.shields.io/github/stars/free5gc/free5gc?style=social)](https://github.com/free5gc/free5gc/stargazers) — Popular open-source 5G core network implementation. Community and research projects add **NWDAF** (Network Data Analytics Function) support for event-driven analytics, subscription/notification, and predictive insights.
- **[srsRAN](https://github.com/srsran/srsRAN_Project)** [![Stars](https://img.shields.io/github/stars/srsran/srsRAN_Project?style=social)](https://github.com/srsran/srsRAN_Project/stargazers) — Open-source 4G/5G RAN software suite. Useful for generating realistic traffic and KPIs in lab environments.
- **[OpenAirInterface (OAI)](https://openairinterface.org/)** [![Stars](https://img.shields.io/github/stars/openairinterface/openairinterface5g?style=social)](https://github.com/openairinterface/openairinterface5g/stargazers) — Full-stack open-source 5G RAN and core. Widely used for research, with extensions for telemetry, xApps, and analytics.
- Open-source NWDAF implementations — Multiple research and community projects integrate NWDAF with Free5GC, Open5GS, or OAI to provide standardized 5G analytics (event exposure, ML-based insights, closed-loop automation).

### O-RAN & RAN Intelligent Controller (RIC) Monitoring
- **[FlexRIC](https://gitlab.eurecom.fr/mosaic5g/flexric)** [![Stars](https://img.shields.io/gitlab/stars/mosaic5g/flexric?gitlab_url=https%3A%2F%2Fgitlab.eurecom.fr&style=social)](https://gitlab.eurecom.fr/mosaic5g/flexric/-/stargazers) / SD-RAN related projects — Open near-real-time RIC frameworks that enable xApps for RAN monitoring, KPI collection, and analytics.
- **[5G-Spector](https://github.com/5GSEC/5G-Spector)** [![Stars](https://img.shields.io/github/stars/5GSEC/5G-Spector?style=social)](https://github.com/5GSEC/5G-Spector/stargazers) and similar O-RAN xApps — Security and monitoring xApps that extract fine-grained RAN telemetry (e.g., MobiFlow) for analysis and anomaly detection.
- Community O-RAN monitoring stacks that combine E2 interface metrics with Prometheus/Grafana or Zabbix.

### General Observability & Analytics Tooling (Highly Adaptable)
- **[Grafana](https://grafana.com/)** [![Stars](https://img.shields.io/github/stars/grafana/grafana?style=social)](https://github.com/grafana/grafana/stargazers) — De-facto open-source visualization and analytics platform. Widely used to dashboard 5G KPIs, logs, and metrics.
- **[Prometheus](https://prometheus.io/)** [![Stars](https://img.shields.io/github/stars/prometheus/prometheus?style=social)](https://github.com/prometheus/prometheus/stargazers) — De-facto open-source monitoring and alerting toolkit. Widely used to scrape 5G KPIs, logs, and metrics.
- **[OpenTelemetry](https://opentelemetry.io/)** [![Stars](https://img.shields.io/github/stars/open-telemetry/opentelemetry-collector?style=social)](https://github.com/open-telemetry/opentelemetry-collector/stargazers) — Vendor-neutral observability framework for traces, metrics, and logs; increasingly applied to telecom workloads.
- **[MobileInsight](https://github.com/mobileinsight-project)** [![Stars](https://img.shields.io/github/stars/mobileinsight-project/mobileinsight-core?style=social)](https://github.com/mobileinsight-project/mobileinsight-core/stargazers) (and 5G extensions) — UE-side protocol tracing and analytics tool for cellular networks.
- ELK / OpenSearch stack — For log aggregation, search, and analytics of network events and KPIs.

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

