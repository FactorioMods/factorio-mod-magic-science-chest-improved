# Factorio 2.1 notes

Tested with **Factorio 2.1.23**. Current fork version: **1.0.2**.

## Changes

- Use disabled_by_script for the legacy refill-disable path.
- Removed ignored prototype and GUI fields.

## Tests

- Production thresholds unlocked the intended science packs without unlocking unrelated packs.
- Native refill restored removed packs to the configured supply.
- Filters, refill and saved state passed connected-client tests and restart/rejoin.

The tests use the installed science-pack set and settings; they are not a benchmark of every overhaul.

Tests used private copies of saves and local host/client sessions. Raw player data and test hooks are not shipped.
