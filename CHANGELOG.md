# Fusion (KinDR007 fork)

Date-based versioning: `YYYY.M.N` where `N` is the sequential commit
number in that month.

## 2026.5.13
- **SensorDetailsModal**: rich read-only modal for `sensor.*` and
  `binary_sensor.*` clicks (temperature, humidity, water-leak, door/window, …)
  - Hero state line with device-class icon + unit
  - Friendly labels for binary sensors (open/closed, wet/dry, detected/clear)
  - Related siblings on the same device (temp ↔ humi ↔ pressure ↔ dewpoint)
  - Device info: battery, RSSI, linkquality, voltage, last_seen
  - 24h history graph (numeric sensors, via `recorder/statistics_during_period`)
  - Collapsible attributes dump

## 2026.5.12
- Repoint upstream UI references (Version check, "open issue", Map docs)
  from `matt8707/ha-fusion` to `KinDR007/ha-fusion`
- Align `package.json` version with addon image tag

## 2026.5.11
- `temp_humi_button`: Jinja templates for state/color/name/icon
  (same pattern as classic Button); drop `RH` suffix from auto state-line
  → format is now `21.5 °C / 55 %`
- Switch to date-based versioning

## 2024.10.6 (KinDR007 fork)
- New `temp_humi_button` item type: dedicated tile for temperature +
  humidity sensor pairs (auto-discovered via `_temperature` / `_humidity`
  suffix swap)

## 2024.10.5 (KinDR007 fork)
- `grid_button` / `info_grid` / `flex_grid`: per-cell Jinja templates
  + tabbed editor (dimensions / cells)
- `LightModal`: chroma-only fix — RGB picker now shows for lights that
  advertise color modes without `COLOR` capability

## 2024.10.4 (KinDR007 fork)
- New item types: `grid_button` (1×2 footprint, inner 2×3 cells),
  `info_grid` (read-only stat panel), `flex_grid` (dynamic span/inner grid)

## 2024.10.3 (KinDR007 fork)
- New `victron_button` item type: hybrid layout for Victron MQTT entities
  with device filtering and shortcode-based metric grouping (MPPT/BMS/INV/GX)

## 2024.10.2 (KinDR007 fork)
- New `power_button` item type: auto state/color derived from a
  companion `sensor.<base>_power` entity

## 2024.10.1 (KinDR007 fork)
- Fork of upstream `matt8707/ha-fusion`; CI build pushes images to GHCR
- amd64-only target

---

Upstream changelog (reference):
https://github.com/matt8707/ha-fusion/releases
