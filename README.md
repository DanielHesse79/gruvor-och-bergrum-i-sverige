# Gruvor och bergrum i Sverige

Interaktiv karta över gruvor, bergrum, bunkrar och mineralrättigheter i hela Sverige.
Kartan är en helt fristående HTML-fil ([`index.html`](index.html)) byggd med [Leaflet](https://leafletjs.com/) och markörklustring – ingen server eller installation behövs, öppna filen i en webbläsare.

För en mer detaljerad variant över bara Uppland, se [gruvor-och-bergrum-i-uppland](https://github.com/DanielHesse79/gruvor-och-bergrum-i-uppland).

## Innehåll

| Lager | Antal | Källa |
|---|---|---|
| Malmgruvor (nedlagda) | ~10 000 | SGU |
| Kalk-/industrimineralbrott (nedlagda) | ~2 000 | SGU |
| Stenbrott & täkter (nedlagda) | ~3 500 | SGU |
| Gruvor/täkter i drift | ~600 | SGU |
| Gruvor/schakt enligt OSM | ~760 | OpenStreetMap |
| Bergrum & underjordsanläggningar | ~270 | OpenStreetMap + egna efterforskningar |
| Bunkrar & fort | ~2 300 | OpenStreetMap |
| Skyddsrum | ~180 | OpenStreetMap |
| Mineralrättigheter (polygoner) | ~1 290 | Bergsstaten/SGU |

Totalt visas ca **16 000 gruvor/brott/täkter** från SGU plus ca **3 500 OSM-objekt**. Punkterna klustras automatiskt – zooma in för att se enskilda objekt.

Funktioner: tändbara lager, ämnesfilter (klickbara chips för metaller och mineral), sökruta, tre bakgrundskartor (OSM, OpenTopoMap, Esri flygfoto) och popup med detaljer och källa för varje objekt.

## Datakällor och licenser

- **SGU – Mineralresurser**: hämtat via [SGU:s öppna data-API](https://api.sgu.se/oppnadata/mineralresurser/ogc/features/v1/collections) (OGC API Features). Endast objekt med status *mine/quarry* och *closed mine/quarry* visas (faktiska gruvor/brott/täkter) – prospekt och geokemiska anomalier är utelämnade. Licens: [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
- **OpenStreetMap** (gruvschakt, stollgångar, bergrum, bunkrar, fort, skyddsrum): hämtat via Overpass API. © OpenStreetMap-bidragsgivare, licens [ODbL](https://www.openstreetmap.org/copyright).
- **Bergsstaten/SGU – Mineralrättigheter**: undersökningstillstånd, bearbetningskoncessioner och markanvisningar ur SGU:s nedladdningsbara GPKG. Se [`mineral_sweden.json`](mineral_sweden.json).

Bakgrundskartor laddas från respektive tjänst (OSM, OpenTopoMap, Esri) och kräver internetuppkoppling.

## Förbehåll

Datat är ett ögonblicksavläst utdrag (juni 2026) och kan innehålla fel. Gamla gruvhål kan vara livsfarliga – besök på egen risk och respektera privat mark. Kartan är ett hobbyprojekt och inte en officiell produkt från SGU eller Bergsstaten.

## Licens

Kod: MIT. Data: enligt respektive källas licens ovan.
