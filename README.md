# Anuj R. Patil

**Senior Data Scientist — Transit Data Platforms · Geospatial Analytics · Machine Learning**

I design and operate the data infrastructure behind public transit: GTFS and GTFS-Realtime feeds, fleet telemetry, service analytics, and the maps and dashboards that turn them into operating decisions. At the Volunteer Transportation Center I own the transit data platform for three public agencies across five counties in northern New York. That covers ingestion, validation, modeling, and publishing to riders, planners, and partners such as Google Maps and Transit.

M.S. Applied Data Science, Clarkson University · B.E. Computer Engineering, Savitribai Phule Pune University · Speaker, MobilityData Conference, Montréal 2024

🌐 **[arpatil.xyz](https://arpatil.xyz)** · 🚌 **[gtfsfoundry.com](https://gtfsfoundry.com)** · 📍 Potsdam, NY

---

### Platform architecture — the Foundry product family

A closed-loop transit operations platform I architected and built end to end, now in field pilot with agency operations.

- **GTFS Control Tower** — multi-tenant SaaS for authoring, validating, and publishing GTFS Static, Realtime, and Flex. Tenant data isolation, role-based access control with capability gates, a release pipeline gated on validation quality, protobuf GTFS-RT publishing, live dispatch, and a third-party feed-monitoring tier. Stack: React/TypeScript, Directus, PostgreSQL, Redis, Python workers, Docker on AWS, and Prometheus/Grafana for observability.
- **Foundry Pilot** — offline-first Android/PWA driver application for automated passenger counting, flag-stop and detour logging, and realtime vehicle position and occupancy. Durable local queuing with batched sync, HMAC-signed device authentication, and kiosk-mode device management.
- **GTFS Foundry** — feed validation and data quality suite built on the MobilityData canonical validator.

### Transit data engineering

- **Production GTFS publishing and Google Maps onboarding** — led the technical side of the Jefferson County Public Transit launch, from feed authoring through Google Transit quality review and the GTFS-Realtime launch with the AVL vendor. Also integrated with the Transit app.
- **Serverless realtime archive** — event-driven AWS Lambda + S3 data lake retaining GTFS-RT history. It is the foundation for on-time performance and service reliability analytics, built to run at minimal operating cost.
- **Telemetry processing at scale** — GPS stop-arrival and dwell-time pipelines with parallelized Lambda workers, plus automated detour detection with SNS alerting.
- **Feed reliability monitoring** — infrastructure-as-code (Terraform) and containerized validation, scheduled to service hours, with alerting on critical errors and historical reporting. The monitored network serves a 28-bus fleet that has carried about 1M passengers during my tenure. → [SLC-Transit-GTFS-RT-Validator](https://github.com/anujpatil610/SLC-Transit-GTFS-RT-Validator)
- **Public data delivery** — CDN-hardened feed hosting (Cloudflare) and automated GTFS-to-ArcGIS Online refresh for public maps and Experience Builder apps.

### Analytics, modeling & applied AI

- **Service planning decision support** — self-serve dashboard with trip-level decision scoring (cut, consolidate, retime, protect), route diagnostics across APC, load, dwell, and deviation, and coverage-gap and flag-stop clustering.
- **Network and microtransit design** — origin-destination and first/last-mile analysis to co-design zone-based microtransit and align fixed-route, Flex, and on-demand service.
- **Applied ML for transportation** — physics-informed and hybrid models for routing, arrival prediction, and collision risk; LLM-driven synthetic data generation where real data is sparse.
- **Agency collaboration** — work with NYSDOT and federal partners (FHWA, USDOT) on applied AI initiatives and multi-agency technical working groups.

### Selected research & projects

- **Road safety risk modeling** — unified crash, traffic, roadway geometry, and weather data into a segment-level composite risk score that prioritizes the top 5% of segments for engineering review. → [NYC crash & pavement analysis](https://github.com/anujpatil610/Analysis-of-Car-Crash-Data-and-Pavement-Ratings-in-New-York-City)
- **Wildlife–vehicle collision hotspots (A2A corridor)** — kernel-density screening and penalized regression over 1,000+ collision records, producing mitigation layers delivered to three counties.
- **Predictive modeling of booking cancellations** — gradient-boosted classifier (CatBoost, 88.3% accuracy) with model explainability through feature importance and partial dependence. → [repo](https://github.com/anujpatil610/Predictive-Analysis-and-Key-Determinants-of-Hotel-Booking-Cancellations)
- **Climate risk analytics** — emissions risk prediction over 10M+ environmental audit records across the US, EU, Canada, and India. → [repo](https://github.com/anujpatil610/Climate-Change-Risk-and-Opportunity-Analysis)

---

### Stack

**Transit & geospatial**<br>
![GTFS](https://img.shields.io/badge/GTFS-Static%20%7C%20RT%20%7C%20Flex-2EA44F?style=flat-square)
![PostGIS](https://img.shields.io/badge/PostGIS-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![ArcGIS](https://img.shields.io/badge/ArcGIS%20Pro%20%2F%20Online-2C7AC3?style=flat-square)
![ArcPy](https://img.shields.io/badge/ArcPy-2C7AC3?style=flat-square)
![QGIS](https://img.shields.io/badge/QGIS-589632?style=flat-square&logo=qgis&logoColor=white)
![GeoPandas](https://img.shields.io/badge/GeoPandas-139C5A?style=flat-square&logo=geopandas&logoColor=white)
![GDAL](https://img.shields.io/badge/GDAL-5CAE58?style=flat-square)
![H3](https://img.shields.io/badge/H3-1E54B7?style=flat-square)
![Mapbox](https://img.shields.io/badge/Mapbox%20GL-000000?style=flat-square&logo=mapbox&logoColor=white)

**ML & modeling**<br>
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![CatBoost](https://img.shields.io/badge/CatBoost-FFCC00?style=flat-square&logoColor=black)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=flat-square&logo=keras&logoColor=white)
![Statistical modeling](https://img.shields.io/badge/Statistical%20modeling-8E44AD?style=flat-square)

**Data & cloud**<br>
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-336791?style=flat-square)
![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-Lambda%20%7C%20EC2%20%7C%20S3%20%7C%20SNS%20%7C%20Redshift-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white)

**Application platform**<br>
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Directus](https://img.shields.io/badge/Directus-263238?style=flat-square&logo=directus&logoColor=white)
![Capacitor](https://img.shields.io/badge/Capacitor-119EFF?style=flat-square&logo=capacitor&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)

---

### Connect

Open to conversations about transit data, geospatial platforms, and applied ML in mobility.

[Portfolio](https://arpatil.xyz) · [GTFS Foundry](https://gtfsfoundry.com) · [Email](mailto:anuj.patil4435@gmail.com) · [LinkedIn](https://www.linkedin.com/in/anujrpatil)
