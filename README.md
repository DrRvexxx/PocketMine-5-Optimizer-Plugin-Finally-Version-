# MyClearLag

A high-performance, automated entity clearing and server optimization plugin for PocketMine-MP (API 5).

## Features

- **Automated Clearing**: Periodically removes ground items, experience orbs, and lingering projectiles.
- **Pre-clear Warnings**: Notifies players before a clearing cycle begins to prevent accidental item loss.
- **Manual Control**: In-game commands allow administrators to trigger purges instantly.
- **Fully Configurable**: Easily toggle what entity types to clear and adjust intervals via `config.yml`.

## Commands & Permissions

| Command | Description | Default | Permission |
|---------|-------------|---------|------------|
| `/clearlag` | Manually clears configured entities | OP | `myclearlag.command` |
| `/cl` | Alias for `/clearlag` | OP | `myclearlag.command` |

## Configuration

The plugin generates a default `config.yml` on its first run:

```yaml
clear_interval: 300       # Time in seconds between automated clears
warning_seconds: 10       # Seconds before the clear to send a warning message
clear_items: true         # Clear dropped items and XP orbs
clear_mobs: false         # Clear living mobs (Disabled by default)
clear_projectiles: true   # Clear arrows, snowballs, etc.
