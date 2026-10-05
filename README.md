

Readme · MD
# Diani Beach → Tsavo East, Amboseli & Tsavo West: 4-Day Safari Route Map
 
This is an interactive 3D map of a 4-day road safari from **Diani Beach** on Kenya's south coast. The trip visits three of southern Kenya's best-known parks: **Tsavo East**, **Amboseli** (at the foot of Kilimanjaro) and **Tsavo West**.
 
🗺️ **See the full itinerary and the live map:**
[Cztery dni zwiedzania Tsavo Wschód i Tsavo Zachód](https://safarikenia.com.pl/cztery-dni-zwiedzania-tsavo-wschod-i-tsavo-zachod/) on **Safari Kenia**
 
---
 
## The route
 
| Stop | Park | Accommodation |
|------|------|---------------|
| Start | Diani Beach | — |
| Day 1 | Tsavo East National Park | Voi Safari Lodge |
| Day 2 | Amboseli National Park | Amboseli Sopa Lodge |
| Day 3 | Tsavo West National Park | Ngulia Safari Lodge |
| Day 4 | Return to Diani Beach | — |
 
**Outbound:** Diani Beach → Likoni Ferry → Mariakani → Taru junction → Buchuma → Voi (Tsavo East)
**Through the parks:** Voi → Amboseli → past the Chyulu Hills → Ngulia (Tsavo West)
**Return:** Tsavo West → Mariakani → Likoni Ferry → Diani Beach
 
The interface labels are in Polish, matching the tour page it's embedded on.
 
## Features
 
- **Satellite basemap with 3D terrain.** The map uses the Mapbox Standard Satellite style with DEM terrain (1.5× exaggeration) and a tilted camera. This brings out the Ngulia Hills, the Chyulu Hills and the plains around Amboseli.
- **Road-accurate route.** Each leg is fetched from the Mapbox Directions API (driving profile) and stitched into one continuous line. If a request fails, the map falls back to a straight segment.
- **Animated route line.** The route is drawn as a golden "marching ants" dashed line over a soft glow layer.
- **Interactive itinerary panel.** A glassmorphism sidebar lists each day. Clicking a card flies the camera to that lodge and opens its popup.
- **Custom markers.** Gold SVG pins mark each overnight stop. Hidden waypoints keep the route on the correct roads.
- **Mobile-friendly.** On small screens the sidebar becomes a bottom sheet, and cooperative gestures keep page scrolling smooth.
- **WordPress-ready.** Styles are scoped to a single container, so the code can be pasted into a Custom HTML block.
## Tech stack
 
- [Mapbox GL JS](https://docs.mapbox.com/mapbox-gl-js/) v3.9.0
- [Mapbox Directions API](https://docs.mapbox.com/api/navigation/directions/)
- Vanilla JavaScript, with no build step
- Plus Jakarta Sans (Google Fonts)
## Usage
 
1. Copy the HTML into a WordPress **Custom HTML** block or any web page.
2. Replace the Mapbox access token with your own, and restrict it to your domain in your [Mapbox account](https://account.mapbox.com/access-tokens/).
3. Adjust the container height in `.wp-safari-itinerary-container` to fit your layout.
To change the route, edit the `itineraryData` array. Entries with `isWaypoint: true` shape the route only. All other entries get a marker and a sidebar card.
 
## About
 
Built for [Safari Kenia](https://safarikenia.com.pl/), which offers Polish-language safari tours and travel guides for Kenya.
 
➡️ [View this 4-day safari itinerary](https://safarikenia.com.pl/cztery-dni-zwiedzania-tsavo-wschod-i-tsavo-zachod/)
 
