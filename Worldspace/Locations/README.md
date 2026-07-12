# Locations

This repo does not duplicate Tepenia's deep city/district-level geography and culture — that lives in InnerTepeniaGDD's own "Megasheet" system, which is large (~60 final compiled documents, ~1.75MB) and still actively evolving. Duplicating it here would both bloat this repo and go stale every time InnerTepeniaGDD's own city work moves on. This file is a map to that system, not a cache of its contents — read the source directly (local clone or `raw.githubusercontent.com/TerranLights/InnerTepeniaGDD/main/...`) when location detail is needed.

## The Megasheet hierarchy

Each tier is a synthesis of the tier below it — cities roll up into subnets, subnets and Concordia's districts roll up into the whole game:

1. **City Megasheets** (`Worldspace/Locations-and-Levels/Outside-World/Tepenian-Federation/Locations/Cities/City_Megasheets/<Subnet>/<City>/`) — each of Tepenia's 35 cities gets a `README.md` compiled from three staged documents: `<City>_Mega_Init.md` (synthesis of the city's raw inputs), `<City>_Full_Extrapolation.md` (invented answers to open questions, clearly marked as proposed), `<City>_Cross_Reference_Synthesis.md` (implications that only emerge from combining multiple sources). The three staged files stay in the folder alongside the compiled `README.md`. Some city folders also carry DLC-specific scaffolding files (`<City>_DLC_*.md`) — those are CRPG-exclusive, not general lore.
2. **Concordia's District Megasheets** (`Worldspace/Locations-and-Levels/Concordia-City/Districts/District_Megasheets/<01-13>_<District>/`) — same three-stage process, one per district (12 zodiac-named + neutral Hub/Axis Mundi). See `Reference/World_History_Reference.md` and this repo's own Timeline Eras for the subset of dated district events already migrated here.
3. **Subnet Ultra-Megasheets** (`.../City_Megasheets/<Subnet>/<Subnet>_Subnet_Ultra_Megasheet/`) — one per subnet, synthesizing that subnet's own cities. Byrd is a single-city subnet, so its own City Megasheet stands in for a Subnet Ultra-Megasheet.
4. **Concordia Ultra-Megasheet** (`Worldspace/Locations-and-Levels/Concordia-City/Districts/Concordia_Ultra_Megasheet/`) — synthesizes all 13 districts.
5. **Super-Ultra-Megasheet** (`Worldspace/Locations-and-Levels/Super_Ultra_Megasheet/`) — the whole game-world treated as one subject: all 5 Subnet Ultra-Megasheets, Byrd, Concordia's Ultra-Megasheet, Amundsen Station, and nationwide census data, plus cross-regional Patterns/Throughways documents. Marked tentative in places pending still-open city-level decisions (e.g. Byrd's own central conflict).

## The six subnets and their cities (as of 2026-07-12)

- **Halley subnet:** Abowasa, Belgrano, Halley, Lazar, Neumayer, Princess Elisabeth, Sanay, Troll
- **Janbogo/Ross subnet:** Cape Adare, Denison, Dumont d'Urville, Fort McMurdo (Tepenia's historical capital), Janbogo, Scott, Zukelli
- **Mawson subnet:** Dome Fuji, Mawson, Sayowa
- **Mirny subnet:** Casey, Davis, Kunlun, Mirny, Shirayuki, Soyuz, Vostok, Zhongshan
- **Palmer subnet:** Esperanza, Juan Carlos, Marambio, Palmer City (Tepenia's first city), Port Lockroy, Rothera, Sejong, Signy
- **Byrd** — single-city subnet
- **Amundsen Station** — tracked separately from the 35-city count but essential to the whole-game picture

Plus **Concordia** — the last surviving Tepenian city in the present day (≈2822–2827), not itself part of a subnet, structured into its own 13 districts.

## What's already migrated here vs. what stays referenced

- Migrated: the handful of dated district-level events in `Timeline Eras/2 The Second Interwar Period/Timeline.md`'s "Confirmed Dated Events" table, city/character facts folded into specific Doll character files during backstory work (e.g. Zukelli/Janbogo's destruction, Fort McMurdo as historical capital, Casey's Megasheet existing — see `TODO.md`), and a first dedicated location file: `Worldspace/Locations/Juan_Carlos.md` — origin of Tepenia's first bureaucratic archive, later consolidated into Amundsen Station's own archive (see `Reference/World_History_Reference.md`'s Machu Picchu Border & Customs Authority section), destroyed in the Long Night War for that same function.
- Referenced only: everything else above. If a future session needs deep city or district detail, go to InnerTepeniaGDD directly rather than assuming it's been brought over.
- **Standing rule for any future location file:** a city's real-world founding nation is a GPS fact only — never a source of inherited culture, faction conflict, or in-world explanation. See `Reference/No_National_Stereotypes.md` before writing a new location's Character & Culture section.
