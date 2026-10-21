# DRC Cholera 2026: epidemiological dashboard

Interactive monitoring and reactivation-risk dashboard for cholera in the Democratic Republic of the Congo, 2026.

**Live dashboard:** https://global-wash-cluster.github.io/drc_cholera_2026/

The dashboard has three views:

- **Carte des risques**: health-zone map of transmission status, the combined risk ranking of zones without recent cases (importation from affected zones plus recurrence), incidence, case fatality, Flowminder mobility and GRID3 health facilities.
- **Évolution hebdomadaire**: weekly cases, deaths, transmission status and reporting completeness.
- **Epicurves hebdomadaires**: weekly epidemic curves by province, with an Excel export.

Source data: PNECHOL / Ministère de la Santé RDC weekly cholera list, aggregated by health zone.

## How it is published

The dashboard is a self-contained HTML file rendered from an R (`flexdashboard` + Leaflet) pipeline held in a separate working repo, and published here by a one-command script. The site is served from the `gh-pages` branch, which is rebuilt from scratch and force-pushed on every publish, so it always holds exactly one commit.
