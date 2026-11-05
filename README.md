# Magic Science Chest: Improved

A free passive-provider chest supplies science packs after your force has produced enough of each pack.

**Factorio 2.1 · Version 1.0.2**

## Fork changes

- Corrects science-pack filters and refreshes the progress window when the available pack list changes.
- Caches science-pack discovery and avoids rewriting unchanged chest filters or rebuilding identical progress views.
- Rediscovers existing chests when switching from the original mod and refreshes their filters after configuration changes.
- Restores native refill for saves affected by an earlier fork release that left chests disabled.
- Updates production-statistics access, prototype fields and GUI handling for Factorio 2.1.

Science still comes from the original native refill mechanism. The production threshold defaults to 100 of each pack; unlocked packs are supplied as full stacks. Each pack unlocks independently when its own threshold is reached.

## Installation

Requires Factorio 2.1.23+. Disable `magic-science-chest` before enabling this fork. Existing chest names are retained, so the fork can rediscover them. Space Age is optional.

Original code and artwork by Dreaden; [original source](https://github.com/bengardner/factorio-mod-magic-science-chest) by Ben Gardner. Maintained by johnmart19 under [MIT-0](license.txt).

[Mod Portal](https://mods.factorio.com/mod/magic-science-chest-optimized) · [Source](https://github.com/FactorioMods/factorio-mod-magic-science-chest-improved) · [Downloads](https://github.com/FactorioMods/factorio-mod-magic-science-chest-improved/releases) · [Changes and tests](FACTORIO-2.1.md)
