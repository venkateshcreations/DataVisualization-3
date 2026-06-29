# GEC — Global Supply Chain Analytics Dashboard

A portfolio-grade, single-page data visualization dashboard for **Global Electronics Corporation (GEC)**, built entirely with **D3.js v7**. Features 12 interactive sections covering the end-to-end supply chain from raw materials to retail.

## Live Demo

Open `index.html` in a browser (requires internet for D3.js CDN and world map topology data).

## Visualizations

| Section | Chart Type | Description |
|---|---|---|
| **Overview** | KPIs, Bar, Scatter | High-level metrics and performance snapshots |
| **Sankey Flow** | Sankey Diagram | Material flow from suppliers → manufacturing → distribution → warehouses → retail |
| **Network** | Force-Directed Graph | Interactive supply chain relationship topology with drag, zoom, pan |
| **Hierarchy** | Zoomable Sunburst | Hierarchical breakdown of the supply chain structure |
| **World Map** | Geo Map with Animated Arcs | Geographic shipment flows between global hubs with animated cargo dots |
| **Shipments** | Bar, Bubble, Horizontal Bar | Route performance: volume, cost vs CO₂, transit days |
| **Warehouses** | Gauges, Horizontal Bar | Real-time utilization gauges and inventory vs capacity |
| **Routes** | Bubble, Risk Bars, Table | Logistics corridor analysis with cost, distance, risk scoring |
| **Sustainability** | Stacked Area Chart | Monthly CO₂ emissions by stage (Raw Material, Manufacturing, Transport) |
| **Suppliers** | Radar Chart | Multi-dimension supplier QA scores (quality, speed, cost, compliance, reliability) |
| **Incidents** | Table + Alert Ticker | Live disruption monitoring with severity-coded status badges |
| **Forecasting** | Line Chart with Confidence Bands | Historical sales vs ML-predicted demand with 95% confidence intervals |

## Interactive Features

- **Tab Navigation** — 12-section lazy-loaded interface with smooth scrolling
- **Dark/Light Theme** — Toggle between dark and light mode
- **Global Search** — Filter nodes across Sankey, Network, and Sunburst charts
- **SVG Export** — Download any chart as SVG
- **CSV Export** — Export section data as CSV
- **Interactive Tooltips** — Hover details on all charts
- **Animated Transitions** — Chart entrance animations and cargo flow animation on the world map
- **Zoom & Pan** — Force-directed network supports zoom/pan/drag

## Data

All datasets are embedded as JSON within `index.html` and also available as standalone JSON files:

- `Sankey Flow Dataset.json`
- `Force Directed Network Dataset.json`
- `Supply Chain Hierarchy Dataset - Tree Chart - OR - Sunburst Chart.json`
- `Geographic Flow Map Dataset.json`
- `Shipment Analytics Dataset.json`
- `Inventory Dataset -Warehouse Dashboard.json`
- `Route Optimization Dataset.json`
- `Sustainability Metrics.json`
- `Supplier QA Dataset.json`
- `Active Incidents.json`
- `Demand Forecast.json`

## Tech Stack

- **D3.js v7** — All chart rendering
- **d3-sankey** — Sankey diagram layout
- **TopoJSON** — World map topology
- **Inter** — Typeface (Google Fonts)
- Pure vanilla JavaScript — No frameworks, no build step

## Supply Chain Storyline

```
Raw Materials (12 Countries)
        ↓
Manufacturing Plants (4 Countries)
        ↓
Distribution Centers (4 Continents)
        ↓
Regional Warehouses
        ↓
Retail Networks
        ↓
Customers
```

## Usage

1. Clone or download the repository
2. Open `index.html` in any modern browser
3. Navigate sections using the sticky tab bar at the top
4. Use the theme toggle (🌞/🌙) to switch light/dark mode

No build tools or server required.
