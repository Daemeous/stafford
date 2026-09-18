# Stafford — OS Open Roads comparison

A static, read-only map of Stafford's roads sourced from Ordnance Survey's
**OS Open Roads** dataset, built to visually compare against the
OSM-derived [live Stafford leafletting tracker](https://daemeous.github.io/leaflet-map/).

This is not a tracker — no editing, no Google Sheet backend, no residence
counts. It exists purely to eyeball how OS Open Roads' road coverage and
naming compares to the OSM-based pipeline for the same 17 wards.

Roads are colour-coded:

- **Blue** — has a real street name in OS Open Roads (`name_1`)
- **Amber** — no street name, but has a classified route number (A/B roads,
  motorways) used as a fallback label
- **Red** — neither a name nor a route number in this dataset

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
