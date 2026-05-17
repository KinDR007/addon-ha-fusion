# Fusion+

A friendlier, feature-rich Fusion dashboard for Home Assistant.

Source: <https://github.com/KinDR007/ha-fusion>
Upstream: <https://github.com/matt8707/ha-fusion>

[![Open your Home Assistant instance and show the add add-on repository dialog with a specific repository URL pre-filled.](https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg)](https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2FKinDR007%2Faddon-ha-fusion)

This fork adds:

- New item types: `power_button`, `victron_button`, `grid_button`,
  `info_grid`, `flex_grid`, `temp_humi_button`
- Per-cell Jinja templates + tabbed editor for grid components
- `SensorDetailsModal` — rich read-only modal with grouped attributes,
  related siblings (temperature ↔ humidity ↔ pressure) and a 24h history
  graph for numeric sensors
- `LightModal` chroma-only fix (RGB picker now appears for lights without
  the COLOR capability flag)
- Date-based versioning (`YYYY.M.N`)

See [CHANGELOG.md](CHANGELOG.md) for the full release history.
