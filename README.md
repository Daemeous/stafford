# Stafford — OS Open Roads comparison

A static, read-only map comparing Stafford's OSM-derived road data (the
same pipeline behind the [live Stafford leafletting tracker](https://daemeous.github.io/leaflet-map/))
against Ordnance Survey's **OS Open Roads** dataset, for the same 17
wards. Not a tracker — no editing, no Google Sheet backend, no residence
counts.

Three view modes (top of the sidebar):

- **Compare** — overlays both datasets and highlights the differences:
  roads OS Open Roads has that OSM is missing entirely ("new"), stretches
  where the two only partially overlap ("diverges" — just the
  non-overlapping part is highlighted), and OSM's own previously-unnamed
  road clusters split into ones a nearby OS Open Roads match could name
  ("renamed") vs ones neither dataset names ("unknown"). Matching/unchanged
  stretches are hidden by default (toggle to show) so the differences are
  what stands out.
- **OSM** — OSM's own road network, coloured by whether it was already
  named, auto-named via an OS Open Roads match, or still unnamed.
- **OS Open Roads** — coloured by how the road is identified: a real
  street name, a route number only (A/B roads), or neither. Motorways and
  slip roads are excluded from the diff entirely (no pedestrian frontage).

A stats panel and click-for-details popup are available in every mode, plus
a ward quick-jump dropdown.

See [leaflet-pipeline](https://github.com/Daemeous/leaflet-pipeline) for
the data pipeline this compares against.

## License

This project's own code is licensed under the
**[PolyForm Noncommercial License 1.0.0](LICENSE)**: free to use, share,
and modify for any non-commercial purpose, with attribution. See
[`LICENSE`](LICENSE) for the full text.

Copyright © Daniel Hodgkins.

That covers this project's own code only. The geographic data it displays
comes from sources under their own separate licenses that explicitly
permit commercial use (see Attributions below) — this project's
non-commercial restriction doesn't, and legally can't, extend to that
underlying data.

## Attributions

| Dependency | License | Notes |
|---|---|---|
| [Leaflet.js](https://leafletjs.com) | BSD-2-Clause | © Vladimir Agafonkin and contributors |
| [OpenStreetMap](https://www.openstreetmap.org/copyright) | [ODbL](https://opendatacommons.org/licenses/odbl/) | Map tiles only. © OpenStreetMap contributors. |
| OS Open Roads | [Open Government Licence v3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/) | © Crown copyright and database right, Ordnance Survey. Permits commercial use; requires attribution. |
