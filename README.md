🌍 AQI Monitor — Global Air Quality Dashboard
An interactive, real-time Air Quality Index (AQI) dashboard built with vanilla HTML, CSS, and Chart.js. Tracks and visualizes air quality data across 7 major world cities with live-updating charts and health advisories.

📸 Features

7 City Profiles — Mumbai, Delhi, London, New York, Beijing, Sydney, Tokyo
Live Data Simulation — values update every 8 seconds with realistic jitter
Color-coded AQI Severity — from Good (green) through Hazardous (purple)
Health Advisories — context-aware recommendations per AQI level
Fully Responsive — adapts to desktop, tablet, and mobile screens


📊 Charts & Visualizations
ChartTypeDescription24-Hour TrendLineAQI over the past 24 hours with gradient fillPollutant RadarRadarRelative concentration of 6 pollutantsCity ComparisonBarSide-by-side AQI across all 7 cities7-Day HistoryBarDaily AQI for the past week

🧪 Pollutants Tracked

PM2.5 — Fine particulate matter (µg/m³)
PM10 — Coarse particulate matter (µg/m³)
NO₂ — Nitrogen Dioxide (µg/m³)
O₃ — Ground-level Ozone (µg/m³)
CO — Carbon Monoxide (mg/m³)
SO₂ — Sulfur Dioxide (µg/m³)


🎨 AQI Scale Reference
AQI RangeCategoryColor0–50Good🟢 Green51–100Moderate🟡 Yellow101–150Unhealthy for Sensitive Groups🟠 Orange151–200Unhealthy🔴 Red201–300Very Unhealthy🟣 Purple301–500Hazardous☠️ Dark Purple

🚀 Getting Started
No build tools or dependencies required. Just open the file in a browser.
bash# Clone or download the project
git clone https://github.com/your-username/aqi-dashboard.git

# Open directly in your browser
open air-quality-dashboard.html
Or simply drag and drop air-quality-dashboard.html into any modern browser.

🛠 Tech Stack

HTML5 / CSS3 / Vanilla JS — zero framework dependencies
Chart.js v4.4.1 — all charts and graphs
Google Fonts — Share Tech Mono, Barlow Condensed
CSS Custom Properties — theming and color system
CSS Animations — scanline overlay, pulse indicators, staggered fade-ins


📁 File Structure
aqi-dashboard/
└── air-quality-dashboard.html   # Single self-contained file
└── README.md

🔧 Customization
All city data is defined in the CITIES object near the top of the <script> block. To add a new city or change values:
jsconst CITIES = {
  'Your City': {
    aqi: 85,
    pollutants: { PM2_5: 28.0, PM10: 52.0, NO2: 35.0, O3: 48.0, CO: 0.8, SO2: 10.0 },
    trend24h: [ /* 24 hourly AQI values */ ],
    week:     [ /* 7 daily AQI values */ ]
  },
  // ...
};
To connect real data, replace the static CITIES object with an API call to a provider such as IQAir, OpenAQ, or WAQI.
