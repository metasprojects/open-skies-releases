# Data credits and licences

Every map in this series is built from open data by Open Skies, the open-source (MIT) map maker at
https://github.com/metasprojects/open-skies. This repository holds the map files only. The data is not ours,
and each source keeps its own licence. When you pass on a map, or anything built from one, pass on the notices
below with it.

Checked 2026-11-06. Licence pages change: re-read the links before each release.

## Elevation: Copernicus DEM GLO-30

- Used for: all land heights (30 m grid), from the AWS Registry of Open Data (`copernicus-dem-30m`).
- Licence: the Copernicus DEM licence for GLO-30 (free, worldwide, including redistribution of modified data,
  with the notices below).
- Required notice:
  > produced using Copernicus WorldDEM-30 © DLR e.V. 2010-2014 and © Airbus Defence and Space GmbH 2014-2018
  > provided under COPERNICUS by the European Union and ESA; all rights reserved.
- Required liability sentence:
  > The organisations in charge of the Copernicus programme by law or by delegation do not incur any liability
  > for any use of the Copernicus WorldDEM-30.
- Also required: never suggest that Airbus Defence and Space, DLR, ESA, the European Union or Copernicus endorse
  the map, its author or its use. Anyone who passes on data derived from the DEM takes on the same duties.

## Land cover: ESA WorldCover 2021 v200

- Used for: ground colour and texture weights (cities, cropland, forest, grass, bare rock, water), 10 m.
- Licence: CC BY 4.0.
- Notice:
  > © ESA WorldCover project 2021 / Contains modified Copernicus Sentinel data (2021) processed by ESA WorldCover
  > consortium.

## Roads, buildings, ferry routes, land use: Overture Maps (OpenStreetMap)

- Used for: road network for ground AI, building positions and heights, ferry routes, water and land use.
  Release `2026-10-21.0`.
- Licence: ODbL 1.0 for the transportation, buildings and base themes (OpenStreetMap-derived);
  CDLA-Permissive-2.0 for places (not used today).
- Notice:
  > © OpenStreetMap contributors, Overture Maps Foundation. Available under the Open Database License
  > (https://www.openstreetmap.org/copyright).
- Share-alike: the road, building and ferry data inside a map is a derivative of OpenStreetMap and stays under
  ODbL 1.0. Anyone may extract and reuse it on those terms, and each map page offers the derived layers on
  request (open an issue here).
- Some Overture features come from sources other than OpenStreetMap (for example machine-learned building
  footprints, or TomTom in transportation). Their `sources` field names them; credit any such source that a map
  actually uses, as listed on https://docs.overturemaps.org/attribution/.

## Ship lanes: World Bank Global Shipping Traffic Density

- Used for: where AI ships sail (six years of AIS ship positions, 2015-2021, 0.005° cells).
- Licence: CC BY 4.0.
- Credit:
  > Global Shipping Traffic Density, World Bank. Data obtained through a partnership with the IMF, as part of
  > IMF's World Seaborne Trade Monitoring System (Cerdeiro, Komaromi, Liu and Saeed, 2020).

## Sea floor: Terrain Tiles on AWS (Mapzen / Tilezen joerd)

- Used for: sea depth (Terrarium PNG tiles, `s3://elevation-tiles-prod`).
- Required attribution (verbatim, from https://github.com/tilezen/joerd/blob/master/docs/attribution.md; give
  the lines for the regions a map covers, or all of them):
  > * ArcticDEM terrain data DEM(s) were created from DigitalGlobe, Inc., imagery and funded under National
  >   Science Foundation awards 1043681, 1559691, and 1542736;
  > * Australia terrain data © Commonwealth of Australia (Geoscience Australia) 2017;
  > * Austria terrain data © offene Daten Österreichs – Digitales Geländemodell (DGM) Österreich;
  > * Canada terrain data contains information licensed under the Open Government Licence – Canada;
  > * Europe terrain data produced using Copernicus data and information funded by the European Union - EU-DEM layers;
  > * Global ETOPO1 terrain data U.S. National Oceanic and Atmospheric Administration
  > * Mexico terrain data source: INEGI, Continental relief, 2016;
  > * New Zealand terrain data Copyright 2011 Crown copyright (c) Land Information New Zealand and the New Zealand
  >   Government (All rights reserved);
  > * Norway terrain data © Kartverket;
  > * United Kingdom terrain data © Environment Agency copyright and/or database right 2015. All rights reserved;
  > * United States 3DEP (formerly NED) and global GMTED2010 and SRTM terrain data courtesy of the U.S. Geological Survey.
- Per map: Taiwan Strait, Korea, Hormuz and Falklands need the Global ETOPO1 and USGS GMTED2010/SRTM lines;
  Lofoten & Narvik adds "Norway terrain data © Kartverket" and, if the tiles there use it, the ArcticDEM line.

## Airports: OurAirports

- Used for: runway positions, lengths, headings and idents.
- Licence: public domain. Credited as a courtesy: OurAirports (https://ourairports.com).

## Software we work with (not shipped in maps)

- NOCustomMaps (MIT): the BepInEx plugin that loads these maps. Players install it from the Nuclear Option Mod
  Manager.
- Unity 2022.3.62f2 (Unity Personal licence) builds the map bundles.

## Nuclear Option

This project is an unofficial community modification and is not affiliated with, sponsored by, or endorsed by
Shockfront Studios Pty Ltd. Original Nuclear Option assets, vehicle designs, audio, and code are Copyright (c)
2026 Shockfront Studios Pty Ltd. All rights reserved. Nuclear Option and Shockfront Studios are trademarks or
registered trademarks of Shockfront Studios Pty Ltd. Original mod content and all other trademarks belong to
their respective owners.

Mods for Nuclear Option may not be sold, monetised or put behind paywalls. Nothing here contains game files.
