# Row One aircraft table

The aircraft registration database bundled with the [Row One](https://www.milivon.com) iPhone app,
published under the [Open Database License (ODbL) 1.0](https://opendatacommons.org/licenses/odbl/1-0/).

Row One uses it offline to identify an aircraft from its registration (for example `D-AIXP` → Airbus A340-600).

## Contents

`aircraft.csv`: 87,860 aircraft, one per registration, sorted by registration.

| Column | Meaning |
|---|---|
| `reg` | Registration (tail number) |
| `icao24` | 24-bit ICAO transponder address (hex) |
| `type` | ICAO aircraft type designator, e.g. `A346` |
| `description` | Model description |
| `operator` | Operator, where known |
| `year_built` | Year built, where known |
| `serial` | Manufacturer serial number (MSN), where known |
| `source` | Where the row's values come from, comma-separated: `adsblol`, `vrs` and/or `faa` |

Built 2026-10-17; FAA details added 2026-11-20.

## Sources

- **[adsb.lol globe_history](https://github.com/adsblol)**: aircraft metadata from the ADS-B trace dumps,
  © adsb.lol contributors, ODbL 1.0.
- **[Virtual Radar Server standing data](https://github.com/vradarserver/standing-data)**: CC0 1.0 (public domain).
- **[FAA Aircraft Registry](https://www.faa.gov/licenses_certificates/aircraft_certification/aircraft_registry/releasable_aircraft_download)**:
  model, serial number and year built for US N-registrations, US government work (public domain).
  Owner names and addresses are not included.

They were merged and filtered (airliners and other aircraft with a registration) by Row One's build scripts.
Because the result is derived from an ODbL database, it is offered here under the same license.

## License

This Row One aircraft table is made available under the Open Database License:
https://opendatacommons.org/licenses/odbl/1-0/. Any rights in individual contents of the database are
licensed under the Database Contents License: https://opendatacommons.org/licenses/dbcl/1-0/.

See [LICENSE](LICENSE). Contact: support@milivon.com.
