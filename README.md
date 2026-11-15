# Mosteiro de Flor da Rosa

An interactive guide to the Monastery of Santa Maria de Flor da Rosa, in Crato (Alto Alentejo, Portugal): the 14th-century fortress-church and palace of the Order of the Hospital, now the Pousada Mosteiro do Crato. You can move through it floor by floor, era by era, from the founder's square of walls before 1340 to the hotel today.

The site is in Portuguese, English and Dutch.

**Live site** (once GitHub Pages is on, see below): https://madalenarb.github.io/Mosteiro-Flor-da-Rosa-site/

## What's inside

- **Timeline:** 70 dated events from the Order's founding in Jerusalem (1048) to the Pousada (1995 onward). Tap a date to read what happened.
- **The Pousada today:** floors 0 to 6 drawn as plans in one shared frame, so you can see how the floors stack and where the new wing meets the monastery. Photos are pinned where they were taken.
- **How it grew:** every wall coloured by building period, conjectural reconstructions of the first three phases, elevations, a section and the towers.
- **The 1615 plan:** Pedro Nunes Tinoco's manuscript plan, with every note transcribed and translated, and the matching view of the monastery on a Portalegre tapestry.
- **Stories:** histories, traditions and legends, each with its sources and how far it can be trusted.
- **The Order:** the Hospitallers from Jerusalem to Malta and the Priory of Crato, with maps of the Holy Land and of the Order's commanderies in Portugal.
- **Visiting:** the town walk from Flor da Rosa to Crato, the Historical Route to the Anta do Tapadão dolmen (PR1 CRT), places to eat, and how to book the Pousada.

## Run it

No build step and no server. Download or clone the repository and open `index.html` in a browser. It works offline: the fonts, maps and photos are all in the repository.

## Structure

| Path | Contents |
| --- | --- |
| `index.html` | The page, its fixed texts in three languages and the plan drawings (as `<template>` elements) |
| `css/estilo.css` | Layout and colours, light by default, with dark and automatic modes in the menu |
| `css/fontes.css`, `fontes/` | Barlow, Barlow Semi Condensed and EB Garamond, with their licences |
| `js/app.js` | Menu, maps, timeline, photo viewer and the texts that change with the language |
| `js/dados.js` | The numbered 1980 plans, the notes on the 1615 plan and the stories with their sources |
| `photos/`, `thumbs/` | Photographs, full size and thumbnails |
| `maps/`, `elev/`, `plan.jpg` | Region maps, elevation images and the 1615 manuscript plan |
| `desenhos/` | Every plan, elevation and map as a standalone SVG, for printing or editing |

## Editing texts

Every text exists in three languages. In `js/app.js` and `js/dados.js` they look like `{pt:"…",en:"…",nl:"…"}`. In `index.html` they are sibling elements marked `data-l="pt"`, `data-l="en"` and `data-l="nl"`. Save and reload the page to see the change.

## Publishing with GitHub Pages

In the repository, open **Settings → Pages**, set **Source** to *Deploy from a branch*, choose **main** and **/ (root)**, and save. After a minute or two the site is live at the address above.

## Sources and credits

- History: the monastery's exhibition panels and chronology; Jorge Rodrigues and Paulo Pereira, *O Mosteiro de Flor da Rosa: do Priorado do Crato ao Panteão de Álvaro Gonçalves Pereira* (By the Book, 2023); Paula Pinto Costa (2014); SIPA and Património Cultural; Crato council. Each story on the site lists its own sources.
- Maps: data © OpenStreetMap contributors, available under the Open Database Licence (ODbL).
- Fonts: SIL Open Font License, via Fontsource.
- Photographs: by the author unless stated. Photos of the exhibition panels and some photos of the surroundings belong to their owners, for example the interior of the Igreja Matriz do Crato by Rui Ponte e Sousa (2017).

Texts, drawings and the author's photographs: all rights reserved.

---

**Em português:** guia interativo do Mosteiro de Flor da Rosa, no Crato, hoje Pousada Mosteiro do Crato. Abra `index.html` no navegador; funciona sem internet. Mais detalhes em [LEIA-ME.md](LEIA-ME.md).
