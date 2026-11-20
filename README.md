# SEQ Transit in Motion

Interactive map of public transport passengers in South East Queensland, 2016 to 2026, built by Team Pengen Lulus for DataNova 2026 (problem DN-DS-01).

**Live map:** https://hazjel.github.io/seq-transit-pulse/

## What it shows

- **Passengers** moving from the stop where they board to the stop where they get off, along the route they rode (the 400 busiest stop-to-stop pairs per month and time of day).
- **Route activity**: marks moving along each route line, one per 150 boardings per day on that route. They show how busy a route is, not where vehicles are.
- Twelve months (July 2016 to July 2026, plus April 2020) and the five time-of-day groups in the origin-destination data, with trips per day and the share starting or ending in the Brisbane CBD.
- **Round 2 analysis** (optional layers):
  - *Bus load, weekday afternoon*: bus passengers passing along each segment, weekdays 15:00 to 18:59, May to July 2026, all routes summed, drawn along the route shapes. Built from trips with a recorded tap-off and scaled to all boardings; an average, not a crowding count.
  - *Near frequent service*: for each ABS SA2 area, the share of residents within 400 m (straight line) of a stop with about four departures an hour, 07:00 to 19:00, on Wednesday 25 November 2026.

The passenger and route-activity views use only the Translink origin-destination data; there the GTFS timetable only places stops and draws route lines. The Round 2 layers also use the GTFS timetable (scheduled trips, stop departures and stop order) and ABS data. On-screen speeds are illustrative: the origin-destination data has no travel times.

## Data and licences

| Source | Use | Licence |
|---|---|---|
| State of Queensland (Department of Transport and Main Roads), Translink Origin-Destination Trips | all passenger and boarding figures | CC BY 4.0 (CC BY 3.0 AU for 2016 to 2021) |
| Translink SEQ GTFS | stop locations and route lines; Round 2 layers: scheduled trips, stop departures, stop order | CC BY 4.0 |
| OpenStreetMap contributors | base map, buildings (inner Brisbane with 2016 to 2026 history) | ODbL |
| Microsoft Global ML Building Footprints | buildings where OpenStreetMap has none | ODbL |
| Australian Bureau of Statistics: Regional population 2024-25 (SA2), 2021 Census G01 (SA1), SEIFA 2021 (SA2) | Round 2 access layer | CC BY 4.0 |

Data aggregated and modified by the team. The building tiles in `bld/` and `buildings.json` are derived from OpenStreetMap and Microsoft data and are available under the [Open Database License](https://opendatacommons.org/licenses/odbl/1-0/).

Map rendering: [deck.gl](https://deck.gl) (MIT).
