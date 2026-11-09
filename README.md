# SEQ Transit in Motion

Interactive map of public transport passengers in South East Queensland, 2016 to 2026, built by Team Pengen Lulus for DataNova 2026 (problem DN-DS-01).

**Live map:** https://hazjel.github.io/seq-transit-pulse/

## What it shows

- **Passengers** moving from the stop where they board to the stop where they get off, along the route they rode (the 400 busiest stop-to-stop pairs per month and time of day).
- **Route activity**: marks moving along each route line, one per 150 boardings per day on that route. They show how busy a route is, not where vehicles are.
- Twelve months (July 2016 to July 2026, plus April 2020) and the five time-of-day groups in the origin-destination data, with trips per day and the share starting or ending in the Brisbane CBD.

Every number comes from the Translink origin-destination data. The Translink GTFS timetable is used only to place stops and draw route lines. On-screen speeds are illustrative: the origin-destination data has no travel times.

## Data and licences

| Source | Use | Licence |
|---|---|---|
| State of Queensland (Department of Transport and Main Roads), Translink Origin-Destination Trips | all passenger and boarding figures | CC BY 4.0 (CC BY 3.0 AU for 2016 to 2021) |
| Translink SEQ GTFS | stop locations and route lines | CC BY 4.0 |
| OpenStreetMap contributors | base map, buildings (inner Brisbane with 2016 to 2026 history) | ODbL |
| Microsoft Global ML Building Footprints | buildings where OpenStreetMap has none | ODbL |

Data aggregated and modified by the team. The building tiles in `bld/` and `buildings.json` are derived from OpenStreetMap and Microsoft data and are available under the [Open Database License](https://opendatacommons.org/licenses/odbl/1-0/).

Map rendering: [deck.gl](https://deck.gl) (MIT).
