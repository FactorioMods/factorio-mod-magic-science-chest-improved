# Magic Science Chest: Improved

A fork of [Magic Science Chest](https://mods.factorio.com/mod/magic-science-chest) by Dreaden for Factorio 2.0 and Space Age.

Adds a free passive-provider chest that supplies science packs once your force has produced enough of each pack (100 by default). Each unlocked pack keeps a one-stack buffer. This is a cheat mod.

## Changes

- Compare chest filters without temporary flattened tables and update only chests of affected forces.
- Share production calculations between open windows on the same force and avoid rewriting unchanged GUI captions.
- Refresh science caches and GUI rows when science pack keys change.
- Skip production-statistics reads when the unlock threshold is zero.
- Rediscover existing chests when replacing the original mod and restore native refill when upgrading from batched fork releases.

Uses the original continuous native refill and five-second unlock check. These changes target periodic filter checks and GUI work.

## Endgame validation

Compared with the original 2.0.2 mod on Factorio 2.0.77 using an endgame save with 2,509 science chests and 5,011 biolabs. Both completed research-productivity level 49 after 2,306 ticks, starting at 64.68% progress. Each consumed 2,771,479 science packs across all types over 3,000 ticks; the remaining ticks after completion were idle.

Controlled research pause/restart checks also matched: about 71,707 combined packs per game-second before pausing, zero while paused, and 72,873 after restarting. Overall update timings overlapped between runs.

## Installation

Disable the original Magic Science Chest and enable this fork. Existing chest, item, recipe and original setting identifiers are retained. Multiplayer clients must use the same mod version as the host.

## Credits

Original code and artwork by Dreaden. Fork maintained by johnmart19 under the original MIT-0 license.

[Original source](https://github.com/bengardner/factorio-mod-magic-science-chest) | [Fork source](https://github.com/FactorioMods/factorio-mod-magic-science-chest-improved)
