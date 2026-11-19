### Hi, I'm Anuj 👋

I build data infrastructure for public transit: the feeds, pipelines, and field software that tell a rural bus system where its vehicles are, who is riding, and whether the service is working.

I'm a data scientist by training (M.S. Applied Data Science, Clarkson) and a platform engineer by necessity. Small transit agencies rarely have a data team, so I've ended up owning the whole stack for three of them in northern New York, from GTFS authoring and realtime telemetry through validation, analytics, and publishing to Google Maps.

---

### 🚌 What I'm building — [GTFS Foundry](https://gtfsfoundry.com)

An open-standards operations platform for small and rural transit agencies, now in field pilot.

| | |
|---|---|
| **Control Tower** | Multi-tenant GTFS / GTFS-Flex authoring, validation-gated publishing, GTFS-Realtime feeds, live dispatch, and feed-health monitoring for agencies whose data comes from a third-party vendor. |
| **Foundry Pilot** | Offline-first Android driver app for passenger counting, flag-stop and detour capture, and realtime vehicle position and occupancy. |
| **Validation suite** | Continuous feed QA built on the MobilityData canonical validator. |

`React` `TypeScript` `Directus` `PostgreSQL` `Redis` `Python` `Docker` `AWS` `Capacitor` `Prometheus` `Grafana`

<sub>Production source is private. I'm glad to walk through the architecture.</sub>

---

### 🧭 How I approach the work

- **Data quality is a release gate.** A feed that fails validation doesn't ship. Riders find the bugs we let through.
- **Field software has to work offline.** Rural routes lose signal, so devices queue locally, sync in batches, and sign every request.
- **Right-size the infrastructure.** Serverless and event-driven where the load is spiky, one well-run box where it isn't. Public agencies pay for every idle server.
- **Analysis should end in a decision.** Service-planning work here ends in a specific call on each trip: cut, consolidate, retime, or protect.

---

### 📂 Public work

| Project | What it shows |
|---|---|
| [**SLC-Transit-GTFS-RT-Validator**](https://github.com/anujpatil610/SLC-Transit-GTFS-RT-Validator) | Production realtime-feed monitoring: Terraform, Docker, service-hour scheduling, alerting on critical errors |
| [**NYC crash & pavement analysis**](https://github.com/anujpatil610/Analysis-of-Car-Crash-Data-and-Pavement-Ratings-in-New-York-City) | Spatial join of crash records to road segments to find road-safety risk patterns |
| [**Climate risk & emissions**](https://github.com/anujpatil610/Climate-Change-Risk-and-Opportunity-Analysis) | Emissions-risk prediction over 10M+ audit records across four regions |
| [**Booking cancellation model**](https://github.com/anujpatil610/Predictive-Analysis-and-Key-Determinants-of-Hotel-Booking-Cancellations) | Gradient boosting with explainability (feature importance and partial dependence) |

---

### 🎤 Talks

**MobilityData Conference, Montréal 2024**: building a realtime transit data archive for a small agency

---

### 🛠 Toolbox

**Transit & geo** · GTFS (Static, Realtime, Flex) · PostGIS · ArcGIS Pro/Online · QGIS · GeoPandas · GDAL · H3 · Mapbox GL<br>
**Data & ML** · Python · SQL · R · scikit-learn · CatBoost · TensorFlow · Snowflake · Redshift<br>
**Platform** · AWS (Lambda, EC2, S3, SNS) · Terraform · Docker · GitHub Actions · Cloudflare · TypeScript · React · Node.js

---

[arpatil.xyz](https://arpatil.xyz) · [LinkedIn](https://www.linkedin.com/in/anujrpatil) · [anuj.patil4435@gmail.com](mailto:anuj.patil4435@gmail.com)
