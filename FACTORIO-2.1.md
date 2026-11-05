# Factorio 2.1 notes

Version **1.0.2** uses `disabled_by_script` for legacy refill restoration and removes obsolete prototype and GUI fields.

## Factorio 2.1.24 headless checks

Powered assemblers produced automation and logistic science packs. Each pack became available independently after its production threshold was reached; the chest did not refill it early. Native refill supplied 200 packs and replaced 50 removed packs. This check used a threshold of one to exercise the production gate.

## Earlier Factorio 2.1.23 host/client checks

Production thresholds, pack filters and native refill passed with a connected client. Chest state survived save, restart and rejoin.

Coverage uses the installed science-pack set; overhaul mods may introduce additional progression rules.
