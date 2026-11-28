# Hiking Sim — live season data

This year's weather, snowpack and fires along each trail, for Hiking Sim's live season. A GitHub Actions job rebuilds
these files twice a day (`LIVE=1 scripts/bake-season.mjs` in the app's repo) and replaces this repo's single commit,
so it never grows.

One file per trail: `pct.json`, `cdt.json`, `at.json`, `azt.json`, `hayduke.json`, `pnt.json`, `adt.json`, `ft.json`.

Sources: Open-Meteo forecast and historical weather APIs (CC BY 4.0), USDA NRCS SNOTEL, NOAA NCEI GHCN-Daily, NIFC
WFIGS wildfire perimeters.
